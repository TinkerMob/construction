## Problem 问题

Given an array $a$ of length $n$, find a permutation of $a$ that for all $i$, $a_i \ne b_i$.

给定一个长度为$n$的数组$a$，找到这个数组的一个排列，使得变换之后的的数组与原数组每一位都不相同。

## Condition 条件

The permutation only exists if the number of the most frequent element is less or equal to half of $n$.

数组里出现次数最多的元素的个数必须小于等于所有元素个数的一半。

## Method 方法

Sort the array, we can find a permutation that maps each element at index $i$ to the element at $(\lfloor n / 2 \rfloor + i)~\text{mod}~n$.

将数组排序，然后可以在排序后的数组里找到一组映射关系，每个位置$i$的元素映射到位置$(\lfloor n / 2 \rfloor + i)~\text{mod}~n$。因为排序后每种元素的长度一定小于$\lfloor n / 2 \rfloor$，所以不会映射回自身。
