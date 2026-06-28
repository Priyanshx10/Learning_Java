# 27. Remove Element

## Difficulty

Easy

---

## Problem Statement

Given an integer array `nums` and an integer `val`, remove all occurrences of `val` in-place.

The order of the elements may be changed.

Return the number of elements in `nums` which are **not equal** to `val`.

The first `k` elements of `nums` should contain the elements that are not equal to `val`.

---

## Example 1

### Input

```text
nums = [3,2,2,3]
val = 3
```

### Output

```text
2
```

### Modified Array

```text
[2,2,_,_]
```

---

## Example 2

### Input

```text
nums = [0,1,2,2,3,0,4,2]
val = 2
```

### Output

```text
5
```

### Modified Array

```text
[0,1,4,0,3,_,_,_]
```

---

## Constraints

- 0 <= nums.length <= 100
- 0 <= nums[i] <= 50
- 0 <= val <= 100

---

## Key Observation

- Do not create a new array.
- Modify the existing array (`nums`) in-place.
- Return the number of valid elements (`k`).
