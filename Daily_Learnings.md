# LeetCode Daily Progress 🚀

---

## 📅 2026-07-16

### Problems Solved Today: 5

- LeetCode 2235 — Add Two Integers
- LeetCode 1480 — Running Sum of 1D Array
- LeetCode 1929 — Concatenation of Array
- LeetCode 2011 — Final Value of Variable After Performing Operations
- LeetCode 2114 — Maximum Number of Words Found in Sentences

### What I Learned Today

- Traversing arrays using loops.
- Traversing an array of strings.
- Traversing characters of a string using `charAt()`.
- Creating and returning values from functions.
- Passing parameters to methods.
- Performing basic arithmetic operations.
- Understanding and implementing Running Sum (Prefix Sum).
- Creating and working with new arrays.
- Using array indexing effectively.
- Comparing strings using `.equals()`.
- Using conditional statements (`if-else`).
- Incrementing and decrementing variables.
- Counting occurrences of a character.
- Converting spaces to words (`words = spaces + 1`).
- Finding the maximum value using comparison logic.
- Using nested loops to process strings and arrays.
- Improving problem-solving by breaking problems into smaller steps.

### Important Patterns

#### Running Sum Pattern

```java
// Add previous cumulative sum to current element
arr[i] = arr[i] + arr[i - 1];
```

#### Maximum Value Pattern

```java
// Update maximum value when a larger value is found
if(current > max)
{
    max = current;
}
```

#### String Comparison

```java
// Compare string contents
str.equals("text");
```

#### Character Access

```java
// Access character at index i
str.charAt(i);
```

### Day Summary

- Problems Solved: **5**
- Main Topics: **Arrays, Strings, Loops, Nested Loops, Prefix Sum**
- Difficulty: **Easy**
- Status: **Completed ✅**

---

# 🚀 LeetCode Daily Progress — 18 July 2026

## Problems Solved Today: 6

1. LeetCode 2114 — Maximum Number of Words Found in Sentences
2. LeetCode 2942 — Find Words Containing Character
3. LeetCode 412 — Fizz Buzz
4. LeetCode 2469 — Convert the Temperature
5. LeetCode 2652 — Sum Multiples
6. LeetCode 1528 — Shuffle String


# 📚 What I Learned Today (Overall)


## 🔹 Array Traversal

- Traversing arrays using loops.
- Accessing elements using index.
- Understanding array length.

Pattern:

```java
for(int i = 0; i < arr.length; i++)
{

}
```


---

# 🔹 String Traversal

Learned how to traverse characters inside a string.

Example:

```java
String s = "hello";

s.charAt(0); // h
```

Important:

```java
String length  → str.length()

Array length   → arr.length
```


Used in:
- LeetCode 2114
- LeetCode 2942


---

# 🔹 Nested Loop Pattern

Used when working with:

```
Array of Strings
        |
        ↓
Individual String
        |
        ↓
Each Character
```


Pattern:

```java
for(int i = 0; i < words.length; i++)
{
    for(int j = 0; j < words[i].length(); j++)
    {

    }
}
```


Used in:

- Finding characters inside words.
- Counting spaces.
- String searching.


---

# 🔹 String Comparison

Learned that Java strings should be compared using:

```java
.equals()
```

Wrong:

```java
str == "text"
```

Correct:

```java
str.equals("text")
```


---

# 🔹 Counting Pattern

## Counting spaces

LeetCode 2114:

Logic:

```
Words = Spaces + 1
```


Pattern:

```java
if(sentence.charAt(i) == ' ')
{
    count++;
}
```


---

# 🔹 Maximum Value Pattern

Used in LeetCode 2114.

Pattern:

```java
if(current > max)
{
    max = current;
}
```


Used to find:
- Maximum words
- Maximum values
- Best answer


---

# 🔹 List Usage

Learned how to create and use lists.

## String List

```java
List<String> ans = new ArrayList<>();
```

Adding:

```java
ans.add("Fizz");
```


## Integer List

```java
List<Integer> ans = new ArrayList<>();
```

Adding:

```java
ans.add(i);
```


Used in:

- LeetCode 2942
- LeetCode 412


---

# 🔹 String Conversion

## Integer → String

Learned:

```java
String.valueOf(number)
```


Example:

```java
String.valueOf(5);
```

Output:

```
"5"
```


Used in:

- LeetCode 412 Fizz Buzz


---

# 🔹 Character Array

Learned:

```java
char[] ans = new char[size];
```


Why?

Because Strings are immutable.

When changing/rearranging characters:

```
String
 ↓
char[]
 ↓
String
```


Conversion:

```java
new String(charArray)
```


Used in:

- LeetCode 1528 Shuffle String


---

# 🔹 Returning Different Data Types


