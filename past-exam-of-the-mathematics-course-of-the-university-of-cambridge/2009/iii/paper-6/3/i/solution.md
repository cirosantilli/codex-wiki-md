<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $\bar i=2n+1-i$, and let $E_{ab}$ denote a [matrix unit](../../../../../../matrix-unit.md). The diagonal [Cartan subalgebra](../../../../../../cartan-subalgebra.md) consists of

$$
t=\operatorname{diag}(t_1,\ldots,t_n,-t_n,\ldots,-t_1),\qquad \varepsilon_i(t)=t_i.
$$

For a [diagonal matrix](../../../../../../diagonal-matrix.md), $[t,E_{ab}]=(t_a-t_b)E_{ab}$. Substituting into the symplectic relation shows that the following are [root vectors](../../../../../../root-vector.md):

$$
\begin{array}{c|c}
\text{weight}&\text{vector}\\\hline
\varepsilon_i-\varepsilon_j&E_{ij}-E_{\bar j\bar i}\quad(i\ne j)\\
\varepsilon_i+\varepsilon_j&E_{i\bar j}+E_{j\bar i}\quad(i<j)\\
-\varepsilon_i-\varepsilon_j&E_{\bar i j}+E_{\bar j i}\quad(i<j)\\
2\varepsilon_i&E_{i\bar i}\\
-2\varepsilon_i&E_{\bar i i}
\end{array}
$$

The zero [weight space](../../../../../../weight-space.md) is spanned by $H_i=E_{ii}-E_{\bar i\bar i}$. The symplectic equation pairs the remaining entries exactly as in this table; the displayed vectors and the $H_i$ are independent and span the algebra. This proves the [root-space decomposition](../../../../../../root-space-decomposition.md)

$$
\mathfrak g=\mathfrak t\oplus\bigoplus_{\alpha\in R}\mathbb C X_\alpha,\qquad
\boxed{R=\{\pm\varepsilon_i\pm\varepsilon_j:i<j\}\cup\{\pm2\varepsilon_i:1\le i\le n\}.}
$$

There are $2n^2$ [roots of a root system](../../../../../../root-of-a-root-system.md), each with one-dimensional [root space](../../../../../../root-space.md), giving $\dim\mathfrak g=n(2n+1)$.

The upper triangular [root vectors](../../../../../../root-vector.md) select precisely

$$
\boxed{R^+=\{\varepsilon_i-\varepsilon_j,\varepsilon_i+\varepsilon_j:i<j\}\cup\{2\varepsilon_i\}.}
$$

The [simple roots](../../../../../../simple-root.md) of this [Cn root system](../../../../../../cn-root-system.md) are

$$
\alpha_i=\varepsilon_i-\varepsilon_{i+1}\ (1\le i<n),\qquad \alpha_n=2\varepsilon_n.
$$

Indeed, the positive [roots of a root system](../../../../../../root-of-a-root-system.md) have expansions

$$
\begin{aligned}
\varepsilon_i-\varepsilon_j&=\alpha_i+\cdots+\alpha_{j-1},\\
\varepsilon_i+\varepsilon_j&=\alpha_i+\cdots+\alpha_{j-1}+2(\alpha_j+\cdots+\alpha_{n-1})+\alpha_n,\\
2\varepsilon_i&=2(\alpha_i+\cdots+\alpha_{n-1})+\alpha_n.
\end{aligned}
$$

These expansions also identify the [highest root](../../../../../../highest-root.md):

$$
\boxed{\theta=2\varepsilon_1=2\alpha_1+\cdots+2\alpha_{n-1}+\alpha_n.}
$$

Normalize the coordinate [inner product](../../../../../../inner-product.md) by $(\varepsilon_i,\varepsilon_j)=\delta_{ij}$. The [simple coroots](../../../../../../simple-coroot.md) are $\alpha_i^\vee=\varepsilon_i-\varepsilon_{i+1}$ for $i<n$ and $\alpha_n^\vee=\varepsilon_n$. Solving $\langle\omega_j,\alpha_i^\vee\rangle=\delta_{ij}$ gives the [fundamental weights](../../../../../../fundamental-weight.md)

$$
\boxed{\omega_j=\varepsilon_1+\cdots+\varepsilon_j\quad(1\le j\le n).}
$$

In the sum of the positive [roots of a root system](../../../../../../root-of-a-root-system.md), the pair $(\varepsilon_i-\varepsilon_j)+(\varepsilon_i+\varepsilon_j)$ contributes $2\varepsilon_i$, and the long root contributes another $2\varepsilon_i$. Therefore the [Weyl vector](../../../../../../half-sum-of-positive-roots.md) is

$$
\boxed{\rho=\frac12\sum_{\alpha\in R^+}\alpha=\sum_{i=1}^n(n-i+1)\varepsilon_i=\sum_{j=1}^n\omega_j.}
$$

These are the [Positive-root data for Cn](../../../../../../positive-root-data-for-cn.md).

For $n\ge2$, the finite [Dynkin diagram](../../../../../../dynkin-diagram.md) is a chain of $n$ vertices. The bonds between $\alpha_i$ and $\alpha_{i+1}$ for $i<n-1$ are single. The last bond is double, with its arrow pointing from the [long root](../../../../../../long-root.md) $\alpha_n$ toward the [short root](../../../../../../short-root.md) $\alpha_{n-1}$. For the [Extended Dynkin diagram](../../../../../../extended-dynkin-diagram.md), add $\alpha_0=-\theta=-2\varepsilon_1$ at the other end, doubly bonded to $\alpha_1$, with arrow toward $\alpha_1$. The following [Cn Dynkin diagrams](../../../../../../cn-dynkin-diagrams.md) include both ends and the low-rank cases.

<a id="3/i/image-finite-and-extended-cn-dynkin-diagrams-with-arrows-toward-the-short-roots-and-separate-rank-one-and-rank-two-cases"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-6-cn-diagrams.png)

**[Figure 1](#3/i/image-finite-and-extended-cn-dynkin-diagrams-with-arrows-toward-the-short-roots-and-separate-rank-one-and-rank-two-cases). Finite and extended Cn Dynkin diagrams with arrows toward the short roots and separate rank-one and rank-two cases**.

At $n=1$, there is just the root $\alpha_1=2\varepsilon_1$ and one finite vertex. The affine [Cartan matrix](../../../../../../cartan-matrix.md) is $\begin{pmatrix}2&-2\\-2&2\end{pmatrix}$; its two vertices have equal root length, so the double bond has no arrow.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
