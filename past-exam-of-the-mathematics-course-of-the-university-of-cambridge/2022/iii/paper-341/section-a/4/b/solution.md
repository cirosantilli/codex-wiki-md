<h1 id="section-a/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose the [Sobolev space](../../../../../../../sobolev-space-split.md) $V$ encoding the homogeneous essential [boundary conditions](../../../../../../../boundary-condition.md), set

$$
a(u,v)=\langle\mathcal Lu,v\rangle,
\qquad \ell(v)=\langle f,v\rangle,
$$

after the appropriate [integration by parts](../../../../../../../integration-by-parts.md), and define the [energy functional](../../../../../../../energy-functional.md)

$$
J(v)=\frac12a(v,v)-\ell(v).
$$

Its first variation is $J'(u)v=a(u,v)-\ell(v)$, so its stationary points are exactly the solutions of the [weak formulation](../../../../../../../weak-formulation.md)

$$
a(u,v)=\ell(v)\qquad(v\in V).
$$

If $a$ is bounded, symmetric, and coercive and $\ell\in V'$, the [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md) supplies a unique [weak solution](../../../../../../../weak-solution.md) $u$. Moreover, for every $w\in V$,

$$
J(u+w)-J(u)
=a(u,w)-\ell(w)+\frac12a(w,w)
=\frac12a(w,w)>0
$$

unless $w=0$. Thus $J$ is [strictly convex](../../../../../../../strictly-convex-function.md), and $u$ is its unique global minimizer. This proves existence and uniqueness of the minimizer and of the weak solution simultaneously.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Section A](../../../section-a.md)
4. [Paper 341](../../../../paper-341-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
