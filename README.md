# CODE REFACTORING

## Description

We tried to improve a [javascript code](https://github.com/hei-school/cc-d4-rice-cooker-ci-NyAndoMayah/blob/feat/js/js/main.js) from school project, and [here](https://github.com/fenohasinalala/test-cc/blob/main/main.js) are the results.

## Complexity analysis

### 1. Definitions

#### 1.1 Complexity

In the field of algorithm design and analysis, it is essential to understand complexity, particularly with regard to time and space. Our goal is often to design algorithms that are efficient in terms of their use of time and space.

#### 1.2 Time complexity

Temporal complexity refers to the time required to execute an algorithm.
An algorithm with a time complexity of O(n) implies that its execution time increases linearly with the size of the input. 
If the size of the input doubles, the execution time of the algorithm will also double.

#### 1.3 Spatial complexity

Spatial complexity refers to the amount of memory an algorithm needs to execute.
An algorithm with a space complexity of O(n), means that the memory required by the algorithm grows linearly with the size of the input data.

### 2. Analysis

#### 2.1 addRice()

##### 2.1.1 Initial implementation

The function contains only constant time compexity operations,
The case with  most operations

    Check if this.ricePresent is false.
        Time Complexity: O(1)
    Initialized variables
        Time Complexity: O(1)
    Print a message.
        Time Complexity: O(1)
    Check for the else statement.
        Time Complexity: O(1)

    Total Time Complexity for addRice():
        O(1)+O(1)+O(1)+O(1)= 4*O(1) = O(1)

The function has a constant time complexity of O(1) because it only performs a single check and either adds rice or prints a message. The number of operations does not depend on the size of any input or data structure.

##### 2.1.2 New implementation

The function contains only constant time compexity operations,
The case with  most operations

    Check if this.ricePresent is false.
        Time Complexity: O(1)
    Initialized variables
        Time Complexity: O(1)
    Print a message.
        Time Complexity: O(1)
    Return from the function.
        Time Complexity: O(1)O

    Total Time Complexity for addRice():
        O(1)+O(1)+O(1)+O(1)= 4*O(1) = O(1)

The function has a constant time complexity of O(1) because it only performs a simple check and prints a message based on the value of the 'ricePresent' variable. The execution time does not depend on the size of any input or any loops, making it constant.

##### 2.1.3 Conclusions

In both the old and new code versions, the addRice() function has a constant time complexity of O(1) as it consists of a series of constant time operations.

Regarding space complexity, both versions have a constant space complexity of O(1) as they do not use additional memory that scales with the input.

#### 2.2 cookRice()

##### 2.2.1 Initial implementation

The function contains only constant time compexity operations,
The case with  most operations

    Check if this.ricePresent is true and this.riceCooked is false.
        Time Complexity: 2*O(1)

    Print a message.
        Time Complexity: O(1)

    Introduce a fixed delay of 1500 milliseconds (this.delaySync(1500)).
        Time Complexity: O(1)

    Set this.riceCooked to true.
        Time Complexity: O(1)

    Print a message.
        Time Complexity: O(1)

    Check if this.ricePresent is false
        Time Complexity: O(1)
        
    Check for the else statement.
        Time Complexity: O(1)

    Total Time Complexity for cookRice():
        2*O(1)+O(1)+O(1)+O(1)+O(1)+O(1)+O(1) = 8*O(1) = O(1)

The function has a constant runtime complexity of O(1) because it only performs a fixed number of operations regardless of the input size. The if-else statements and console.log statements all have constant time complexity.

##### 2.2.2 New implementation

The function contains only constant time compexity operations,
The case with  most operations

    Check if this.ricePresent is true and this.riceCooked is false.
        Time Complexity: 2*O(1)

    Print a message.
        Time Complexity: O(1)

    Set this.riceCooked to true.
        Time Complexity: O(1)

    Introduce a fixed delay of 1500 milliseconds (this.delaySync(1500)).
        Time Complexity: O(1)

    Print a message.
        Time Complexity: O(1)

    Return from the function.
        Time Complexity: O(1)

    Total Time Complexity for cookRice():
        2*O(1)+O(1)+O(1)+O(1)+O(1)+O(1)= 7*O(1) = O(1)

Same as the old code, the function has a constant time complexity because it only performs a fixed number of operations regardless of the input size. The overall time complexity is O(1).

##### 2.2.3 Conclusions

In both the old and new code versions, the cookRice() function has a constant time complexity of O(1) as it consists of a series of constant time operations.

Regarding space complexity, both versions have a constant space complexity of O(1) as they do not use additional memory that scales with the input.

#### 2.3 steam()

##### 2.3.1 Initial implementation

The function contains only constant time compexity operations,
The case with  most operations

    Check if this.ricePresent is true and this.steamingInProgress is false.
        Time Complexity: 2*O(1)

    Print a message.
        Time Complexity: O(1)

    Set this.steamingInProgress to true.
        Time Complexity: O(1)

    Introduce a fixed delay of 1500 milliseconds (this.delaySync(1500)).
        Time Complexity: O(1)

    Set this.steamingInProgress to false.
        Time Complexity: O(1)

    Print a message.
        Time Complexity: O(1)
    
    Check if this.ricePresent is false
        Time Complexity: O(1)
        
    Check for the else statement.
        Time Complexity: O(1)

    Total Time Complexity for steam():
        2*O(1)+O(1)+O(1)+O(1)+O(1)+O(1)+O(1)= 9*O(1) = O(1)

The function has a constant runtime complexity of O(1) because it only performs a fixed number of operations regardless of the input size. The if-else statements and console.log statements all have constant time complexity.

##### 2.3.2 New implementation

The function contains only constant time compexity operations,
The case with  most operations

    Check if this.ricePresent is true and this.steamingInProgress is false.
        Time Complexity: 2*O(1)

    Print a message.
        Time Complexity: O(1)

    Set this.steamingInProgress to true.
        Time Complexity: O(1)

    Introduce a fixed delay of 1500 milliseconds (this.delaySync(1500)).
        Time Complexity: O(1)

    Set this.steamingInProgress to false.
        Time Complexity: O(1)

    Print a message.
        Time Complexity: O(1)

    Return from the function.
        Time Complexity: O(1)

    Total Time Complexity for steam():
        2*O(1)+O(1)+O(1)+O(1)+O(1)+O(1)+O(1)= 8*O(1) = O(1)

Same as the old code, the function has a constant time complexity because it only performs a fixed number of operations regardless of the input size. The overall time complexity is O(1).

##### 2.3.3 Conclusions

In both the old and new code versions, the steam() function has a constant time complexity of O(1) as it consists of a series of constant time operations.

Regarding space complexity, both versions have a constant space complexity of O(1) as they do not use additional memory that scales with the input.

#### 2.4 keepWarm()

Using the same method to calculate the complexity of previous functions:

    Old implementation time complexity = 7*O(1) = O(1)

    New implementation time complexity = 6*O(1) = O(1)

both versions of the function have a constant time complexity of O(1) because they only perform a fixed number of operations regardless of the input size.

Regarding space complexity, both versions have a constant space complexity of O(1) as they do not use additional memory that scales with the input.

#### 2.5 removeRice()

Using the same method to calculate the complexity of previous functions:

    Old implementation time complexity = 8*O(1) = O(1)

    New implementation time complexity = 9*O(1) = O(1)

both versions of the function have a constant time complexity of O(1) because they only perform a fixed number of operations regardless of the input size.

Regarding space complexity, both versions have a constant space complexity of O(1) as they do not use additional memory that scales with the input.

#### 2.6 simulateRiceCooker()

Using the same method to calculate the complexity of previous functions:

    Old implementation time complexity = 2*O(1) + O(n) = O(n)
    (to the last else if)

    New implementation time complexity = 7*O(1) + 0(n) = O(n)

both versions of the function have a constant time complexity of O(n) because they perform a number of operations depending on the number of input.

Regarding space complexity, both versions have a constant space complexity of O(n) as they do not use additional memory that scales with the input.

#### 2.7 delaySync()

Didn't modify the delaySync function, so let's see it's complexity.

    Initialize start with the current timestamp.
        Time Complexity: O(1)

    Enter a loop that continues until the difference between the current timestamp and start reaches "n".
        Time Complexity: O(n)

    Total Time Complexity for delaySync(n):
        O(1)+O(n)=O(n)

 The delaySync(n) function has a linear time complexity of O(n) because the time taken to execute the function scales linearly with the value of n.
