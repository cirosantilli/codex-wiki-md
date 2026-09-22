<h1 id="7c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $F_n=x_n$. For $n\geq1$, the recurrence and the previously proved [greatest common divisor](../../../../../../greatest-common-divisor.md) invariance give

$$
\gcd(F_{n+1},F_n)=\gcd(F_n+F_{n-1},F_n)=\gcd(F_{n-1},F_n).
$$

Repeating reaches $\gcd(F_1,F_0)=\gcd(1,0)=1$. This also gives the $n=0$ case directly. Applying the same invariance once more,

$$
\gcd(F_{n+2},F_n)=\gcd(F_{n+1}+F_n,F_n)=\gcd(F_{n+1},F_n)=1.
$$

Thus **both requested greatest common divisors equal one for every $n\geq0$**. This is the adjacent-index instance of [Fibonacci gcd reduction](../../../../../../fibonacci-gcd-reduction.md), derived directly rather than assuming the stronger general formula.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [7C](../../7c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
