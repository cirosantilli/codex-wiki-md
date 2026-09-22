<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We apply the closed-bounded-domain version of the [Schauder fixed-point theorem](../../../../schauder-fixed-point-theorem.md) in the [Banach space](../../../../banach-space-split.md) $L^2(\Omega)$. Write $m=|\Omega|$ and use $G,T,C_P$ from part (b)(ii). Choose

$$
a=C_P^2m^{1/2},\qquad b=C_P^2m^{1/4},\qquad
R=\max\{1,2a,4b^2\},
\qquad C=\{w\in L^2(\Omega):w\geq0\text{ a.e.},\ \|w\|_2\leq R\}.
$$

The set $C$ is nonempty, bounded, closed and a [convex set](../../../../convex-set-split.md). For closedness of its positivity condition, if $w_j\geq0$ and $w_j\to w$ in $L^2$, then pointwise $w^-\leq|w-w_j|$, whence $\|w^-\|_2\to0$.

The [weak maximum principle](../../../../weak-maximum-principle-for-elliptic-operators.md) already gives $Tw\geq0$. Our estimates give, for $w\in C$,

$$
\|Tw\|_2\leq C_P^2\bigl(m^{1/2}+m^{1/4}\|w\|_2^{1/2}\bigr)
\leq a+b\sqrt R\leq R/2+R/2=R.
$$

Thus $T(C)\subset C$.

To prove [continuity](../../../../continuous-function.md), use the pointwise [square root](../../../../square-root.md) estimate $|\sqrt s-\sqrt t|^2\leq|s-t|$ for $s,t\geq0$. The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) then gives

$$
\|\sqrt w-\sqrt z\|_2^2\leq\|w-z\|_1\leq m^{1/2}\|w-z\|_2,
\qquad
\|Tw-Tz\|_2\leq C_P^2m^{1/4}\|w-z\|_2^{1/2}.
$$

Hence $T$ is a [continuous map](../../../../continuous-map.md) on $C$, even though the [square root](../../../../square-root.md) need not have a bounded [derivative](../../../../derivative.md) near zero.

Finally,

$$
\|\nabla Tw\|_2\leq C_P\bigl(m^{1/2}+m^{1/4}\sqrt R\bigr)
\qquad(w\in C).
$$

The [Rellich-Kondrachov theorem](../../../../rellich-kondrachov-theorem.md) says that $H_0^1(\Omega)$ embeds compactly into $L^2(\Omega)$ on a bounded smooth [domain](../../../../domain-mathematical-analysis.md). For $n>2$, $2<2n/(n-2)$, and for $n=2$ every finite target exponent is available, so the required [compact embedding](../../../../compact-embedding.md) holds in every dimension in the question. Thus $T(C)$ is [relatively compact](../../../../relatively-compact-subset.md) in $L^2(\Omega)$.

All hypotheses of the [Schauder fixed-point theorem](../../../../schauder-fixed-point-theorem.md) are met. It gives $u=Tu\in C$, and part (b)(ii) converts this [fixed point](../../../../fixed-point.md) into the required [weak solution](../../../../weak-solution.md):

$$
\boxed{\text{There exists }u\in H_0^1(\Omega),\ u\geq0\text{ a.e., with }
\int_\Omega\nabla u\cdot\nabla v\,dx=\int_\Omega(1+\sqrt u)v\,dx
\quad\forall v\in H_0^1(\Omega).}
$$

Only existence is needed. The construction does not assume that $\Omega$ is small or that $T$ is a [contraction mapping](../../../../contraction-mapping.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
