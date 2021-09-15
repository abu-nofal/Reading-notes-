# Hash Tables
--- 
> What is a hash table?

A hash table (often called a hash map) is a data structure that maps keys to values. Hash tables combine lookup, insert, and delete operations in an efficient way. The key is sent to a hash function that performs arithmetic operations on it. The result (called the hash value or hash) is an index of the key-value pair. 

---
> Hash tables are made up of two parts:

- **Object**: An object with the table where the data is stored. The array holds all the key-value entries in the table. The size of the array should be set according to the amount of data expected.
- **Hash function (or mapping function)**: This function determines the index of our key-value pair. It should be a one-way function and produce the a different hash for each key.

![](https://www.educative.io/api/page/4910944193871872/image/download/5155964159262720)

---
> Uses of hash tables

- Database indexing
- Caches
- Unique data representation
- Lookup in an unsorted array
- Lookup in sorted array using binary search

---
> What is a hash function?

A hash function is a method or function that takes an item’s key as an input, assigns a specific index to that key and returns the index whenever the key is looked up. This operation usually returns the same hash for a given key. A good hash function should be efficient to compute and uniformly distribute keys.

Hash functions help to limit the range of the keys to the boundaries of the array, so we need a function that converts a large key into a smaller key. This is the job of the hash function.

> Common hash functions 

- **Arithmetic Modular**
  - In this approach, we take the modular of the key with the list/array size: index=key MOD tableSize. So, the index will always stay between 0 and tableSize - 1.
- **Truncation**
  - Here, we select a part of the key as the index rather than the whole key. We can use a mod function for this operation, although it does not need to be based on the array size
- **Folding**
  - This approach involves dividing the key into small chunks and applying a different arithmetic strategy at each chunk.

---
> Hash table collisions

- **Linear probing**
  - Linear probing works by skipping over an index that is already filled. It could be achieved by adding an offset value to an already computed index. If that index is also filled, add it again and so on.

  ![](https://www.educative.io/api/page/4910944193871872/image/download/5691071517425664)
  
- **Chaining**
  - In the chaining strategy, each slot of our hash table holds a pointer to another data structure such as a linked list or a tree. Every entry at that index will be inserted into the linked list for that index.
  ![](https://www.educative.io/api/page/4910944193871872/image/download/4810203387133952)

- **Resizing the Array or List** 
  - Another way to reduce collisions is to resize the list or array. We can set a threshold and once it is crossed, we can create a new table which is double the size of the original. All we have to do then is to copy the elements from the previous table.

---
[ref](https://www.educative.io/blog/data-strucutres-hash-table-javascript?utm_term=&utm_campaign=%5BTest%5D+Dynamic+Verticals&utm_source=adwords&utm_medium=ppc&hsa_acc=5451446008&hsa_cam=14045073269&hsa_grp=128822123401&hsa_ad=535845844738&hsa_src=g&hsa_tgt=aud-470210443676:dsa-310094130363&hsa_kw=&hsa_mt=b&hsa_net=adwords&hsa_ver=3&gclid=Cj0KCQjws4aKBhDPARIsAIWH0JUT1vVdgeakmA95QTLHmgHPYDVN4OFwRKqzRP7_mx4_odUDBoqoeYoaAotbEALw_wcB)