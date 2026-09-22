<h1 id="22g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) makes the family of iterates relatively compact in $C([0,T_1])$. The standard successive-approximation proof for this scalar autonomous equation shows that, after decreasing to some $T_2\leq T_1$, the adjacent differences

$$
R_n=f_{n+1}-f_n
$$

tend uniformly to zero. One way to finish the existence argument without requiring a Lipschitz hypothesis on $\phi$ is the following direct scalar construction.

If $\phi(0)=0$, the function $f(t)=0$ is already a solution. If $\phi(0)\ne0$, continuity gives an interval $[-A_0,A_0]$ on which $\phi$ has constant sign and never vanishes. Define

$$
F(x)=\int_0^x\frac{du}{\phi(u)}.
$$

Then $F$ is continuously differentiable with $F'(0)\ne0$. By the [inverse function theorem](../../../../../../inverse-function-theorem.md), it has a continuously differentiable local inverse on $[0,T_2]$ after choosing $T_2>0$ small enough and choosing the appropriate one-sided range. Put

$$
f(t)=F^{-1}(t).
$$

The chain rule gives

$$
F'(f(t))f'(t)=1,
$$

and hence

$$
\boxed{f(0)=0,\qquad f'(t)=\phi(f(t))}.
$$

Equivalently, $f(t)=\int_0^t\phi(f(s))\,ds$, the fixed-point equation approximated by the iterates. This is the [local existence for a scalar autonomous ordinary differential equation with continuous vector field](../../../../../../local-existence-for-a-scalar-autonomous-ordinary-differential-equation-with-continuous-vector-field.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [22G](../../22g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
