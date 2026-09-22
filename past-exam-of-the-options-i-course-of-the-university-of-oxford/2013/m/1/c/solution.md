<h1 id="m/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $I_2=T_2-T_1$ and $I_3=T_3-T_2$ be the interarrival times adjacent to the second arrival. They are independent [exponential random variables](../../../../../exponential-distribution.md) of rate twelve per hour. The second customer meets the first if $I_2<1/12$ hour, and meets a later customer if $I_3<1/12$ hour. If the third arrives too late, every subsequent customer does also. Thus the only way to meet nobody is for both gaps to be at least five minutes:

$$
\mathbb P(\text{no meeting})=\mathbb P(I_2\geq1/12)\mathbb P(I_3\geq1/12)=e^{-1}e^{-1}=e^{-2}.
$$

Hence $\boxed{\mathbb P(\text{meeting})=1-e^{-2}}$. Exact equality of arrival and departure times has [probability](../../../../../probability.md) zero. The calculation includes both customers already present and customers arriving during the visit; it is a [two-sided interarrival test for overlap](../../../../../two-sided-interarrival-test-for-overlap.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [M](../../../m.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
