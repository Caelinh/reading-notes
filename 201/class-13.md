# Local storage

### [Local Storage and How To Use It On Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

**Why would a developer use local storage for a web application?**  
To store a state of the site for a user so that they wouldn't have to restart everytime they came to the site. HTTP is stateless by design so the developer needs to work
aroud that with local storage and server storage.
  
**What information should not be stored in local storage?**  
Server side states such as login storage. A key to access the object on the server would be okay but the account object itself, not so much.  
**Local storage can store what type of data? How would you convert it to that type before storing?**  
Local storage can only store strings. things can be converted to string by using the `JSON.stringify()` and `JSON.parse()` methods.  
  ```
  var car = {};
car.wheels = 4;
car.doors = 2;
car.sound = 'vroom';
car.name = 'Lightning McQueen';
console.log( car );
localStorage.setItem( 'car', JSON.stringify(car) );
console.log( JSON.parse( localStorage.getItem( 'car' ) ) );

```
![picture of this output](https://cloud.netlifyusercontent.com/assets/344dbf88-fdf9-42bb-adb4-46f01eedd629/1c7f4cfb-16dc-40c8-9b56-644a1792a3c2/console-e1285930679229.png)
