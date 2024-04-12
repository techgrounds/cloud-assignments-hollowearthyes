# Passwords
Understanding Password Hashing, Rainbow Tables, and Salting in Linux

## Key-terms
- Password hashing: The process of converting a plaintext password into a fixed-length string of characters using a cryptographic hash function.
- Symmetric encryption: A type of encryption where the same key is used for both encryption and decryption.
- Rainbow Table: A precomputed table for reversing cryptographic hash functions, typically used to crack passwords.
- Salt: A random value appended to passwords before hashing to prevent the same password from generating the same hash.

## Opdracht
1. **Password Hashing vs. Symmetric Encryption:** Password hashing is preferred over symmetric encryption for storing passwords because:
   - Hashing is a one-way function, meaning it cannot be reversed to obtain the original password.
   - Even if the hashed password is stolen, it's computationally infeasible to reverse the hash back to the original password.
   - Hashing provides unique hashes for each input, ensuring that even similar passwords will have vastly different hashes.
   
2. **Using Rainbow Tables to Crack Hashed Passwords:**
   - Rainbow tables are databases of precomputed hashes for commonly used passwords.
   - Attackers use rainbow tables to compare stolen hashed passwords against the precomputed hashes to find matches.
   - If a match is found, the corresponding plaintext password can be determined.
   
3. **MD5 Hash Lookup:**
   - Two MD5 hashes are provided: 
     1. 03F6D7D1D9AAE7160C05F71CE485AD31: 	md5	welldone!
     2. 03D086C9B98F90D628F2D1BD84CFA6CA: (unkown)
   - Use an online Rainbow Table (e.g., crackstation.net) to attempt to crack these hashes and determine the original passwords.

4. **Linux User Creation and Salting:**
   - Create a new user in Linux with the password "12345".
   - Attempt to crack the hashed password "12345" using a Rainbow Table.
   - Note that despite being a weak password and using common hashing algorithms, you won't find a match in the Rainbow Table due to salting.
   
5. **Understanding Salting:**
   - Salting involves appending a random value to each password before hashing.
   - The salt value ensures that even if two users have the same password, their hashed passwords will be different.
   - To understand salting, compare the hashed password of "12345" with a peer who also has the same password in their /etc/shadow file.

## Gebruikte bronnen
- Explanation of Password Hashing: (https://en.wikipedia.org/wiki/Cryptographic_hash_function)
- Understanding Rainbow Tables: (https://en.wikipedia.org/wiki/Rainbow_table)
- Introduction to Salting: (https://en.wikipedia.org/wiki/Salt_(cryptography))
- Rainbow table: (https://crackstation.net/)

## Ervaren problemen
- No major issues were encountered during the execution of the tasks. Ensure proper permissions and access to necessary tools and directories in the Linux environment.

## Resultaat
- The success of the task can be confirmed by attempting to crack the provided MD5 hashes and the password "12345" using a Rainbow Table. Additionally, comparing the hashed password of "12345" with a peer's hashed password will illustrate the impact of salting.