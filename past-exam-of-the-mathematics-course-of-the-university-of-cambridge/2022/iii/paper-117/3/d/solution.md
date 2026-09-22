<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the fourth moment from part c, put

$$
s_1=r_1-r_2,\quad s_2=r_1+r_2,\qquad
u_1=t_1-t_2,\quad u_2=t_1+t_2.
$$

Then the phase is $e(\alpha s_1s_2u_1u_2)$. The contribution with $s_1=0$ is $O(RT^2)$, because $r_1=r_2$; the contribution with $u_1=0$ is $O(TR^2)$. Their fourth roots are respectively $R^{1/4}T^{1/2}$ and $R^{1/2}T^{1/4}$.

Off the diagonals, fix $s_2,u_1,u_2$. The variable $s_1$ ranges over an interval of length $O(R)$, subject only to harmless parity and range restrictions. The [exponential geometric sum bound](../../../../../../exponential-geometric-sum-bound.md) gives

$$
\left|\sum_{s_1\in I}e(\alpha s_1s_2u_1u_2)\right|
\ll\min(R,\|\alpha s_2u_1u_2\|^{-1}).
$$

Put $m=|s_2u_1u_2|$. We have $m\leq CRT^2$, and the number of representations of a fixed $m$ by the three factors, including signs and range restrictions, is $O(\tau_4(m))$. Hence the fourth moment is

$$
\ll RT^2+TR^2+\sum_{m\leq CRT^2}\tau_4(m)\min(R,\|\alpha m\|^{-1}).
$$

Using $(A+B+C)^{1/4}\leq A^{1/4}+B^{1/4}+C^{1/4}$ in part c proves

$$
|S|\ll\|b\|_2\|c\|_2\left(
R^{1/4}T^{1/2}+R^{1/2}T^{1/4}
+\left(\sum_{m\leq CRT^2}\tau_4(m)\min(R,\|\alpha m\|^{-1})\right)^{1/4}
\right).
$$

This is the [factorized fourth moment for a bilinear quadratic exponential sum](../../../../../../factorized-fourth-moment-for-a-bilinear-quadratic-exponential-sum.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
