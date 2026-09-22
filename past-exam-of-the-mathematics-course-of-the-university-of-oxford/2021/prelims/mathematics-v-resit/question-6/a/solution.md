<h1 id="question-6/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

Let $u_1,u_2$ be two solutions with the same data, and write $w=u_1-u_2$ on the rectangle $\Omega=(0,\pi)\times(-1,1)$. By [linearity](../../../../../../linearity.md),

$$
\Delta w=0,\qquad
w(x,-1)=w(x,1)=0,\qquad
w_x(0,y)=w_x(\pi,y)=0.
$$

The [normal derivative](../../../../../../normal-derivative.md) is $-w_x$ on the left edge and $w_x$ on the right edge, so it vanishes on both. The [energy method](../../../../../../energy-method.md) applies [Green's first identity](../../../../../../green-s-first-identity.md), which follows by integrating

$$
\nabla\cdot(w\nabla w)=|\nabla w|^2+w\Delta w.
$$

It gives

$$
\iint_\Omega|\nabla w|^2\,dA
=\int_{\partial\Omega}w\,\partial_nw\,ds
-\iint_\Omega w\Delta w\,dA=0.
$$

The boundary term vanishes on each horizontal edge because $w=0$, and on each vertical edge because $\partial_nw=0$. The interior term vanishes because $w$ is a [harmonic function](../../../../../../harmonic-function.md). Since the continuous integrand $|\nabla w|^2$ is nonnegative, a zero [integral](../../../../../../integral-split.md) forces $\nabla w=\mathbf0$. The rectangle is [connected](../../../../../../connected-space.md), so $w$ is constant; its zero value on either horizontal edge makes that constant zero. Hence

$$
\boxed{u_1=u_2}.
$$

This proof assumes enough boundary regularity for [Green's first identity](../../../../../../green-s-first-identity.md). It also works in the finite [Dirichlet energy](../../../../../../dirichlet-energy.md) class using the weak identity with test function $w$, so it remains applicable when corner derivatives are not continuous. It proves uniqueness conditional on existence and does not impose a compatibility condition for arbitrary $f,g$.

## ↑ Ancestors (12)

1. [a](../a.md)
2. [Question 6](../../question-6.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
