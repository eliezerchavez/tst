## Programming Logic

1. **Basic Algorithms**  
   - Write a function to check if a number is prime.
   - Write a program that reverses a string.
   - Write a function that finds the greatest common divisor (GCD) of two numbers.

2. **Control Structures**  
   - Explain the difference between `for` and `while` loops. Provide an example of when to use each.
   - Write a program that prints the numbers from 1 to 100, but for multiples of three print "Fizz" instead of the number and for the multiples of five print "Buzz". For numbers which are multiples of both three and five, print "FizzBuzz".

3. **Data Structures**  
   - Explain what a linked list is and write a function to append a node to a singly linked list.
   - Describe the differences between an array and a list. Provide examples of when to use each.
   - Write a function to find the most frequent element in an array.

4. **Problem-Solving**  
   - Given an array of integers, write a function that returns the indices of the two numbers that add up to a specific target.
   - Describe how you would approach solving a new problem you have never seen before.

---

## Code Organization

1. **Code Readability**  
   - Explain why code readability is important.
   - Refactor the following code to improve its readability:
     ```python
     def f(a):
         if a % 2 == 0:
             return True
         else:
             return False
     ```

2. **Modularity**  
   - What are the benefits of modular programming?
   - Write a simple program that demonstrates the use of functions to create modular code. For example, a program that calculates the area and perimeter of a rectangle.

3. **Design Patterns**  
   - Explain what design patterns are and why they are useful.
   - Provide an example of a Singleton pattern in any programming language.
   - Describe the Factory pattern and provide a code example.

4. **Documentation**  
   - What are the best practices for documenting code?
   - Provide an example of a well-documented function.

---

## Source Code Management (Git)

1. **Basic Commands**  
   - Explain the purpose of the following Git commands: `clone`, `commit`, `push`, `pull`, `branch`, `merge`.
   - Describe the process of creating a new repository and pushing an initial commit.

2. **Branching and Merging**  
   - What is the difference between `git merge` and `git rebase`? When would you use each?
   - Demonstrate how to resolve a merge conflict.

3. **Collaboration**  
   - Explain the workflow of using feature branches in a team environment.
   - Describe how to use Git to review and approve changes before they are merged into the main branch.

4. **Advanced Topics**  
   - What is the purpose of a `git stash`? Provide an example of its usage.
   - Explain how to use Git tags and why they might be useful.
   - Describe how to set up a Git hook to enforce code quality checks before a commit.

## Code Analysis

### Python

1. **Function Analysis**  
   ```python
   def mystery_function(lst):
       return [x**2 for x in lst if x % 2 == 0]
   ```
   - What does this function do?
   - Provide an example input and the corresponding output.

2. **Loop and Conditional**  
   ```python
   def compute(a, b):
       result = 0
       for i in range(a, b):
           if i % 3 == 0 and i % 5 == 0:
               result += i
       return result
   ```
   - Explain what this function computes.
   - What is the output when `compute(1, 16)` is called?

### JavaScript

1. **Array Manipulation**  
   ```javascript
   function transformArray(arr) {
       return arr.map(item => item * 2).filter(item => item > 10);
   }
   ```
   - Describe what this function does.
   - Provide an example input and output.

2. **Callback Function**  
   ```javascript
   function doSomethingAsync(callback) {
       setTimeout(() => {
           callback("Hello, world!");
       }, 1000);
   }
   ```
   - Explain how this function works.
   - How would you call this function and handle its callback?

### TypeScript

1. **Generic Function**  
   ```typescript
   function identity<T>(arg: T): T {
       return arg;
   }
   ```
   - What does this function do?
   - Provide an example of how to use this function with a string and a number.

2. **Interface Implementation**  
   ```typescript
   interface Shape {
       area(): number;
   }

   class Rectangle implements Shape {
       constructor(public width: number, public height: number) {}

       area(): number {
           return this.width * this.height;
       }
   }
   ```
   - Describe how this code works.
   - Create an instance of `Rectangle` and call its `area` method.

### BASH

1. **Script Analysis**  
   ```bash
   #!/bin/bash
   for file in *.txt
   do
       mv "$file" "${file%.txt}.bak"
   done
   ```
   - What does this script do?
   - What would be the result of running this script in a directory containing `file1.txt` and `file2.txt`?

2. **Conditional and Loop**  
   ```bash
   #!/bin/bash
   count=0
   while [ $count -lt 5 ]
   do
       echo "Count is: $count"
       count=$((count + 1))
   done
   ```
   - Explain what this script does.
   - What will be the output when this script is executed?

### Java

1. **Class and Method**  
   ```java
   public class Counter {
       private int count = 0;

       public void increment() {
           count++;
       }

       public int getCount() {
           return count;
       }
   }
   ```
   - Describe what this class does.
   - How would you use this class in a Java program to count from 0 to 5?

2. **Control Flow**  
   ```java
   public class FizzBuzz {
       public static void main(String[] args) {
           for (int i = 1; i <= 20; i++) {
               if (i % 3 == 0 && i % 5 == 0) {
                   System.out.println("FizzBuzz");
               } else if (i % 3 == 0) {
                   System.out.println("Fizz");
               } else if (i % 5 == 0) {
                   System.out.println("Buzz");
               } else {
                   System.out.println(i);
               }
           }
       }
   }
   ```
   - What does this program print?
   - Explain the logic behind this program.

### C

1. **Pointer Usage**  
   ```c
   #include <stdio.h>

   void swap(int *a, int *b) {
       int temp = *a;
       *a = *b;
       *b = temp;
   }

   int main() {
       int x = 5, y = 10;
       swap(&x, &y);
       printf("x: %d, y: %d\n", x, y);
       return 0;
   }
   ```
   - What does the `swap` function do?
   - What will be the output of this program?

2. **Array Handling**  
   ```c
   #include <stdio.h>

   void printArray(int arr[], int size) {
       for (int i = 0; i < size; i++) {
           printf("%d ", arr[i]);
       }
       printf("\n");
   }

   int main() {
       int nums[] = {1, 2, 3, 4, 5};
       int size = sizeof(nums) / sizeof(nums[0]);
       printArray(nums, size);
       return 0;
   }
   ```
   - Explain how this program works.
   - What will be the output when this program is executed?
  
