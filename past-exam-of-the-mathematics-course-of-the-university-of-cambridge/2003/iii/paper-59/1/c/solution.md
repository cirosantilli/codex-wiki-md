<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The cubic [Taylor expansion](../../../../../../taylor-expansion.md) at the double-zero point is

$$
\begin{aligned}
\dot q&=2q-2p-\frac43q^3+2p^2q+pq^2+\frac43p^3+O(5),\\
\dot p&=2q-2p-\frac13q^3-2p^2q+\frac43p^3+O(5).
\end{aligned}
$$

There are no quadratic or quartic terms because the local [vector field](../../../../../../vector-field.md) is odd under $(q,p)\mapsto(-q,-p)$. Set $u=p$, $v=q-p$, and use $\tau=2t$. The [linear transformation](../../../../../../linear-map.md) is invertible, and the positive time rescaling preserves orbit orientation. With primes denoting $d/d\tau$, the result is

$$
\begin{aligned}
u'&=v-\frac12u^3-\frac32u^2v-\frac12uv^2-\frac16v^3+O(5),\\
v'&=2u^3+\frac32u^2v-uv^2-\frac12v^3+O(5).
\end{aligned}
$$

This supplies the requested cubic functions, with a remainder stronger than $O(4)$.

There is an important [normal form](../../../../../../normal-form-dynamical-systems.md) check. Setting $x=u$, $y=u'$ straightens the first equation, and differentiating gives

$$
x'=y,\qquad y'=2x^3-4xy^2-y^3+O(5).
$$

In particular the [nilpotent cubic damping invariant](../../../../../../nilpotent-cubic-damping-invariant.md) is $g_{21}+3f_{30}=3/2-3/2=0$. A nonsingular cubic [near-identity transformation](../../../../../../near-identity-transformation.md) and rescaling cannot change this vanishing invariant into the nonzero $-x^2y$ coefficient in the supplied later [normal form](../../../../../../normal-form-dynamical-systems.md). The conclusions for that assumed system are therefore given separately from the independently derived conclusions for the printed original equations.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
