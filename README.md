# Tower of Hanoi Implementation

## Overview

This Java program implements the classic Tower of Hanoi puzzle using recursion. The Tower of Hanoi is a mathematical game or puzzle consisting of three rods and a number of disks of different sizes which can slide onto any rod. The puzzle starts with the disks stacked on one rod in order of decreasing size, with the smallest at the top, and the objective is to move the entire stack to another rod, following these rules:

1. Only one disk can be moved at a time.
2. Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack or on an empty rod.
3. No disk may be placed on top of a smaller disk.

## Implementation Details

The program is contained in a single Java class named `HanoiTowerUsingRecursion` within the `hanoi` package. It uses recursion to solve the puzzle for any given number of disks.

### Algorithm

The recursive algorithm for Tower of Hanoi can be described as follows:

1. Move n-1 disks from source rod to auxiliary rod
2. Move the nth disk from source rod to destination rod
3. Move n-1 disks from auxiliary rod to destination rod

### Time Complexity

The time complexity of this recursive solution is O(2^n), where n is the number of disks. This is because for n disks, we need to make 2^n - 1 moves.

### Space Complexity

The space complexity is O(n) due to the recursive call stack depth.

## How to Run

1. Ensure you have Java Development Kit (JDK) installed on your system.
2. Save the code in a file named `HanoiTowerUsingRecursion.java` within a directory structure that matches the package name (i.e., inside a folder named `hanoi`).
3. Compile the Java file using the command: `javac hanoi/HanoiTowerUsingRecursion.java`
4. Run the compiled program: `java hanoi.HanoiTowerUsingRecursion`

## Example Output

For n = 4 disks, the output will be a sequence of 15 moves (2^4 - 1) that solve the puzzle:

```
Move disk 1 from rod A to rod B
Move disk 2 from rod A to rod C
Move disk 1 from rod B to rod C
Move disk 3 from rod A to rod B
Move disk 1 from rod C to rod A
Move disk 2 from rod C to rod B
Move disk 1 from rod A to rod B
Move disk 4 from rod A to rod C
Move disk 1 from rod B to rod C
Move disk 2 from rod B to rod A
Move disk 1 from rod C to rod A
Move disk 3 from rod B to rod C
Move disk 1 from rod A to rod B
Move disk 2 from rod A to rod C
Move disk 1 from rod B to rod C
```

## Customization

To change the number of disks, modify the value of variable `n` in the `main` method.

```java
int n = 4; // Change this value to use a different number of disks
```

## Mathematical Background

The minimum number of moves required to solve the Tower of Hanoi puzzle is 2^n - 1, where n is the number of disks.

## Applications

The Tower of Hanoi has applications in:
- Teaching recursion concepts in computer science
- Backup rotation schemes
- Gray code generation in mathematical puzzles

## License

This implementation is provided for educational purposes and can be freely used and modified.

## Author

This implementation was created as a demonstration of recursive problem-solving in Java.

---

© 2025 Tower of Hanoi Java Implementation
