<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The necessary formulation uses a real [Hilbert space](../../../../../../hilbert-space-split.md) $V$ of functions satisfying the essential [boundary conditions](../../../../../../boundary-condition.md), a continuous symmetric [bilinear form](../../../../../../bilinear-form.md) $a$, and a continuous [linear functional](../../../../../../linear-functional.md) $\ell$. Assume constants $C,c>0$ with

$$
|a(v,w)|\leq C\|v\|_V\|w\|_V,\qquad
\boxed{a(v,v)\geq c\|v\|_V^2.}
$$

The latter is [coercivity](../../../../../../coercive-function.md), the positive-definiteness condition needed in the chosen complete space. On the domain of the strong differential operator, [integration by parts](../../../../../../integration-by-parts.md) and the [boundary conditions](../../../../../../boundary-condition.md) identify $a(v,w)=\langle\mathcal Lv,w\rangle$; this form extends to $V$. Let $\ell(w)=\langle f,w\rangle$ for admissible forcing. Define

$$
I(v)=a(v,v)-2\ell(v),\qquad
\boxed{u\text{ is a weak solution if }a(u,w)=\ell(w)\text{ for every }w\in V.}
$$

When $u$ has the regularity to belong to the strong operator domain, this is $\mathcal Lu=f$ with its [boundary conditions](../../../../../../boundary-condition.md). For complex spaces use a Hermitian form and $-2\operatorname{Re}\ell(v)$ to make the functional real.

Here is an existence proof by minimization. Continuity of $\ell$ and [coercivity](../../../../../../coercive-function.md) give $I(v)\geq c\|v\|_V^2-2\|\ell\|_{V^*}\|v\|_V$, so $m=\inf_VI$ is finite and a minimizing sequence $v_n$ is bounded. The quadratic parallelogram identity is

$$
I((v_n+v_j)/2)=\frac{I(v_n)+I(v_j)}2-\frac14a(v_n-v_j,v_n-v_j).
$$

Since its left side is at least $m$,

$$
a(v_n-v_j,v_n-v_j)\leq2\bigl(I(v_n)+I(v_j)-2m\bigr)\longrightarrow0.
$$

[Coercivity](../../../../../../coercive-function.md) makes $v_n$ Cauchy in $V$. [Completeness](../../../../../../completeness.md) gives $v_n\to u\in V$, and continuity of the form and forcing gives $I(u)=m$.

For every $w\in V$, differentiation along $u+tw$ yields

$$
0=\frac d{dt}I(u+tw)\bigg|_{t=0}=2a(u,w)-2\ell(w).
$$

Thus the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) is exactly the stated [weak solution](../../../../../../weak-solution.md) equation. Conversely, if $u$ satisfies it, expansion gives

$$
\boxed{I(v)-I(u)=a(v-u,v-u)\geq c\|v-u\|_V^2.}
$$

This proves that the [weak solution](../../../../../../weak-solution.md) is the unique global minimum and that two [weak solutions](../../../../../../weak-solution.md) coincide. It proves the symmetric coercive case underlying the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) directly, rather than taking existence as a theorem name. The framework is [symmetry and coercivity in quadratic energy minimization](../../../../../../symmetry-and-coercivity-in-quadratic-energy-minimization.md).

The qualifications matter if positive definiteness is read more weakly. For a nonsymmetric operator the derivative of $\langle\mathcal Lv,v\rangle$ uses $(\mathcal L+\mathcal L^*)/2$, so it need not give $\mathcal Lu=f$. For example, on smooth periodic real functions $\mathcal L=1+\partial_x$ has $\langle\mathcal Lv,v\rangle=\|v\|_2^2$, but the functional's equation is $u=f$, not $u+u_x=f$. Even a symmetric operator can be strictly positive without being coercive: on [l2 sequence space](../../../../../../l2-sequence-space.md), $(Lv)_n=v_n/n$ with $f_n=1/n$ would require a solution $u_n=1$, which is not square summable. The associated functional has values $-\sum_{n=1}^N1/n$ on vectors with the first $N$ entries equal to one, so it has no minimum in that space. This is [strict positivity without coercivity can fail variational solvability](../../../../../../strict-positivity-without-coercivity-can-fail-variational-solvability.md). Under the usual symmetric coercive meaning of positive definiteness, the proof above supplies every assertion requested.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
