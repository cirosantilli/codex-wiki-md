<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use complex-linear [distributions](../../../../../distribution-mathematical-analysis.md), so the pairing contains no complex conjugation. The [space of smooth functions](../../../../../space-of-smooth-functions.md) is $\mathcal E(X)=C^\infty(X)$, with [seminorms](../../../../../seminorm.md)

$$
p_{K,r}(f)=\max_{|\alpha|\leq r}\sup_{x\in K}|\partial^\alpha f(x)|,\qquad K\Subset X.
$$

Thus $f_j\to f$ means uniform convergence of every [derivative](../../../../../derivative.md) on every [compact subset](../../../../../compact-space.md) of $X$. A cofinal [compact exhaustion](../../../../../compact-exhaustion.md) with $K_j\subset\operatorname{int}K_{j+1}$ makes $p_j=p_{K_j,j}$ an increasing defining family. Such an exhaustion exists for every [open set](../../../../../open-set.md); for example, use bounded sets staying a positive distance from its complement and enlarge them slightly. This is a [Fréchet space](../../../../../frechet-space.md).

The [compactly supported distribution space](../../../../../compactly-supported-distribution-space.md) is the [continuous dual space](../../../../../continuous-dual-space-split.md) $\mathcal E'(X)$. We use its [weak-star topology](../../../../../weak-star-topology.md): $u_j\to u$ precisely when $\langle u_j,f\rangle\to\langle u,f\rangle$ for every $f\in\mathcal E(X)$. A stronger standard choice is the [strong dual topology](../../../../../strong-dual-topology.md), which requires uniform convergence on bounded subsets of $\mathcal E(X)$; specifying the weak convention avoids conflating these definitions.

A continuous linear functional necessarily takes null sequences to zero. Conversely, suppose a linear functional $u$ fails to be continuous. For each $j$, it is unbounded on $\{f:p_j(f)\leq1\}$; otherwise scaling would give a continuity estimate. We can therefore choose $f_j$ with

$$
p_j(f_j)\leq\frac1j,\qquad |u(f_j)|\geq1.
$$

For each fixed $l$, $p_l(f_j)\leq p_j(f_j)\to0$ once $j\geq l$. This contradicts the assumed null-sequence property. Hence **sequential continuity characterizes the continuous dual**:

$$
\boxed{u\in\mathcal E'(X)\iff f_j\to0\text{ in }\mathcal E(X)\Longrightarrow u(f_j)\to0.}
$$

This is the [sequential continuity criterion in a metrizable vector space](../../../../../sequential-continuity-criterion-in-a-metrizable-vector-space.md) applied to a linear functional.

Continuity also yields one compact $K\Subset X$, an integer $m$ and a constant $C$ such that $|u(f)|\leq Cp_{K,m}(f)$. Thus $u$ has [compact support](../../../../../compact-support.md) in $K$ and finite [order of a distribution](../../../../../order-of-a-distribution.md). Conversely, a [compactly supported distribution](../../../../../compactly-supported-distribution.md) extends to $\mathcal E(X)$ by $u(f)=u(\eta f)$, where a [cutoff function](../../../../../cutoff-function.md) $\eta$ equals one near its [support of a distribution](../../../../../support-of-a-distribution.md). The local finite-order estimate makes this extension continuous and independent of $\eta$. This identifies the dual definition with compactly supported [distributions](../../../../../distribution-mathematical-analysis.md).

Here is an explicit [compact continuous-derivative representation of a distribution](../../../../../compact-continuous-derivative-representation-of-a-distribution.md). Extend $u$ by zero to $\mathbb R^n$ using a [cutoff function](../../../../../cutoff-function.md) inside $X$, retaining finite order $m$. Put $r=m+2$ and

$$
E(x)=\prod_{j=1}^n\frac{(x_j)_+^{r-1}}{(r-1)!},\qquad\gamma=(r,\ldots,r).
$$

This locally $C^m$ function satisfies $\partial^\gamma E=\delta_0$. Indeed, each one-dimensional factor has $r$th [distributional derivative](../../../../../distributional-derivative.md) equal to the [Dirac delta distribution](../../../../../dirac-delta-function.md). The [convolution](../../../../../convolution.md) $F=u*E$ is continuous: the finite-order estimate extends $u$ to $C^m$ functions near its [compact support](../../../../../compact-support.md), and translated $E$ varies continuously in their $C^m$ norms. Equivalently, mollify $E$ and use the estimate to obtain local uniform convergence of the convolved functions. Distributional differentiation gives $\partial^\gamma F=u$.

Choose $\chi\in C_c^\infty(X)$ equal to one near $\operatorname{supp}u$. Since $\chi u=u$, repeated [Leibniz rule](../../../../../leibniz-rule.md) gives

$$
u=\chi\partial^\gamma F=\sum_{\beta\leq\gamma}(-1)^{|\beta|}\binom\gamma\beta\partial^{\gamma-\beta}\big((\partial^\beta\chi)F\big).
$$

Every coefficient function on the right is continuous and compactly supported in $X$. Thus **the required representation is finite**:

$$
\boxed{u=\sum_\alpha\partial^\alpha f_\alpha,\qquad f_\alpha\in C_c(X).}
$$

The equality first holds on [test functions](../../../../../test-function.md) and then on all [smooth functions](../../../../../smooth-function.md) after inserting a common cutoff, so it holds in $\mathcal E'(X)$.

**A general [distribution](../../../../../distribution-mathematical-analysis.md) need not admit one finite such sum**, even if [compact support](../../../../../compact-support.md) is not required of the [continuous functions](../../../../../continuous-function.md). On $X=\mathbb R$, consider

$$
v=\sum_{j=1}^\infty\delta_j^{(j)}.
$$

The sum is locally finite, so it defines a [distribution](../../../../../distribution-mathematical-analysis.md). If it were a finite sum $\sum_{l=0}^M\partial^l g_l$ with all $g_l$ continuous, then on every fixed compact set its action would be bounded by test [derivatives](../../../../../derivative.md) through order $M$. Near an integer $j>M$, however, it is exactly $\delta_j^{(j)}$, whose order is $j$. To see the contradiction directly, choose a [test function](../../../../../test-function.md) $\psi$ with $\psi^{(j)}(0)\ne0$ and put $\psi_\varepsilon(x)=\varepsilon^j\psi((x-j)/\varepsilon)$. All [derivative](../../../../../derivative.md) norms through order $M$ tend to zero, while $\langle\delta_j^{(j)},\psi_\varepsilon\rangle=(-1)^j\psi^{(j)}(0)$. This is a [distribution of unbounded order](../../../../../distribution-of-unbounded-order.md). In dimensions $n>1$, the same example uses point masses at $(j,0,\ldots,0)$ and [derivatives](../../../../../derivative.md) in the first coordinate.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
