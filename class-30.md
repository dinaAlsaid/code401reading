# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-29) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-31)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Hashtables

A hash table is a data structure that uses a hash function to compute an index, called a hash code, into an array of buckets, from which the desired value can be found.  
Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.  
Collisions can happen when more than one key gets hashed to the same location of the hashtable.  

we can do a lookup in an O(1) time complexity.  

## Hashing

Basically, a hash code turns a key into an integer. It’s very important that hash codes are deterministic: their output is determined only by their input.  
Hash codes should never have randomness to them. The same key should always produce the same hash code.  
In hashing, large keys are converted into small keys by using hash functions.  
