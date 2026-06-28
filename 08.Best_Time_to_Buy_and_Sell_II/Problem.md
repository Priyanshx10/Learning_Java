# 122. Best Time to Buy and Sell Stock II

## Difficulty

Medium

---

## Problem Statement

You are given an integer array `prices` where `prices[i]` is the price of a given stock on the `iᵗʰ` day.

On each day, you may decide to buy and/or sell the stock.

You can hold **at most one share** of the stock at any time.

You are allowed to buy and sell the stock multiple times.

Return the **maximum profit** you can achieve.

---

## Example 1

### Input

```text
prices = [7,1,5,3,6,4]
```

### Output

```text
7
```

### Explanation

Buy at price **1** and sell at **5** → Profit = **4**

Buy at price **3** and sell at **6** → Profit = **3**

Total Profit = **7**

---

## Example 2

### Input

```text
prices = [1,2,3,4,5]
```

### Output

```text
4
```

### Explanation

Buy at **1** and sell at **5**

Profit = **4**

The greedy solution also produces the same result by adding every positive increase.

---

## Example 3

### Input

```text
prices = [7,6,4,3,1]
```

### Output

```text
0
```

### Explanation

Prices continuously decrease.

No profitable transaction can be made.

---

## Constraints

* `1 <= prices.length <= 3 × 10⁴`
* `0 <= prices[i] <= 10⁴`

---

## Key Observations

* Multiple transactions are allowed.
* You cannot hold more than one stock at a time.
* Add every positive price difference.
* Ignore decreasing prices.

---

## Approach

### Greedy

Traverse the array once.

Whenever today's price is greater than yesterday's price, add the difference to the total profit.

This captures every profitable transaction while achieving the maximum possible profit.

---

## Complexity

### Time Complexity

```text
O(n)
```

### Space Complexity

```text
O(1)
```

---

## Concepts Learned

* Arrays
* Greedy Algorithm
* Single Pass Traversal
* Profit Maximization
* Time Optimization

---

## Similar Problems

* 121. Best Time to Buy and Sell Stock
* 123. Best Time to Buy and Sell Stock III
* 188. Best Time to Buy and Sell Stock IV
* 714. Best Time to Buy and Sell Stock with Transaction Fee
