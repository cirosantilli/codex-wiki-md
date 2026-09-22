<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\bar i=2n+1-i$ and let $E_{ij}$ denote a [matrix unit](../../../../../../matrix-unit.md). The antidiagonal matrix satisfies $J^{-1}=J$, so the orthogonal condition is $A=-JA^TJ$, or entrywise $A_{ij}=-A_{\bar j\bar i}$. Consequently the diagonal [Cartan subalgebra](../../../../../../cartan-subalgebra.md) is

$$
\mathfrak t=\{H(t)=\operatorname{diag}(t_1,\ldots,t_n,-t_n,\ldots,-t_1)\},\qquad\varepsilon_i(H(t))=t_i.
$$

We first take $n\geq2$. Since $[H,E_{ab}]=(H_{aa}-H_{bb})E_{ab}$, the [matrix root basis of the even orthogonal Lie algebra](../../../../../../matrix-root-basis-of-the-even-orthogonal-lie-algebra.md) gives

$$
\begin{aligned}\mathfrak g_{\varepsilon_i-\varepsilon_j}&=\mathbb C(E_{ij}-E_{\bar j\bar i})&& (i\ne j),\\\mathfrak g_{\varepsilon_i+\varepsilon_j}&=\mathbb C(E_{i\bar j}-E_{j\bar i})&& (i<j),\\\mathfrak g_{-\varepsilon_i-\varepsilon_j}&=\mathbb C(E_{\bar j i}-E_{\bar i j})&& (i<j).
\end{aligned}
$$

The zero [weight space](../../../../../../weight-space.md) is $\mathfrak t$; its [basis](../../../../../../basis.md) is $H_i=E_{ii}-E_{\bar i\bar i}$. No vector of weight $2\varepsilon_i$ occurs, because the corresponding matrix unit is forced to be its own negative. These spaces account for $n+2n(n-1)=n(2n-1)$ dimensions, exhausting the [Special orthogonal Lie algebra](../../../../../../special-orthogonal-lie-algebra.md). Thus its decomposition as a $\mathfrak t$-module and its [Dn root system](../../../../../../dn-root-system.md) are

$$
\boxed{\mathfrak g=\mathfrak t\oplus\bigoplus_{\alpha\in R}\mathfrak g_\alpha,\qquad R=\{\pm\varepsilon_i\pm\varepsilon_j:1\leq i<j\leq n\}.}
$$

Each nonzero [root space](../../../../../../root-space.md) has [dimension](../../../../../../dimension-vector-space.md) one; the zero weight has multiplicity $n$.

The upper triangular [root spaces](../../../../../../root-space.md) are precisely those of weights $\varepsilon_i-\varepsilon_j$ and $\varepsilon_i+\varepsilon_j$ with $i<j$. Therefore

$$
\boxed{R^+=\{\varepsilon_i-\varepsilon_j,\ \varepsilon_i+\varepsilon_j:i<j\},\qquad\alpha_i=\varepsilon_i-\varepsilon_{i+1}\ (1\leq i<n),\quad\alpha_n=\varepsilon_{n-1}+\varepsilon_n.}
$$

These $n$ roots form the [simple roots](../../../../../../simple-root.md). To check that they generate the chosen positive system with nonnegative coefficients, write $\varepsilon_i-\varepsilon_j=\sum_{k=i}^{j-1}\alpha_k$. For $j<n$,

$$
\varepsilon_i+\varepsilon_j=\sum_{k=i}^{j-1}\alpha_k+2\sum_{k=j}^{n-2}\alpha_k+\alpha_{n-1}+\alpha_n,
$$

and for $j=n$ use $\varepsilon_i+\varepsilon_n=\sum_{k=i}^{n-2}\alpha_k+\alpha_n$. Empty sums are zero. Their [linear independence](../../../../../../linear-independence.md) and these expansions identify the base of the [root system](../../../../../../root-system.md).

Equip the real span of the roots in $\mathfrak t^*$ with the [inner product](../../../../../../inner-product.md) making the $\varepsilon_i$ orthonormal. All roots then have squared length two. The [coroots](../../../../../../coroot.md) of $\varepsilon_i\pm\varepsilon_j$ are $H_i\pm H_j$, so the [fundamental weights of Dn](../../../../../../fundamental-weights-of-dn.md), characterized by $\omega_i(\alpha_j^\vee)=\delta_{ij}$, are

$$
\boxed{\begin{aligned}\omega_i&=\varepsilon_1+\cdots+\varepsilon_i&& (1\leq i\leq n-2),\\\omega_{n-1}&=\tfrac12(\varepsilon_1+\cdots+\varepsilon_{n-1}-\varepsilon_n),\\\omega_n&=\tfrac12(\varepsilon_1+\cdots+\varepsilon_{n-1}+\varepsilon_n).
\end{aligned}}
$$

Taking their pairings with $H_j-H_{j+1}$ and $H_{n-1}+H_n$ verifies the defining identities directly. For each pair $i<j$, the sum of its two positive roots is $2\varepsilon_i$. Hence the [half-sum of positive roots](../../../../../../half-sum-of-positive-roots.md) is

$$
\boxed{\rho=\frac12\sum_{\alpha\in R^+}\alpha=\sum_{i=1}^n(n-i)\varepsilon_i=\sum_{i=1}^n\omega_i.}
$$

The [Dynkin diagram](../../../../../../dynkin-diagram.md) has a chain ending at $\alpha_{n-2}$, which is joined to both $\alpha_{n-1}$ and $\alpha_n$. Every edge is a single bond because the root lengths agree; the nonzero off-diagonal simple-root pairings are minus one. The labelled [Dn Dynkin diagram](../../../../../../dn-dynkin-diagram.md) and its low-rank versions are shown below.

<a id="2/a/image-labelled-d-type-dynkin-diagrams-including-the-low-rank-cases"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-3-dynkin-diagrams.png)

**[Figure 1](#2/a/image-labelled-d-type-dynkin-diagrams-including-the-low-rank-cases). Labelled D-type Dynkin diagrams, including the low-rank cases**.

For $n=2$, $\alpha_1=\varepsilon_1-\varepsilon_2$ and $\alpha_2=\varepsilon_1+\varepsilon_2$ are orthogonal, giving two disconnected [A1 root systems](../../../../../../rank-one-root-system.md). For $n=3$, the diagram is the chain $\alpha_2-\alpha_1-\alpha_3$, of type [A3 root system](../../../../../../a3-root-system.md); the displayed weight formulas still apply. If $n=1$ is allowed, $\mathfrak{so}_2=\mathfrak t$ is one-dimensional and abelian: there are no roots or fundamental weights, and $\rho=0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
