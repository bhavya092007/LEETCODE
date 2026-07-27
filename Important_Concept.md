### Key Concept

This pattern is commonly used to find the **maximum element** in an array or collection.

```java
if(current > max)
{
    max = current;
}

Frequency Array Rule:

freq[s.charAt(i) - 'a']++

means

"Increase the count of the current character."

# Enhanced For Loop vs Normal For Loop in Java

## Enhanced For Loop (For-Each Loop)

```java
for(int num : nums) {
    // code
}
```

### Meaning

- `nums` = array
- `num` = current element of the array

The loop automatically takes each value from `nums` one by one.

Example:

```java
int[] nums = {10, 20, 30};

for(int num : nums) {
    System.out.println(num);
}
```

Output:

```text
10
20
30
```

---

## Expanded Version

The above loop is equivalent to:

```java
for(int i = 0; i < nums.length; i++) {
    int num = nums[i];

    // same code
}
```

### Breakdown

```java
int i = 0;
```

Start from index 0.

```java
i < nums.length;
```

Continue until the last index.

```java
i++;
```

Move to the next index.

```java
int num = nums[i];
```

Store the current element in `num`.

---

## Example

```java
int[] nums = {10, 20, 30};

for(int i = 0; i < nums.length; i++) {
    int num = nums[i];
    System.out.println(num);
}
```

Output:

```text
10
20
30
```

---

## When to Use Each

### Use Enhanced For Loop

```java
for(int num : nums)
```

When you only need the value.

Examples:
- Sum of array
- Finding duplicates
- Finding maximum value

### Use Normal For Loop

```java
for(int i = 0; i < nums.length; i++)
```

When you need the index.

Examples:
- Two Sum
- Contains Duplicate II
- Accessing neighboring elements
- Updating array values by index

---

## Memory Trick

```text
for(int num : nums)
```

Read as:

"For every number num in nums"

```text
for(int i = 0; i < nums.length; i++)
```

Read as:

"For every index i in nums"
```
