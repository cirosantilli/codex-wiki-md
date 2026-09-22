<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Apply the [continued-fraction algorithm](../../../../../continued-fraction-algorithm.md). Since $3<\sqrt{11}<4$,

$$
x_0=\sqrt{11},\qquad a_0=3.
$$

The successive complete quotients are

$$
x_1=\frac1{\sqrt{11}-3}
=\frac{\sqrt{11}+3}{2},
\qquad a_1=3,
$$

and

$$
x_2=\frac1{x_1-3}
=\sqrt{11}+3,
\qquad a_2=6.
$$

Taking one more reciprocal returns to $x_1$, so the [continued fraction of the square root of eleven](../../../../../continued-fraction-of-the-square-root-of-eleven.md) is

$$
\boxed{\sqrt{11}=[3;\overline{3,6}].}
$$

Write

$$
z_n=p_n+q_n\sqrt{11}.
$$

The first convergents are $p_0/q_0=3$ and $p_1/q_1=10/3$, whence

$$
z_1=10+3\sqrt{11}
=\frac{3+\sqrt{11}}2(3+\sqrt{11})
=\frac{3+\sqrt{11}}2z_0.
$$

The [continued fraction convergent](../../../../../continued-fraction-convergent.md) recurrence is

$$
z_{n+1}=a_{n+1}z_n+z_{n-1},
$$

where $a_{n+1}=3$ for even $n$ and $a_{n+1}=6$ for odd $n$.

Set

$$
\alpha=3+\sqrt{11},
\qquad
\beta=\frac{3+\sqrt{11}}2.
$$

If $n$ is even and $z_{n+1}=\beta z_n$, then

$$
z_{n+2}=6z_{n+1}+z_n
=\left(6+\frac1\beta\right)z_{n+1}
=(3+\sqrt{11})z_{n+1}
=\alpha z_{n+1},
$$

because $\beta^{-1}=\sqrt{11}-3$. If $n$ is odd and $z_{n+1}=\alpha z_n$, then

$$
z_{n+2}=3z_{n+1}+z_n
=\left(3+\frac1\alpha\right)z_{n+1}
=\frac{3+\sqrt{11}}2z_{n+1}
=\beta z_{n+1},
$$

because $\alpha^{-1}=(\sqrt{11}-3)/2$. The base case and induction prove the [alternating multiplier recurrence for convergents of the square root of eleven](../../../../../alternating-multiplier-recurrence-for-convergents-of-the-square-root-of-eleven.md):

$$
\boxed{
p_{n+1}+q_{n+1}\sqrt{11}
=\begin{cases}
(3+\sqrt{11})(p_n+q_n\sqrt{11}),&n\text{ odd},\\[2mm]
\dfrac{3+\sqrt{11}}2(p_n+q_n\sqrt{11}),&n\text{ even}.
\end{cases}}
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
