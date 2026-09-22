<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Set $w=(u-k)^+$, the [positive part](../../../../../positive-part-of-a-real-valued-function.md) of $u-k$. The allowed [Sobolev chain rule](../../../../../sobolev-chain-rule.md) gives

$$
\nabla w=\mathbf1_{\{u>k\}}\nabla u\quad\text{almost everywhere}.
$$

Use the admissible zero-boundary [Sobolev space](../../../../../sobolev-space-split.md) function $\varphi^2w$ in the [weak formulation](../../../../../weak-formulation.md), with a valid [cutoff function](../../../../../cutoff-function.md) as explained in (ii). Its [gradient](../../../../../gradient.md) is $\varphi^2\nabla w+2\varphi w\nabla\varphi$, so

$$
0=\int\varphi^2 A\nabla w\cdot\nabla w
+2\int\varphi w A\nabla w\cdot\nabla\varphi.
$$

Indeed the [integrands](../../../../../integrand.md) vanish off $\{u>k\}$, and on that set $\nabla w=\nabla u$. The [uniform ellipticity](../../../../../uniformly-elliptic-operator.md) and [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) estimates from (ii) now apply to $w$ and give

$$
\boxed{\int_{B_{1/2}\cap\{u>k\}}|\nabla u|^2\,dx
\leq\frac{4\Lambda^2 M^2}{\lambda^2}
\int_{B_1\cap\{u>k\}}(u-k)^2\,dx,\qquad M=\|\nabla\varphi\|_\infty.}
$$

Fixing the [cutoff function](../../../../../cutoff-function.md) gives the required constant independent of $k$. This is a [superlevel Caccioppoli inequality](../../../../../superlevel-caccioppoli-inequality.md); it uses the [positive part](../../../../../positive-part-of-a-real-valued-function.md) as a test and does not require the truncated function itself to solve the original equation.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
