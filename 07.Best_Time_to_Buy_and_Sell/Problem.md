# 121. Best Time to Buy and Sell Stock

## Difficulty

Easy

---

## Problem Statement

You are given an integer array `prices` where `prices[i]` is the price of a given stock on the `iᵗʰ` day.

You want to maximize your profit by choosing **one day to buy** one stock and **a different day in the future to sell** that stock.

Return the **maximum profit** you can achieve from this transaction.

If you cannot achieve any profit, return `0`.

---

## Example 1

### Input

```text
prices = [7,1,5,3,6,4]
```

### Output

```text
5
```

### Explanation

* Buy on Day 2 (Price = 1)
* Sell on Day 5 (Price = 6)

Profit = `6 - 1 = 5`

Buying after selling is not allowed.

---

## Example 2

### Input

```text
prices = [7,6,4,3,1]
```

### Output

```text
0
```

### Explanation

The stock price continuously decreases.

No profitable transaction can be made, so the maximum profit is `0`.

---

## Constraints

* `1 <= prices.length <= 10⁵`
* `0 <= prices[i] <= 10⁴`

---

## Key Observations

* You can buy only **once**.
* You can sell only **once**.
* Buying must happen **before** selling.
* Return `0` if no profit is possible.

---

## Approaches

### 1. Brute Force

* Try every possible buy day.
* For each buy day, check every future sell day.
* Calculate the profit.
* Keep track of the maximum profit.

**Time Complexity:** `O(n²)`

**Space Complexity:** `O(1)`

---

### 2. Optimal Approach (Running Minimum)

* Traverse the array once.
* Keep track of the **minimum stock price** seen so far.
* Calculate today's profit using the minimum price.
* Update the maximum profit whenever a better profit is found.

**Time Complexity:** `O(n)`

**Space Complexity:** `O(1)`

---

## Concepts Learned

* Arrays
* Running Minimum
* Greedy Technique
* Single Pass Traversal
* Time Complexity Optimization
* Space Optimization
* Maximum Profit Calculation

---

## Similar Problems

* 122. Best Time to Buy and Sell Stock II
* 123. Best Time to Buy and Sell Stock III
* 188. Best Time to Buy and Sell Stock IV
* 714. Best Time to Buy and Sell Stock with Transaction Fee
