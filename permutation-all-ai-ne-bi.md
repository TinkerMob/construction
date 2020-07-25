## Problem

Given an array $a$ of length $n$, find a permutation of $a$ that for all $i$, $a_i \ne b_i$.

## Condition

The permutation only exists if the number of the most frequent element is less or equal to half of $n$.

## Method

Sort the array, we can find a permutation that maps each element at index $i$ to the element at $(n / 2 + i) \text{mod} n$.
