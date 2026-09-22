<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

After ordering a [symplectic basis](../../../../../../symplectic-basis.md) in two blocks, write

$$
h=\operatorname{diag}(t_1,\ldots,t_n,-t_1,\ldots,-t_n),
\qquad \varepsilon_i(h)=t_i.
$$

Matrices in the [symplectic Lie algebra](../../../../../../symplectic-lie-algebra.md) have block form

$$
\begin{pmatrix}A&B\\ C&-A^T\end{pmatrix},
\qquad B=B^T,quad C=C^T.
$$

The [root-space decomposition](../../../../../../root-space-decomposition.md) is

$$
\mathfrak{sp}_{2n}=\mathfrak t
\oplus\bigoplus_{i\ne j}\mathfrak g_{\varepsilon_i-\varepsilon_j}
\oplus\bigoplus_{i<j}\left(\mathfrak g_{\varepsilon_i+\varepsilon_j}\oplus\mathfrak g_{-\varepsilon_i-\varepsilon_j}\right)
\oplus\bigoplus_i\left(\mathfrak g_{2\varepsilon_i}\oplus\mathfrak g_{-2\varepsilon_i}\right).
$$

For example, these one-dimensional spaces are spanned respectively by

$$
E_{ij}-E_{n+j,n+i},\quad
E_{i,n+j}+E_{j,n+i},\quad
E_{n+i,j}+E_{n+j,i},\quad
E_{i,n+i},\quad E_{n+i,i}.
$$

Thus this is the [Cn root system](../../../../../../cn-root-system.md)

$$
R=\{\pm\varepsilon_i\pm\varepsilon_j:i<j\}\cup\{\pm2\varepsilon_i:1\leq i\leq n\}.
$$

The upper-triangular choice gives

$$
R^+=\{\varepsilon_i-\varepsilon_j:i<j\}
\cup\{\varepsilon_i+\varepsilon_j:i<j\}
\cup\{2\varepsilon_i:1\leq i\leq n\}.
$$

Its [simple roots](../../../../../../simple-root.md), [highest root](../../../../../../highest-root.md), [fundamental weights](../../../../../../fundamental-weight.md), and [half-sum of positive roots](../../../../../../half-sum-of-positive-roots.md) are

$$
\begin{aligned}
\alpha_i&=\varepsilon_i-\varepsilon_{i+1} &&(1\leq i<n),&
\alpha_n&=2\varepsilon_n,\\
\theta&=2\varepsilon_1,&
\omega_k&=\varepsilon_1+\cdots+\varepsilon_k &&(1\leq k\leq n),\\
\rho&=n\varepsilon_1+(n-1)\varepsilon_2+\cdots+\varepsilon_n.
\end{aligned}
$$

Using the notation requested in the paper, the root lattice $P$ and weight lattice $Q$ are

$$
P=\left\{(m_1,\ldots,m_n)\in\mathbb Z^n:\sum_i m_i\equiv0\pmod2\right\},
\qquad Q=\mathbb Z^n,
$$

so $Q/P\cong\mathbb Z/2\mathbb Z$. This reverses the common notation in which the [root lattice](../../../../../../root-lattice.md) is called $Q$ and the [weight lattice](../../../../../../weight-lattice.md) is called $P$.

Since a multiple-edge arrow in a [Dynkin diagram](../../../../../../dynkin-diagram.md) points toward the shorter root, the finite and [extended](../../../../../../extended-dynkin-diagram.md) diagrams are

$$
\alpha_1-\alpha_2-\cdots-\alpha_{n-2}-\alpha_{n-1}\Longleftarrow\alpha_n
$$

and

$$
\alpha_0\Longrightarrow\alpha_1-\alpha_2-\cdots-\alpha_{n-2}-\alpha_{n-1}\Longleftarrow\alpha_n,
\qquad \alpha_0=-2\varepsilon_1.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
