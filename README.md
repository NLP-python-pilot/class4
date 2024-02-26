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
Your function should be able generate the power of any number and should have the following input and output:
- Input parameter: a tuple of two elements where the first element is the base and the second element is the exponent or power.
- Output: return result in the form of integer .

Example:
```python
in_tupple = (3,4) # Input -> 3 raised to the power of 4 
output = 81 # Output -> integer 81

# Test your function
in_tupple = (9,10)
result = 1048576
```

### 2. Modifying the power function:  
- Modify your previous power function so that the input parameter is one list where the first element (position 0) is the base and second element (position 1) is the exponent/power. 
- Your function should return another list containing your base, exponent/power, and result but in the following order `[base, result, exponent]` (as shown below)

Example:
```python
input_list = [3, 4] # Input -> 3 raised to the power of 4 
output = [3, 81, 4] # Output -> [base, result, exponent]

# Testing your function
in_list = [2, 3]
output = [2, 8, 3]
```

### 3. Making your power function interactive:  
You have to modify your previous function so that it does the following (see video):
- Your function does not require any input parameters.
- You should use the `input()` function two times within your function:
    - The first input prompt (`input()` function) should be: "The base is: "
    - The second input prompt (`input()` function) should be: "The exponent is: "
- Once you give both inputs to the function (e.g. 2 and 3), it should print a list with the following order `[base, exponent, result]`. For 2 and 3 the list should be: `[2,3,8]` because 2 to the power of 3 is 8. 
- **This function should run infinitely unless you input "finito"**

https://github.com/NLP-python-pilot/class4/assets/64445959/b01fec95-e31f-4d84-9389-7ff597bf2f8e

### 4. Create a function with a for loop:  
- Your function have two input parameters. Two lists with the same number of elements where each element is an integer such as `input_1` and `input_2`.
- The function should add elements from list input_1 and elements from list input_2 based on their position. The results should be similar to the one in the `output` list.
- For example, position 0 from `input_1` is 2 and position 0 from `input_2` is 4. When you add these numbers your result is 6 which is located in the position 0 from the `output` list.

```python
input_1 = [2, 4, 6, 8]
input_2 = [4, 10, 54, 3]
output = [6, 14, 60, 11]
```

### 5. Create a function to count positional differences and similarities:  

- **Input parameters**: the input parameters for the function should be two lists of words where each word have the same number of characters such as `input_1` and `input_2`. 
- **Output**: the function should return a list of lists containing the positional differences and similarities per word such as `output_lst`.  

```python
input_1 = ['woke', 'sleep', 'have', 'simple_word', 'of!course#']
input_2 = ['wake', 'steel', 'hour', 'not_a_word_', 'of$course#']

ouput_lst = [[3, 1], [3, 2], [1, 3], [0, 11], [9, 1]]
```

Description of the `output_lst` with examples:
- The first word in both `input_1` and `input_2` are `woke` and `wake` respectively. Their characters in position 0, 2, 3 are the same ("w", "k", "e") but the characters in position 1 are different ("o" vs "a"). The positional similarity and difference counts for this word should be `[3, 1]` which is first list (position 0) inside `output_lst`
- The third word in both `input_1` and `input_2` are `have` and `hour` respectively. Their characters in position 0 are the same ("h") and the characrters in positions 1,2,3 are different. The positional similarity and difference counts for this word should be `[1, 3]` which is the third list (position 2) inside `output_lst`