## Integer

```java
return value;
```


## Array

```java
return ans;
```


## List

```java
return list;
```


## Double Array

```java
double[] ans = new double[2];

return ans;
```


---

# 🔹 Modulus Operator (%)


Used for divisibility checking.


Pattern:

```java
number % divisor == 0
```


Meaning:

```
Number is completely divisible by divisor
```


Examples:

```java
i % 3 == 0

i % 5 == 0

i % 7 == 0
```


Used in:

- LeetCode 412
- LeetCode 2652


---

# 🔹 FizzBuzz Pattern (LeetCode 412)


Condition order is important:


```
Check 3 and 5 first

Then check 3

Then check 5

Else number
```


Because:

```
15 is divisible by 3 and 5
```

Output:

```
FizzBuzz
```


---

# 🔹 Temperature Conversion (LeetCode 2469)


Learned:

- Using double data type.
- Returning double arrays.
- Storing multiple answers.


Pattern:

```java
double[] ans = new double[2];

ans[0] = value1;
ans[1] = value2;

return ans;
```


---

# 🔹 Index Mapping Pattern (LeetCode 1528)


Most important learning today.


Problem:

```
Move characters according to given indexes
```


Example:

```
s = "abc"

indices = [2,1,0]
```


Mapping:

```
a → index 2
b → index 1
c → index 0
```


Pattern:

```java
ans[indices[i]] = s.charAt(i);
```


Meaning:

```
Current character
        |
        ↓
New position
```


---

# ❌ Mistakes I Made Today


## Java Syntax Mistakes

### String comparison

Wrong:

```java
str == "abc"
```

Correct:

```java
str.equals("abc")
```


---

### Array vs String length

Array:

```java
arr.length
```

String:

```java
str.length()
```


---

### char vs char[]

char:

```
single character
```

Example:

```java
char ch = 'a';
```


char array:

```
multiple characters
```

Example:

```java
char[] ch;
```


---

### Wrong array creation

Wrong:

```java
char arr[size];
```

Correct:

```java
char[] arr = new char[size];
```


---

### Returning wrong type

Example:

Method:

```java
public String function()
```

Cannot return:

```java
char[]
```

Need:

```java
new String(charArray)
```


---

# 🧠 Biggest Learning Today


The logic of the problem is usually simple.

The main challenge is:

- Choosing correct data structure.
- Remembering Java syntax.
- Understanding return type.
- Converting logic into code.
- Thinking with indexes and positions.


---

# ⭐ Important Patterns To Revise


## Character Access

```java
str.charAt(i)
```


## String Comparison

```java
str.equals("text")
```


## Convert Integer to String

```java
String.valueOf(i)
```


## Character Array to String

```java
new String(charArray)
```


## Index Mapping

```java
result[newIndex] = value;
```


## Maximum Pattern

```java
if(current > max)
{
    max = current;
}
```


---

# 📊 Daily Summary

Problems Solved: **6**

Topics:

- Arrays
- Strings
- Character Arrays
- ArrayList
- Nested Loops
- String Methods
- Modulus Operator
- Conditions
- Type Conversion
- Index Mapping
- Returning Arrays


## Progress 🚀

Today I improved my ability to convert problem logic into Java code and learned how small syntax details affect the final solution.

# 📅 Day 3 — Understanding Mapping, Counting, and Digit Processing

## Problems Solved Today

- LeetCode 1920 — Build Array from Permutation
- LeetCode 1365 — How Many Numbers Are Smaller Than the Current Number
- LeetCode 1295 — Find Numbers with Even Number of Digits

---

# 🧠 Overall Learning From Today

Today was different from previous days.

Earlier, most of my mistakes were syntax-related:

- length vs length()
- char vs char[]
- Returning wrong data types
- Creating arrays incorrectly

Today, I started facing more logic-oriented problems.

The biggest lesson was:

> Understanding what exactly needs to be counted, mapped, or processed before writing code.

---

# 🚀 LeetCode 1920 — Build Array from Permutation

## My First Thought

I understood that a new array needed to be created.

But I struggled with array creation syntax.

## Mistakes I Made

### Incorrect Array Creation

Wrong:

```java
int ans[] = new ans;
```

Learned:

```java
int[] ans = new int[nums.length];
```

### Loop Boundary Confusion

Initially:

```java
for(int i = 1; i <= nums.length; i++)
```

Learned:

Arrays are 0-indexed.

Correct:

```java
for(int i = 0; i < nums.length; i++)
```

### Assignment Without Index

Wrong:

```java
ans[] = nums[i];
```

Learned:

```java
ans[i] = value;
```

Every array assignment needs an index.

## Biggest Concept Learned

### Index Mapping

