<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work in the real [Hilbert space](../../../../../../hilbert-space-split.md) $L^2(\mathbb R^2)$, with $g\in L^2$ and $\alpha>0$. The penalty $J$ is a [proper convex function](../../../../../../proper-convex-function.md): it is finite at zero, and the [bounded-variation space](../../../../../../function-of-bounded-variation-on-a-domain.md) domain is [convex](../../../../../../convex-function.md). Its [subdifferential](../../../../../../subdifferential.md) at a finite-penalty $u$ consists of $q\in L^2$ satisfying $J(v)\ge J(u)+\langle q,v-u\rangle$ for every $v\in L^2$.

If $q=(g-u)/\alpha\in\partial J(u)$, expand the quadratic term and use the [subgradient inequality](../../../../../../subgradient-inequality.md):

$$
\alpha J(v)+\tfrac12\|v-g\|_2^2-\alpha J(u)-\tfrac12\|u-g\|_2^2\ge\alpha\langle q,v-u\rangle+\langle u-g,v-u\rangle+\tfrac12\|v-u\|_2^2=\tfrac12\|v-u\|_2^2.
$$

Thus $u$ is the unique minimizer.

Conversely, let $u$ be a minimizer. Its penalty is finite since comparison with zero gives a finite objective. For any $v$ with $J(v)<\infty$, set $w_t=u+t(v-u)$, where $0<t\le1$. [Convexity](../../../../../../convex-function.md) gives $J(w_t)-J(u)\le t(J(v)-J(u))$. Minimality and quadratic expansion then imply

$$
0\le\alpha\bigl(J(v)-J(u)\bigr)+\langle u-g,v-u\rangle+\tfrac t2\|v-u\|_2^2.
$$

Letting $t\downarrow0$ yields $J(v)\ge J(u)+\langle(g-u)/\alpha,v-u\rangle$. The inequality is automatic if $J(v)=\infty$. Hence

$$
\boxed{u\text{ minimizes }\alpha J+\tfrac12\|\mathord\cdot-g\|_2^2\ \Longleftrightarrow\ \frac{g-u}{\alpha}\in\partial J(u).}
$$

This also follows from the [subdifferential sum rule](../../../../../../subdifferential-sum-rule.md), since the quadratic term is everywhere [continuous](../../../../../../continuous-function.md) and [differentiable](../../../../../../differentiable-function.md), and the [subgradient optimality condition](../../../../../../subgradient-optimality-condition.md). The direct proof above needs no unproved existence theorem.

**On the entire plane, the printed global BV domain is not closed in the L2 geometry.** The usual $BV(\mathbb R^2)$ definition includes an $L^1$ condition. For $1<a\le2$, $f(x)=(1+|x|)^{-a}$ belongs to $L^2$, has finite distributional variation $2\pi a\int_0^\infty r(1+r)^{-a-1}\,dr$, and fails to belong to $L^1$. The truncated $f_T=f\chi_{B(0,T)}$ lies in $BV\cap L^2$ and tends to $f$ in $L^2$. Its variation is the interior variation plus $2\pi T(1+T)^{-a}$, and tends to a finite limit. Thus $J(f_T)$ stays bounded but the literal $J(f)=\infty$, establishing [failure of L2 closure of the global BV domain](../../../../../../failure-of-l2-closure-of-the-global-bv-domain.md). One must not infer universal minimizer existence from an inapplicable closed-penalty [proximal operator](../../../../../../proximal-operator.md) theorem. The standard closed extension uses the [homogeneous bounded-variation space](../../../../../../homogeneous-bounded-variation-space.md), allowing finite distributional variation without global $L^1$. The optimality equivalence just proved is valid for the literal penalty whenever a minimizer exists; the next datum has an explicit certified minimizer in its domain.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
