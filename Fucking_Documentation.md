# 🚀 My LeetCode Journey — From Confusion to Confidence

## Introduction

When I started solving LeetCode problems, I thought the biggest challenge would be finding the solution.

But slowly I realized something:

> The hardest part was not finding the answer. The hardest part was training my brain to break problems into smaller logical steps and convert those thoughts into code.

I already knew programming concepts, but implementing those concepts correctly was a completely different skill.

Understanding a concept and writing a working solution are two different things.


---

# 📅 Journey Timeline


| Day | Problems Solved | Main Concepts Learned |
|-----|----------------|----------------------|
| Day 1 | 5 Problems | Arrays, Loops, Prefix Sum, Conditions |
| Day 2 | 6 Problems | Strings, ArrayList, Nested Loops, Mapping |


*(Future days will be added here)*


---

# 📅 Day 1 — Building The Foundation


## Problems Solved

- LeetCode 2235 — Add Two Integers
- LeetCode 1480 — Running Sum of 1D Array
- LeetCode 1929 — Concatenation of Array
- LeetCode 2011 — Final Value of Variable After Performing Operations
- LeetCode 2114 — Maximum Number of Words Found in Sentences


---

# 🧠 Day 1 Learning


## 1. Function Understanding

Learned how LeetCode functions work.

Example:

```java
public int functionName(parameters)
{

}
```

Important things:

- Understanding parameters.
- Understanding return type.
- Returning correct values.


---

## 2. Array Traversal

Learned how to visit every element of an array.


Pattern:

```java
for(int i = 0; i < arr.length; i++)
{

}
```


Learning:

- Accessing values using indexes.
- Understanding positions.
- Processing each element.


---

## 3. Creating New Arrays


Pattern:

```java
int[] ans = new int[size];
```


Learning:

```
Create Array
      ↓
Store Values
      ↓
Return Answer
```


---

## 4. Running Sum Pattern


Problem:

LeetCode 1480 — Running Sum of 1D Array


Important pattern:

```java
arr[i] = arr[i] + arr[i-1];
```


Learning:

Current answer can depend on previous values.


---

## 5. Array Concatenation


Problem:

LeetCode 1929 — Concatenation of Array


Learned:

- Creating larger arrays.
- Copying values using indexes.


Example:

```
Input:

[1,2,3]


Output:

[1,2,3,1,2,3]
```


---

## 6. Conditions & Variables


Problem:

LeetCode 2011


Learned:

- if-else conditions.
- Incrementing variables.
- Decrementing variables.


---

## 7. Maximum Value Pattern


Problem:

LeetCode 2114


Important pattern:


```java
if(current > max)
{
    max = current;
}
```


Used in:

- Maximum value problems.
- Best answer tracking.
- Comparison problems.


---

# 📅 Day 2 — Strings, Lists & Index Mapping


## Problems Solved

- LeetCode 2114 — Maximum Number of Words Found in Sentences
- LeetCode 2942 — Find Words Containing Character
- LeetCode 412 — Fizz Buzz
- LeetCode 2469 — Convert the Temperature
- LeetCode 2652 — Sum Multiples
- LeetCode 1528 — Shuffle String


---

# 🧠 Day 2 Learning


## 1. String Traversal


Learned that a String contains:

- Characters
- Positions
- Indexes


Example:

```java
String s = "hello";

s.charAt(0);
```


Output:

```
h
```


Learned:

- Traversing characters.
- Counting characters.
- Searching inside strings.


---

# 2. Nested Loop Thinking


Many string problems follow:


```
Array of Strings

        ↓

Individual String

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


Used for:

- Searching characters.
- Comparing characters.
- Processing strings.


---

# 3. ArrayList


Learned dynamic storage.


Creating:

```java
List<Integer> ans = new ArrayList<>();
```


Adding:

```java
ans.add(i);
```


Used in:

LeetCode 2942


---

# 4. FizzBuzz Logic


Problem:

LeetCode 412


Important:

Condition order matters.


Correct thinking:


```
Check divisible by 3 and 5

↓

Check divisible by 3

↓

Check divisible by 5

↓

