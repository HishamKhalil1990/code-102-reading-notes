# Hash tables
## Hash tables
### Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects. it result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. so hash table is a data structure that is used to store keys/value pairs.
### bucket is what is contained in each index of the array of the hashtable, where ollision is what happens when more than one key gets hashed to the same location of the hashtable.
## Why do we use them?
### we are using them for:
- Hold unique values
- Dictionary
- Library
## Structure
### Basically, a hash code turns a key into an integer. It’s very important that hash codes are deterministic, which means their output is determined only by their input. hashtable traditionally is created from an array. it always like the size 1024. 
### A collision occurs when more than one key hashes to the same index in an array. the worst possible hash is one that hashes every single key to the same exact index of an array.
### Hash Maps can have any number of buckets. If a hash map has only a few buckets it will be densely full and have many collisions. If a hash map has more buckets it will be more sparsely populated, there will be less collisions, but there may be a lot of extra empty space.
## Internal Methods
### When adding a new key/value pair to a hashtable:
- Add()
- Find()
- Contains()
- GetHash()
