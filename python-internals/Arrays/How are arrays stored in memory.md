# How are arrays stored in memeory of  computer?

- Computer can only understand 0s & 1s. Hence all the data we store, is stored in 0s and 1s in computer after translation into byte code by the interpreter.

- Arrays are nothing but data stores contineously.
- Now when you ask compute to store an array (By declaring it via a variable), behind the scene each value in array is stored as a byte (8 bits) with corresponding address but contineously.

- 1 byte = 8 bits => _ _ _ _ _ _ _ _

- Arrays are super useful when you want the data to be store on next to other and when you want the add or remove  or retrieve from array in O(1) time complexity.

- There are two types of arrays:
    - Static arrays
    - Dynamic arrays