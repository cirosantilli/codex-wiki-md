<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Set

$$
Z=\binom{u}{u_t},
\qquad
Z_0=\binom{u_0}{u_1},
\qquad
F(t)=\binom0{f(t,\cdot)}.
$$

Then the forced equation is the [abstract Cauchy problem](../../../../../../abstract-cauchy-problem.md)

$$
\dot Z=AZ+F,
\qquad
Z(0)=Z_0.
$$

For $Z_0\in\mathcal H$ and $F\in C([0,T];\mathcal H)$, a [mild solution of an abstract Cauchy problem](../../../../../../mild-solution-of-an-abstract-cauchy-problem.md) is a function $Z\in C([0,T];\mathcal H)$ satisfying the [variation-of-constants formula](../../../../../../variation-of-constants-formula.md)

$$
\boxed{
Z(t)=U(t)Z_0+int_0^tU(t-s)F(s)\,ds}.
$$

Suppose $F(s)\in D(A)$ and both $F$ and $AF$ are continuous. If also $Z_0\in D(A)$, then the closedness of $A$ permits differentiation under the [Bochner integral](../../../../../../bochner-integral.md):

$$
\frac d{dt}\int_0^tU(t-s)F(s)\,ds
=F(t)+\int_0^tU(t-s)AF(s)\,ds.
$$

Thus $Z\in C^1([0,\infty);\mathcal H)$ and $Z'=AZ+F$. The assumption $Z_0\in D(A)$ is necessary here: a unitary group has no smoothing, so the conditions on $F$ alone cannot make $U(t)Z_0$ differentiable for arbitrary $Z_0\in\mathcal H$.

For the resulting strong solution, skew symmetry of $A$ gives the [energy estimate](../../../../../../energy-estimate.md)

$$
\frac d{dt}\|Z(t)\|_{\mathcal H}^2
=2\operatorname{Re}(Z(t),F(t))_{\mathcal H}.
$$

Integration yields

$$
\boxed{
\|Z(t)\|_{\mathcal H}^2
\leq\|Z(0)\|_{\mathcal H}^2
+2\int_0^t|(Z(s),F(s))_{\mathcal H}|\,ds}.
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
