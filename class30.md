# Class 30 (HashTabels)

## Why

Hash tables are crucial in programming because they provide a fast and efficient way to store and retrieve data. They excel at quick searches, insertions, and deletions, making them ideal for scenarios where speedy access to information is essential. The magic lies in their ability to map keys to specific locations, allowing for constant time complexity on average for common operations.


## What

A hash table is a data structure that organizes data using a hash function, which takes an input (or key) and returns a unique index where the corresponding value is stored. In Java, you might create a hash table using the HashMap class. For instance, you could use it to associate names with ages, where the names are the keys and the ages are the values.

here is an example:

```
HashMap<String, Integer> ageMap = new HashMap<>();

ageMap.put("ghaidaa", 21);

ageMap.put("gg", 24);

int aliceAge = ageMap.get("ghaidaa"); // retrieves the age associated with the key "ghaidaa"
```

## How

To implement a hash table, you need a hash function to convert keys into indices. In Java, the hashCode() method is commonly used for this purpose. The hash table then uses these indices to store and retrieve values. Handling collisions (situations where different keys hash to the same index) is a critical consideration. Techniques like chaining (using linked lists at each index) or open addressing (finding the next open slot) are employed to address collisions and maintain the integrity of the hash table.
