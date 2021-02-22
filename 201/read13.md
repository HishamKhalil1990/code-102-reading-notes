# Local Storage
### local storage is used to store the client data local browser. Unlike cookies, the stored data is never transmitted to a remote web server. The storage is a pair values base. The data is stored by a name-key which is a string and the data value which can be any type of JavaScript supported data types. However, the data is actually stored as a string so to restore the value data type then methods as `parseInt()` and `parseFloat()` are used.
  1. **To store an item then `localStorage.setItem("nameKey", value);` or `localStorage["nameKey"] = value;`** 
  2. **To restore the item value then `localStorage.getItem("nameKey");` or `localStorage["nameKey"];`.** 
  3. **To remove an item then `removeItem("nameKey")`.**
  4. **To clear the storage then `clear();`**
  5. **To iterate through all of the name-keys stored by an index then `key(index);`.**
### The storage event is triggered on the window object when adding `setItem ();` , removing `removeItem();` or clearing `clear();` and actual changes are happened. The storage object is:
![ex](https://i.ibb.co/MntZqjp/2.jpg)
### Local storage is based in pair values only, so to store an item with more than one value then the web SQL database is use as in: 
![ex](https://i.ibb.co/Wfb6BRb/3.jpg)
