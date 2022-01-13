# Read: Hash Tables

Hash tables are another type of a data structure. The reason it is used is to increase the efficiency of accessing the data stored in it.
Ideally, acessing the needed data from a hash table takes O(1) time complexity. This means, that no matter how many elements are stored in the hash table, it will take exactly the same aamount if time to find one.

Typically, the base structure of a hash table is an array. As we remember, if we want to access a certain element of an array by its index, we write `array[i]`. Such operation takes O(1) time complexity. Hash tables are also utilizing this method to grab an element. But the trick is you have to know at what index your element is located. 

With hash tables, the whole logic begins with the process placing an element into an array. It is done a certain way. One thing we also have to know though, is the size of the array (unless we are talking about automatically expanding hash table, which is a different beast). When we create an array of a certain length, all of it slots
are empty. Then we start placing elements in it. And this is where our hash alogrithm comes in. We have to have a function, that does a computation on an element, and tells us at what index the array should be placed. We can also use the same function to find out what index the element was supposed to be at, when we are searching for this element.

Normally, hash tables work with key-value pairs. We give the function a key as a parameter, it will do some computation on that key, and tell us an index of where the key-value pair will be placed at. So, if we want to find a value of a given key, we need to provide the function the key.

One common method the algorithm computes an index given a key is this. Each alpha-numeric character has an ASCII code, which is a number. So, it sums up each character's ASCII codes. Then it divides the sum by the length of an array (as we said earlier, the function needs to know the length). What ever the remainder of that division is, will be our index. For example, if we try to divid 19 by 5, there will be a remainder of a 5, because 19 is not divisible by 5. The closest lower number that can be divided is 15. And some, the remaining for is not divisible. This is also called "modulo".

There are a big possibility of collisions though. In that case, both elements will be stored at the same index of an array. However, in a form of a linked list. So, finding an element means traversing such linked list.

## Resources

Read [Intro to Hash Tables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
Watch [what is a hash table?](https://www.youtube.com/watch?v=MfhjkfocRR0)
Read [basics of hash tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
Skim [hash table wiki](https://en.wikipedia.org/wiki/Hash_table)

[**<== BACK**](401-toc.md)