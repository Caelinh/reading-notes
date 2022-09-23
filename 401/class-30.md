# Datastructures: Hash Table

1. Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
2. Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
3. Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

 Hash tables are used to find values with key value pairs. The value is held in a bucket or node that can be accessed by finding it's correspodning key.  
 
 ## Structure

### Hashing
Basically, a hash code turns a key into an integer. It’s very important that hash codes are deterministic: their output is determined only by their input. Hash codes should never have randomness to them. The same key should always produce the same hash code.  

### Creating a hash

A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement. After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value.  
Here is a simplistic hashing algorithm:
1. Add or multiply all the ASCII values together.
2. Multiply it by a prime number such as 599.
3. Use modulo to get the remainder of the result, when divided by the total size of the array.
4. Insert into the array at that index.
 
 ### Collisions
 The thing that must be avoided in hash maps. If two vales are stored in the same key there is a collision. One way to circumvent this is to have each bucket be a linked list
this way the other value will be added to the key without overriding whats already saved. Store the key pair together saving to a hash map to keep track of the pair.

- To Store Values
  - accept a key
  - calculate the hash of the key
  - use modulus to convert the hash into an array index
  - store the key with the value by appending both to the end of a linked list

- To read value
  - accept a key
  - calculate the hash of the key
  - use modulus to convert the hash into an array index
  - use the array index to access the short LinkedList representing a bucket
  - search through the bucket looking for a node with a key/value pair that matches the key you were given

## Methods
**set()**  
When adding a new key/value pair to a hashtable:  

- send the key to the hash() method.
- Once you determine the index of where it should be placed, go to that index
- Check if something exists at that index already, if it doesn’t, add it with the key/value pair.
- If something does exist, add the new key/value pair to the data structure within that bucket.
**get()**  
The get() method takes in a key, gets the Hash, and goes to the index location specified. Once at the index location is found in the array, it is then the responsibility of the algorithm the iterate through the bucket and see if the key exists and return the value.

**has()**  
The has() method will accept a key, and return a bool on if that key exists inside the hashtable. The best way to do this is to have the contains call the hash() method and check the hashtable if the key exists in the table given the index returned.

**keys()**  
The keys() method returns a collection (array) of unique hash keys.

**hash()**  
The hash() method will accept a key as a string, conduct the hash, and then return the index of the array where the key/value should be placed

### Resources
https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html  
https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/  
https://www.youtube.com/watch?v=MfhjkfocRR0&ab_channel=PaulProgramming  
https://en.wikipedia.org/wiki/Hash_table  

 
