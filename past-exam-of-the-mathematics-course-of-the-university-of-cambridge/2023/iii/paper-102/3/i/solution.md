<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write an element of the diagonal torus as

$$
\operatorname{diag}(t_1,\ldots,t_n,-t_n,\ldots,-t_1)
$$

and let $\varepsilon_i$ extract $t_i$. The [root-space decomposition](../../../../../../root-space-decomposition.md) is

$$
\mathfrak{so}_{2n}
=\mathfrak t\oplus
\bigoplus_{1\leq i<j\leq n}
\left(
\mathfrak g_{\varepsilon_i-\varepsilon_j}\oplus
\mathfrak g_{\varepsilon_i+\varepsilon_j}\oplus
\mathfrak g_{-\varepsilon_i+\varepsilon_j}\oplus
\mathfrak g_{-\varepsilon_i-\varepsilon_j}
\right),
$$

with one-dimensional root spaces. Thus the $D_n$ [root system](../../../../../../root-system.md) is

$$
R=\{\pm\varepsilon_i\pm\varepsilon_j:i<j\}.
$$

The upper-triangular choice gives

$$
R^+=\{\varepsilon_i-\varepsilon_j,\ \varepsilon_i+\varepsilon_j:i<j\}.
$$

A compatible simple system is

$$
\alpha_i=\varepsilon_i-\varepsilon_{i+1}\quad(1\leq i<n),\qquad
\alpha_n=\varepsilon_{n-1}+\varepsilon_n.
$$

The [highest root](../../../../../../highest-root.md) and [Weyl vector](../../../../../../half-sum-of-positive-roots.md) are

$$
\theta=\varepsilon_1+\varepsilon_2
=\alpha_1+2\alpha_2+\cdots+2\alpha_{n-2}+\alpha_{n-1}+\alpha_n,
\qquad
\rho=\sum_{i=1}^n(n-i)\varepsilon_i.
$$

The [fundamental weights](../../../../../../fundamental-weight.md) are

$$
\omega_k=\varepsilon_1+\cdots+\varepsilon_k\quad(1\leq k\leq n-2),
$$



$$
\omega_{n-1}=\frac12(\varepsilon_1+\cdots+\varepsilon_{n-1}-\varepsilon_n),
\qquad
\omega_n=\frac12(\varepsilon_1+\cdots+\varepsilon_n).
$$

Using the paper's letters, the root lattice and weight lattice are respectively

$$
P=\left\{(a_i)\in\mathbb Z^n:\sum_i a_i\ \text{is even}\right\},
\qquad
Q=\mathbb Z^n\cup\left(\mathbb Z+\frac12\right)^n.
$$

Their quotient is

$$
Q/P\cong
\begin{cases}
\mathbb Z/2\mathbb Z\times\mathbb Z/2\mathbb Z,&n\text{ even},\\
\mathbb Z/4\mathbb Z,&n\text{ odd}.
\end{cases}
$$

The [Dynkin diagram](../../../../../../dynkin-diagram.md) is the $D_n$ diagram: a chain $\alpha_1-\cdots-\alpha_{n-2}$ whose last node is joined to both $\alpha_{n-1}$ and $\alpha_n$. The [Extended Dynkin diagram](../../../../../../extended-dynkin-diagram.md) adds $\alpha_0=-\theta$ joined to $\alpha_2$. For $D_4$, the central node $\alpha_2$ consequently has the four leaves $\alpha_0,\alpha_1,\alpha_3,\alpha_4$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
