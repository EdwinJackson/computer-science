# Best Time to Buy and Sell Stock
Difficulty: **Easy**

Requirements:
- You are given an array `prices` where `prices[i]` is the price of a given stock on the `i`th day.
- You want to maximize your profit by choosing a single day to buy one stock and choosing a different day in the future to sell that stock.
- Return the maximum profit you can achieve from this transaction.
- If you cannot achieve any profit, return 0.

Test cases:
```js
maxProfit([7, 1, 5, 3, 6, 4]) // returns 5 (Buy on day 2 (price 1) and sell on day 5 (price 6))
maxProfit([7, 6, 4, 3, 1]) // returns 0 (No transactions are profitable)
maxProfit([1, 2]) // returns 1
maxProfit([2, 4, 1]) // returns 2
```

JavaScript Solution

```js
/**
 * @param {number[]} prices
 * @return {number}
 */
var maxProfit = function(prices) {
    if (!prices || prices.length < 2) {
        return 0;
    }

    let minPrice = prices[0];
    let maxProfit = 0;

    for (let i = 1; i < prices.length; i++) {
        const currentPrice = prices[i];
        const potentialProfit = currentPrice - minPrice;

        // Update maxProfit if current potential profit is higher
        maxProfit = Math.max(maxProfit, potentialProfit);

        // Update minPrice if we find a lower price to buy
        minPrice = Math.min(minPrice, currentPrice);
    }

    return maxProfit;
};
```

## Related To
- [[data structures/Arrays]]
- [[Greediness]]
