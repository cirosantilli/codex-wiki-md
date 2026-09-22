<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [space of test functions](../../../../../space-of-test-functions.md) is

$$
\mathcal D(\mathbb R^n)=C_c^\infty(\mathbb R^n).
$$

A sequence $\varphi_j$ converges to $\varphi$ in $\mathcal D$ when all supports lie eventually in one [compact set](../../../../../compact-space.md) $K$ and

$$
\sup_{x\in K}|D^\alpha(\varphi_j-\varphi)(x)|\longrightarrow0
$$

for every [multi-index](../../../../../multi-index-notation.md) $\alpha$. A [distribution](../../../../../distribution-mathematical-analysis.md) is a [linear functional](../../../../../linear-functional.md) $u:\mathcal D\to\mathbb C$ such that, for every compact $K$, there are $C_K>0$ and $m_K\in\mathbb N_0$ with

$$
|\langle u,\varphi\rangle|
\leq C_K\max_{|\alpha|\leq m_K}
\sup_{x\in K}|D^\alpha\varphi(x)|
$$

whenever $\operatorname{supp}\varphi\subseteq K$. Convergence in $\mathcal D'$ is [pointwise convergence on test functions](../../../../../weak-convergence-of-distributions.md).

Continuity plainly implies sequential continuity. Conversely, suppose the linear form is sequentially continuous but the displayed estimate fails for some compact $K$. For every $j$, choose $\varphi_j$ supported in $K$ such that

$$
\max_{|\alpha|\leq j}\sup_K|D^\alpha\varphi_j|\leq\frac1j,
\qquad
|\langle u,\varphi_j\rangle|\geq1.
$$

Then $\varphi_j\to0$ in $\mathcal D$, while $u(\varphi_j)\not\to0$, a contradiction. Hence the seminorm estimate holds on every compact set and $u\in\mathcal D'$.

For a [translation vector](../../../../../vector.md) $h$ and a [multi-index](../../../../../multi-index-notation.md) $\alpha$, define

$$
\langle\tau_hu,\varphi\rangle
=\langle u,\varphi(\mathord\cdot+h)\rangle,
\qquad
\langle D^\alpha u,\varphi\rangle
=(-1)^{|\alpha|}\langle u,D^\alpha\varphi\rangle.
$$

These definitions extend ordinary [translation](../../../../../translation-of-a-distribution.md) and [differentiation](../../../../../derivative.md) to distributions.

If $\tau_{te_i}u=u$ for every $t$, differentiating its pairing at $t=0$ gives $\partial_i u=0$. Conversely, if $\partial_i u=0$, then for every test function

$$
\frac d{dt}\langle\tau_{te_i}u,\varphi\rangle
=\langle u,\partial_i\varphi(\mathord\cdot+te_i)\rangle
=-\langle\partial_i u,\varphi(\mathord\cdot+te_i)\rangle=0.
$$

The pairing is constant in $t$, hence $\tau_{te_i}u=u$. This proves both directions of [translation invariance and vanishing distributional derivative](../../../../../translation-invariance-and-vanishing-distributional-derivative.md).

Finally, the [distributional differentiation](../../../../../distributional-derivative.md) obeys the linear [chain rule](../../../../../chain-rule.md) under the linear coordinates $s=x-y$ and $t=x+y$. Thus

$$
\partial_x^2 f(x-y)=f''(x-y)=\partial_y^2 f(x-y)
$$

and likewise

$$
\partial_x^2 g(x+y)=g''(x+y)=\partial_y^2 g(x+y)
$$

as distributions. Adding the two identities gives

$$
\boxed{u_{xx}-u_{yy}=0},
$$

the [one-dimensional wave equation](../../../../../one-dimensional-wave-equation.md); this is the low-regularity form of the travelling waves in the [D'Alembert formula](../../../../../d-alembert-s-formula.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 327](../../paper-327-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
