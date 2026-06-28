# 189. Rotate Array

## Difficulty

Medium

---

## Problem Statement

Given an integer array `nums`, rotate the array to the right by `k` steps, where `k` is non-negative.

Modify the array in-place.

---

## Example 1

### Input

```text
nums = [1,2,3,4,5,6,7]
k = 3
```

### Output

```text
[5,6,7,1,2,3,4]
```

### Explanation

Rotate once

```text
[7,1,2,3,4,5,6]
```

Rotate twice

```text
[6,7,1,2,3,4,5]
```

Rotate three times

```text
[5,6,7,1,2,3,4]
```

---

## Example 2

### Input

```text
nums = [-1,-100,3,99]
k = 2
```

### Output

```text
[3,99,-1,-100]
```

---

## Constraints

* `1 <= nums.length <= 10⁵`
* `-2³¹ <= nums[i] <= 2³¹ - 1`
* `0 <= k <= 10⁵`

---

## Follow-up

Can you solve the problem

* in **O(n)** time?
* using **O(1)** extra space?
