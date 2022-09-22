# Local database using room

Good to use if you want cache some data for the user to use offline.

### Three major components

1. The database class that holds the database and serves as the main access point for the underlying connection to your app's persisted data.
2. Data entities that represent tables in your app's database.
3. Data access objects (DAOs) that provide methods that your app can use to query, update, insert, and delete data in the database.

Thee data is treated a lot like database entries done with postgres.  
**Create an entity**

````
@Entity
public class User {
    @PrimaryKey
    public int uid;

    @ColumnInfo(name = "first_name")
    public String firstName;

    @ColumnInfo(name = "last_name")
    public String lastName;
}
````
**Data access object**
````
@Dao
public interface UserDao {
    @Query("SELECT * FROM user")
    List<User> getAll();

    @Query("SELECT * FROM user WHERE uid IN (:userIds)")
    List<User> loadAllByIds(int[] userIds);

    @Query("SELECT * FROM user WHERE first_name LIKE :first AND " +
           "last_name LIKE :last LIMIT 1")
    User findByName(String first, String last);

    @Insert
    void insertAll(User... users);

    @Delete
    void delete(User user);
    }
    
````
    
**Database**
````
@Database(entities = {User.class}, version = 1)
public abstract class AppDatabase extends RoomDatabase {
    public abstract UserDao userDao();
}
````

### Resources
https://developer.android.com/training/data-storage/room  
https://developer.android.com/training/data-storage/room/accessing-data#java  
https://developer.android.com/training/data-storage/room/relationships  
https://developer.android.com/training/data-storage/room/defining-data  