```java
ans[i] = nums[nums[i]];
```

This was my second major mapping problem after Shuffle String.

I learned:

> One index can lead to another index.

Example:

```text
nums[1] = 2

ans[1] = nums[2]
```

## Pattern Learned

```java
ans[i] = nums[nums[i]];
```

## Thinking Improvement

Before:

> Copy values directly.

After:

> Use indexes to locate another position.

---

# 🚀 LeetCode 1365 — How Many Numbers Are Smaller Than the Current Number

## My First Thought

For every number:

Compare it with every other number.

If another number is smaller:

Increase the count.

## Mistakes I Made

### Loop Boundary Mistake

Initially:

```java
i <= nums.length
```

Learned:

```java
i < nums.length
```

### Incrementing Whole Array

Wrong:

```java
count++;
```

Learned:

```java
count[i]++;
```

because count is an array.

## Biggest Concept Learned

### Counting Pattern

I learned that:

```java
count[i]
```

stores the answer for:

```java
nums[i]
```

Every position in the answer array can represent the answer for the corresponding input position.

## Pattern Learned

```java
for(int i = 0; i < nums.length; i++)
{
    for(int j = 0; j < nums.length; j++)
    {
        if(nums[i] > nums[j])
        {
            count[i]++;
        }
    }
}
```

## Runtime

```text
7 ms
Beats 82.27%
```

This showed me that a simple brute-force solution can still perform quite well.

## Thinking Improvement

Before:

> I knew how to compare numbers.

After:

> I understood where the result should be stored.

---

# 🚀 LeetCode 1295 — Find Numbers With Even Number of Digits

## My First Thought

I knew division by 10 was related to digits.

But I struggled to convert that idea into code.

## Mistakes I Made

### Treated Array As A Number

Wrong:

```java
while(nums != 0)
```

I forgot that nums is an array.

### Tried Dividing Entire Array

Wrong:

```java
nums /= 10;
```

Arrays cannot be divided.

Learned:

```java
int num = nums[i];
```

Process the element, not the entire array.

### Checked Wrong Thing

Wrong:

```java
if(nums[i] % 2 == 0)
```

I was checking whether the number was even.

The problem asks whether the number of digits is even.

### Counter Scope Mistake

Initially:

```java
int digits = 0;
```

was outside the loop.

So digit counts from previous numbers continued accumulating.

Learned:

```java
for(...)
{
    int digits = 0;
}
```

Each number needs its own digit counter.

## Biggest Concept Learned

### Digit Counting Pattern

```java
while(num != 0)
{
    num /= 10;
    digits++;
}
```

Every division removes one digit.

## Pattern Learned

```java
for(each number)
{
    digits = 0;

    while(number != 0)
    {
        number /= 10;
        digits++;
    }
}
```

## Thinking Improvement

Before:

> I was trying to process the entire array.

After:

> First select one element. Then process that element.

---

# 🐛 Mistake Database Added Today

## Arrays vs Elements

Wrong Thinking:

```java
nums
```

Correct Thinking:

```java
nums[i]
```

Always ask:

> Am I working with the entire array or one element?

## Array Counter vs Integer Counter

Wrong:

```java
count++;
```

Correct:

```java
count[i]++;
```

when count is an array.

## Variable Scope

Wrong:

```java
int digits = 0;
```

outside processing loop.

Correct:

Reset counters for every new element when required.

---

# 🔥 New Patterns Learned Today

## Mapping Pattern

```java
ans[i] = nums[nums[i]];
```

## Counting Pattern

```java
count[i]++;
```

## Digit Counting Pattern

```java
while(num != 0)
{
    num /= 10;
    digits++;
}
```

## Nested Comparison Pattern

```java
for(int i = 0; i < n; i++)
{
    for(int j = 0; j < n; j++)
    {
        if(nums[i] > nums[j])
        {
            count[i]++;
        }
    }
}
```

---

# 📈 Progress After Day 3

## Problems Solved So Far

- LeetCode 2235
- LeetCode 1480
- LeetCode 1929
- LeetCode 2011
- LeetCode 2114
- LeetCode 2942
- LeetCode 412
- LeetCode 2469
- LeetCode 2652
- LeetCode 1528
- LeetCode 1920
- LeetCode 1365
- LeetCode 1295

**Total Solved: 13 Problems**

---

# 🌟 Biggest Realization Today

Earlier, I thought my biggest weakness was syntax.

Now I realize that many mistakes come from understanding:

- What exactly should be counted.
- What exactly should be stored.
- Whether I am working on an array or a single element.
- Where variables should be reset.

These are problem-solving skills that improve only through practice.

Every problem is making my thinking more structured.

I am no longer just writing code.

I am learning how to think like a programmer. 🚀