Else return number
```


Learned:

```java
String.valueOf(number);
```


Converts:

```
int → String
```


---

# 5. Returning Multiple Values


Problem:

LeetCode 2469


Learned:

Returning arrays.


Pattern:


```java
double[] ans = new double[2];

ans[0] = value1;
ans[1] = value2;

return ans;
```


---

# 6. Modulus Pattern


Used in:

- FizzBuzz
- Sum Multiples


Pattern:


```java
number % divisor == 0
```


Meaning:

Number is completely divisible.


---

# 7. Index Mapping


Problem:

LeetCode 1528 — Shuffle String


Biggest learning of Day 2.


Example:

```
s = "abc"

indices = [2,1,0]
```


Meaning:


```
a → index 2
b → index 1
c → index 0
```


Final pattern:


```java
answer[indices[i]] = s.charAt(i);
```


Learning:


```
Old Position → New Position
```


---

# 🐛 My Mistake Database


## Java Syntax Mistakes


---

## 1. length vs length()


Array:

```java
arr.length
```


String:

```java
str.length()
```


---

## 2. String Comparison


Wrong:


```java
str == "text"
```


Correct:


```java
str.equals("text")
```


---

## 3. char vs char[]


Single character:


```java
char ch = 'a';
```


Multiple characters:


```java
char[] ch;
```


---

## 4. Array Creation


Wrong:


```java
char arr[size];
```


Correct:


```java
char[] arr = new char[size];
```


---

## 5. Returning Wrong Data Type


If function requires:


```java
String
```


Cannot return:


```java
char[]
```


Convert using:


```java
new String(charArray)
```


---

## 6. Creating String Too Early


Wrong:


```
Create String

↓

Fill Array
```


Correct:


```
Fill Character Array

↓

Convert Into String
```


---

# 🔥 Pattern Library


## Array Traversal

```java
for(int i = 0; i < arr.length; i++)
{

}
```


---

## Character Access

```java
str.charAt(i)
```


---

## String Conversion

```java
String.valueOf(number)
```


---

## Character Array To String

```java
new String(charArray)
```


---

## Maximum Pattern

```java
if(current > max)
{
    max = current;
}
```


---

## Index Mapping

```java
result[newPosition] = value;
```


---

# 📚 My Learning System


For every problem:


```
1. Understand the problem statement.

2. Identify input and output.

3. Think about the brute-force approach.

4. Write logic in simple words.

5. Convert logic into code.

6. Debug mistakes.

7. Write what I learned.

8. Save reusable patterns.
```


---

# 📅 Future Day Template


## Day X — Problem Solving


### Problems Solved

- LeetCode XXXX — Problem Name


---

### My First Thought

What I understood initially.


---

### My Approach

Step-by-step thinking.


---

### Mistakes I Made

- Syntax mistakes.
- Logic mistakes.
- Wrong approach.


---

### What I Learned


Concepts and patterns learned.


---

### Pattern To Remember


```java

Reusable code pattern

```


---

### My Improvement

Before:

"I was confused about..."


After:

"Now I understand..."


---

# 📈 Progress After 2 Days


Problems Solved:

```
10 Problems
```


Concepts Learned:

- Arrays
- Strings
- Loops
- Nested Loops
- ArrayList
- Character Arrays
- Type Conversion
- Index Mapping
- Return Types
- Modulus Operator
- Prefix Sum


---

# Advice For Beginners


## 1. Do Not Rush To Hard Problems

Easy problems build strong foundations.


---

## 2. Maintain A Mistake Log

Your mistakes become your personal roadmap.


---

## 3. Understand Before Coding


Always ask:


```
What is the input?

What is the output?

What data structure should I use?

What pattern does this problem follow?
```


---

## 4. Do Not Compare Speed


Someone solving faster does not mean they are learning better.


Focus on improvement.


---

# Final Message


I started with confusion.

I struggled with syntax.

I struggled with indexes.

I struggled with converting ideas into code.


But every mistake added one small piece of understanding.


The goal is not only solving thousands of problems.

The goal is becoming a better problem solver every day.


One problem at a time. 🚀
