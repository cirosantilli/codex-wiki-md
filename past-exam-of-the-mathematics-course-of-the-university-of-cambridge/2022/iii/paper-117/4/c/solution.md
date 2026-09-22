<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\delta=\exp(-\varepsilon^{-C})$, with the absolute constant $C$ chosen sufficiently large below, and suppose for a contradiction that no $g_2$ with $0\leq g_2\leq1$ satisfies $\|g_1-g_2\|_{\mathcal F}\leq\varepsilon$.

Let

$$
K=\{g\in\mathcal H_N:0\leq g\leq1\},\qquad
B=\{h\in\mathcal H_N:\|h\|_{\mathcal F}\leq\varepsilon\}.
$$

The set $K$ is compact and convex, while $B$ is closed and convex, so $K+B$ is closed and convex. We use the following finite-dimensional form of the [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md): if a point lies outside a nonempty closed convex set, there is a linear functional whose value at the point is strictly greater than its supremum over that set. Identifying linear functionals on $\mathcal H_N$ through the [inner product](../../../../../../inner-product.md), there is therefore a function $\psi$ such that

$$
\langle g_1,\psi\rangle>
\sup_{g\in K}\langle g,\psi\rangle
+\varepsilon\|\psi\|_{\mathcal F}^{*}.
$$

The separating functional cannot have zero dual norm, so rescale it to make $\|\psi\|_{\mathcal F}^{*}=1$. Because $\mathcal F$ is closed, convex, and symmetric, the finite-dimensional [Bipolar theorem for a dual pair](../../../../../../bipolar-theorem-for-a-dual-pair.md) says that the unit ball of $\|\cdot\|_{\mathcal F}^{*}$ is precisely $\mathcal F$. Thus $\psi\in\mathcal F$ and $|\psi(n)|\leq1$.

The [support function](../../../../../../support-function.md) of $K$ is obtained by choosing $g(n)=1$ where $\psi(n)>0$ and $g(n)=0$ where $\psi(n)<0$. In terms of the [positive part of a real-valued function](../../../../../../positive-part-of-a-real-valued-function.md) $\psi_+=\max(0,\psi)$, the separating inequality becomes

$$
\langle g_1,\psi\rangle>\langle1,\psi_+\rangle+\varepsilon.
$$

Since $0\leq g_1\leq\nu$, pointwise we have $g_1\psi\leq\nu\psi_+$, and hence

$$
\langle\nu-1,\psi_+\rangle>\varepsilon.
$$

Apply the supplied [polynomial approximation of the positive part](../../../../../../polynomial-approximation-of-the-positive-part.md) to $\psi$. If $P_\varepsilon(t)=\sum_{i=0}^m a_it^i$, then its uniform approximation error and $\mathbb E\nu\leq1$ imply

$$
|\langle\nu-1,\psi_+-P_\varepsilon(\psi)\rangle|
\leq\frac{\varepsilon}{100}\mathbb E(\nu+1)
\leq\frac{\varepsilon}{50}.
$$

The constant function $1$ and $\psi$ belong to the dual unit ball. By the assumed submultiplicativity, $\|\psi^i\|_{\mathcal F}^{*}\leq1$ for every $i\geq0$. [Dual seminorm](../../../../../../dual-seminorm.md) therefore gives

$$
|\langle\nu-1,P_\varepsilon(\psi)\rangle|
\leq\sum_{i=0}^m|a_i|\,\|\nu-1\|_{\mathcal F}\|\psi^i\|_{\mathcal F}^{*}
\leq(m+1)\max_i|a_i|\,\delta.
$$

The stated coefficient bound, with $C$ in $\delta$ chosen larger than the absolute constant in that bound, makes this last quantity at most $\varepsilon/50$. Together with the polynomial-approximation error, this contradicts $\langle\nu-1,\psi_+\rangle>\varepsilon$. The required $g_2$ consequently exists. This proves the [dense model theorem for a multiplicative test family](../../../../../../dense-model-theorem-for-a-multiplicative-test-family.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 117](../../../paper-117-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
