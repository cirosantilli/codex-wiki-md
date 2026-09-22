<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The PDF's $J$ is the anti-diagonal identity matrix. Write $\bar i=2n+2-i$ and $o=n+1$. Its diagonal [Cartan subalgebra](../../../../../../cartan-subalgebra.md) consists of

$$
H=\operatorname{diag}(h_1,\ldots,h_n,0,-h_n,\ldots,-h_1),\qquad
\varepsilon_i(H)=h_i.
$$

The defining matrix identity says $A_{ij}=-A_{\bar j,\bar i}$. The [root spaces](../../../../../../root-space.md) have the following [root vectors](../../../../../../root-vector.md), together with their opposites:

$$
\begin{array}{c|c}
\text{root}&\text{root vector}\\\hline
\varepsilon_i-\varepsilon_j&E_{ij}-E_{\bar j,\bar i}\quad(i\ne j)\\
\varepsilon_i+\varepsilon_j&E_{i,\bar j}-E_{j,\bar i}\quad(i<j)\\
\varepsilon_i&E_{i,o}-E_{o,\bar i}
\end{array}
$$

The negative short root has vector $E_{o,i}-E_{\bar i,o}$. Hence the [root-space decomposition](../../../../../../root-space-decomposition.md) is $\mathfrak g=\mathfrak t\oplus\bigoplus_{\alpha\in R}\mathfrak g_\alpha$, each root space is one-dimensional, and the [Bn root system](../../../../../../bn-root-system.md) is

$$
\boxed{R=\{\pm\varepsilon_i\pm\varepsilon_j:i<j\}\cup\{\pm\varepsilon_i\}.}
$$

There are $2n^2$ roots and $n$ zero-weight dimensions, giving $\dim\mathfrak g=n(2n+1)$ as a check. Upper triangular matrices give

$$
\boxed{R^+=\{\varepsilon_i-\varepsilon_j,\varepsilon_i+\varepsilon_j:i<j\}\cup\{\varepsilon_i\},\quad
\alpha_i=\varepsilon_i-\varepsilon_{i+1}\ (i<n),\quad\alpha_n=\varepsilon_n.}
$$

For $n\geq2$, the [highest root](../../../../../../highest-root.md) is $\theta=\varepsilon_1+\varepsilon_2=\alpha_1+2\alpha_2+\cdots+2\alpha_n$. The [fundamental weights](../../../../../../fundamental-weight.md) and [Weyl vector](../../../../../../half-sum-of-positive-roots.md) are

$$
\boxed{\omega_i=\varepsilon_1+\cdots+\varepsilon_i\ (i<n),\quad
\omega_n=\tfrac12(\varepsilon_1+\cdots+\varepsilon_n),\quad
\rho=\sum_{i=1}^n\left(n-i+\tfrac12\right)\varepsilon_i.}
$$

These weights pair to $\delta_{ij}$ with the [simple coroots](../../../../../../simple-coroot.md); summing the positive roots gives the displayed $\rho$.

The [Dynkin diagram](../../../../../../dynkin-diagram.md) is the chain $1,\ldots,n$, with single edges except a double edge between $n-1$ and $n$, whose arrow points to the short root $\alpha_n$. In the [Extended Dynkin diagram](../../../../../../extended-dynkin-diagram.md), $\alpha_0=-\theta$ attaches by a single edge to $\alpha_2$ when $n\geq3$. For $n=2$, both long nodes $\alpha_0,\alpha_1$ have a double edge to the short node $\alpha_2$. The [Bn Dynkin diagram and affine extension](../../../../../../bn-dynkin-diagram-and-affine-extension.md) below distinguishes these small-rank cases.

<a id="3/i/image-ordinary-and-affine-dynkin-diagrams-of-type-b"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102-bn-dynkin.png)

**[Figure 1](#3/i/image-ordinary-and-affine-dynkin-diagrams-of-type-b). Ordinary and affine Dynkin diagrams of type B**.

For $n=1$, the system is $A_1$: $R^+=\{\varepsilon_1\}$, $\theta=\varepsilon_1$, $\omega_1=\rho=\varepsilon_1/2$. Its ordinary diagram is one node; its affine diagram has two equal-length nodes with the usual affine $A_1$ double bond.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
