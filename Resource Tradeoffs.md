You can calculate the number of resources used as a function of space and time. The amount of space used to solve a problem and the amount of time it takes to solve it in that space. Also, in the real world, there is the added constraint of money.

> A resource tradeoff is when you increase the usage of time, space, or money to improve the efficiency of another.

### Example: Sock Matching

Let's say you have 20 socks (n=20) that you want to match in a pile of laundry. You need to assume that you will get lucky and pick the matching sock the first time and you will get unlucky and have to go through each remaining sock until you find the match so 18 socks.

To calculate the maximum number of socks you need to touch to match all the socks, sum the averages of the lucky and unlucky numbers.

1st match `n=20`
```latex
(n + 2) / 2 = 11
```

2nd match `n=18`
```latex
(n + 2) / 2 = 10
```

3rd match `n=16`
```latex
(n + 2) / 2 = 9
```

... nth match 

We have to sum all of these averages and we can do it using the Gaussian trick for summing many numbers. 

```latex
11 + 2 = 13
10 + 3 = 13
9  + 4 = 13
...
```
In this case, there are 5 combinations of these sums of 13. we can get that by finding how many numbers are in the range that we are using.

```latex
(highest - lowest + 1) / 2

11 - 2 + 1 = 10
10/2 = 5
```

## Caching

**Caching** is a general problem-solving approach that provides a much more flexible way of dealing with certain resource tradeoffs.

In the example of a music app on your phone, caching can help reduce the network usage on your data plan at the cost of using more space on your phone. The developers of the app need to decide on the right balance of network and storage utilization to have the best user experience.