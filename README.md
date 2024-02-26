# class4

# Assignment #4 - Feb 26th to March 4th

###### *Solutions for previous assignments can be found here: https://github.com/ponceoscarj/nlp_python_pilot/tree/main*


## Overall Instructions
1. Watch the following video:
    1. Lecture 6: Recursion and Dictionaries. [[Link]](https://ocw.mit.edu/courses/6-0001-introduction-to-computer-science-and-programming-in-python-fall-2016/resources/lecture-6-recursion-and-dictionaries/)


## Python assignment

### Rules:
- Do not use classes or external packages (i.e., regex)
- Only "built-in" functions are allowed
- You cannot use the `count()` or the `pow()` functions.
- All of the questions are **mandatory!**

### Submission format:
- Submit your python code to your classroom repository
- Organise your coding by question (e.g., Q1.1.)

### 1. Creating the power function: 
Input in the form of tupple where base goes first and the exponent or power goes second.


Example:
```python
in_tupple = (3,4) # this would mean 3 raised to the power of 4 
output = 81 # output should be an integer

# Testing your function
in_tupple = (9,10)
result = 1048576
```

### 2. Modifying the power function:  
Modify your previous function so that it inputs a list and outputs another list

Example:
```python
input_list = [3, 4] # this would mean 3 raised to the power of 4 
output = [3, 81, 4] 
# output should be a list including the input [3,4] with the result in-between -> [3, 81, 4].
# base is in position 0 = 3
# exponent is in position 2 = 4
# result is in position 1 = 81

# Testing your function
in_list = [2, 3]
output = [2, 8, 3]
```

### 3. Making your power function interactive:  
You have to modify your previous function so that it does the following (see video):
- The first input prompt should be: "The base is: "
- The second input prompt should be: "The exponent is: "
- Once you give the function both (e.g. 2 and 3), it should print a list that has both inputs and the result at the end. For 2 and 3 the list should be: [2,3,8] because 2 to the power of 3 is 8. 
- **This function should run infinitely unless you input "finito"**

https://github.com/NLP-python-pilot/class4/assets/64445959/b01fec95-e31f-4d84-9389-7ff597bf2f8e

### 4. Create a function with a for loop:  

- Function that adds elements from list input_1 and elements from list input_2 based on their positions. The results should be similar to the one in output.
- For example, position 0 from `input_1` is 2 and position 0 from `input_2` is 4. When you add these numbers your result is 6 which is located in the position 0 from the `output` list.

```python
input_1 = [2, 4, 6, 8]
input_2 = [4, 10, 54, 3]
output = [6, 14, 60, 11]
```

### 5. Create a function to count positional differences and similarities:  

- **Input**: the input for the function should be two lists of words where each word have the same number of characters such as `input_1` and `input_2`. 
- **Output**: the function should return a list of lists containing the positional differences and similarities such as `output_lst`.  

```python
input_1 = ['woke', 'sleep', 'have', 'simple_word', 'of!course#']
input_2 = ['wake', 'steel', 'hour', 'not_a_word_', 'of$course#']

ouput_lst = [[3, 1], [3, 2], [1, 3], [0, 11], [9, 1]]
```

Description of the `output_lst` with examples:
- For the first word in both `input_1` and `input_2`, the position 0, 2, 3 are the same ("w", "k", "e") but the position 1 is different. The count for this should be `[3, 1]` which is first list (position 0) inside `output_lst`
- For the third word in both `input_1` and `input_2`, position 0 is the same ("h") and positions 1,2,3 are different. The results for this should be `[1, 3]` which is the third list (position 2) inside `output_lst`


