# Implementation: Hash Tables

- [Home](https://fadnesscharlie.github.io/reading-notes/401/)

## What are Hash Tables

Hash Tables are a way to store data. The main purpose of this is if you have a unique key value pair, but want to store them together in a way that is easy to access later.

We store that data by hashing the key, this will return back a certain number that is 0 to the size of our Hash Table. This lets us place it in a specific spot that we can grab later.

An example of this would lets say we want to store `UniqueKey: UniqueValue`.

If our size of our array is 1024. We know that it store in position number between 0 and 1024.

To get where we want to store our number, we first split the key into individual letters, then find the character code. We add all of these up, multiple by a prime number then divide by our array size to get back a remainder. This remainder is our position in the array.

If we have a collision, where two keys have the same position in the array, we create a Linked Link to store the data in the next, this allows us to keep our has table moving.

This is what a hash table is. At first it can be a little confusing, but once you understand it, it is actually amazing in how it all works and just how you can create an amazing way to store data and how fast you can grab that data back.

## Resources

- [Read Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
- [Watch what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)
- [Read basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
- [Skim hash table wiki](https://en.wikipedia.org/wiki/Hash_table)

## Things I want to know more about

- How hash tables are used in the world and when hash tables are the best cases of data storage.

Please visit my Github for more of my Projects!

[Charlie Fadness Github](https://github.com/fadnesscharlie)
