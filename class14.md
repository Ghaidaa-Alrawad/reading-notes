# Class 14 Reading

## Password hashing

### Define the term “hashing”.

Hashing is a process in computing where a mathematical algorithm takes an input (such as a password or any data) and transforms it into a fixed-length string of characters, typically in a hexadecimal format.

The key feature of hashing is that it is a one-way function, meaning it is easy to compute the hash from the input, but it is computationally infeasible to reverse the process and derive the original input from the hash.

Hashing is commonly used for securing data, including passwords, and for ensuring data integrity.

### Explain to a non-technical friend what a hash function does to a password.

Imagine a hash function as a magical blender for passwords. When you put your password into this blender, it processes it and turns it into a unique jumble of letters and numbers, like a secret code, and this code is the hash of your password.


Once your password is blended, there's no way to turn it back into the original password. It's a one-way transformation. So, when you log in somewhere, instead of storing your actual password, the system stores this secret code (the hash). When you enter your password, it gets blended again, and if the new code matches the stored one, you're granted access. It's like having a secret handshake that's impossible to figure out just by looking at it.

---

## Bcrypt Overview

### What does it mean to ‘salt’ a password?

Salting a password involves adding a long, random string of bytes (called a 'salt') to the password before it is hashed. This salt is unique for each password, making it different for every user. The purpose of salting is to increase the security of hashed passwords. Even if two users have the same password, their hashes will be different because of the unique salt. This prevents attackers from using precomputed tables (like rainbow tables) to easily crack passwords.

### What piece of information would a hacker need to access in order to find the ‘salt’ string for your passwords?

If a hacker gains access to the source code of the application or system, they can easily find the 'salt' string for passwords. This implies that the 'salt' is stored or generated within the application's source code. So, to find the 'salt' string, a hacker would need to somehow access and analyze the application's source code, which can be a security risk in itself.

---

## jBCrypt 

### How does the Blowfish block cipher handle the increased computation speed of new computers?

The Blowfish block cipher, as implemented in jBCrypt, is designed to handle the increased computation speed of new computers by allowing the computation cost of the hashing algorithm to be parameterized. This means that the cost can be increased as computers become faster. The parameterization is achieved through the "log_rounds" parameter, where the work factor is set as 2 to the power of "log_rounds." As computer hardware advances, you can increase the value of "log_rounds" to make the hashing process more computationally intensive and slower, thus frustrating fast hardware implementations and making it more difficult for attackers to crack passwords offline.

### What are the issue with the two most commong password hashes for Java (“Java password hash” and “Java password encryption”)?

- **Unsalted Hash:** One common approach uses an unsalted hash. This means that passwords are hashed without adding a unique random value (salt) to each password before hashing. Unsalted hashes are vulnerable to reverse dictionary attacks, where attackers can precompute hashes for a list of commonly used passwords and then compare them to the hashed passwords to discover matches.

- **Reversible Encryption:** Another approach recommends reversible encryption for password storage. Reversible encryption allows passwords to be decrypted back to their original form, which is generally not recommended for password storage. If an attacker gains access to the encrypted passwords and the decryption key, they can easily recover the plaintext passwords.

Both of these approaches have security vulnerabilities and are not considered best practices for password hashing in Java or in general. It's suggested that jBCrypt provides a more secure alternative for password hashing in Java by using the Blowfish block cipher with adaptive cost parameters to mitigate these vulnerabilities.