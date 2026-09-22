<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $T=\begin{pmatrix}P&Q\\R&S\end{pmatrix}$ and $J=\begin{pmatrix}0&I_l\\-I_l&0\end{pmatrix}$. Block multiplication gives

$$
T^{\mathsf T}J+JT=
\begin{pmatrix}R-R^{\mathsf T}&P^{\mathsf T}+S\\-S^{\mathsf T}-P&Q^{\mathsf T}-Q\end{pmatrix}.
$$

Its vanishing is equivalent to

$$
\boxed{S=-P^{\mathsf T},\qquad Q=Q^{\mathsf T},\qquad R=R^{\mathsf T}.}
$$

This identifies $L$ with the [symplectic Lie algebra](../../../../../../symplectic-lie-algebra.md) $\mathfrak{sp}_{2l}(\mathbb C)$.

We now supply the requested [root-space decomposition](../../../../../../root-space-decomposition.md), including explicit vectors. Let $E_{ab}$ be the [matrix units](../../../../../../matrix-unit.md), put $h_i=E_{ii}-E_{l+i,l+i}$, and define the [linear functionals](../../../../../../linear-functional.md) $\varepsilon_i$ on the diagonal [Cartan subalgebra](../../../../../../cartan-subalgebra.md) by $\varepsilon_i(h)=\lambda_i$. Then $H=\bigoplus_i\mathbb C h_i$. The [Cn root system](../../../../../../cn-root-system.md) and a corresponding [matrix root basis of the symplectic Lie algebra](../../../../../../matrix-root-basis-of-the-symplectic-lie-algebra.md) are

$$
\begin{aligned}
e_{\varepsilon_i-\varepsilon_j}&=E_{ij}-E_{l+j,l+i} &&(i\ne j),\\
e_{\varepsilon_i+\varepsilon_j}&=E_{i,l+j}+E_{j,l+i} &&(i<j),\\
e_{-\varepsilon_i-\varepsilon_j}&=E_{l+i,j}+E_{l+j,i} &&(i<j),\\
e_{2\varepsilon_i}&=E_{i,l+i},\qquad e_{-2\varepsilon_i}=E_{l+i,i}.&&
\end{aligned}
$$

Each listed vector satisfies the block conditions just proved. For a diagonal matrix $h$, the [matrix unit](../../../../../../matrix-unit.md) calculation $[h,E_{ab}]=(h_{aa}-h_{bb})E_{ab}$ gives all the requested [eigenvalues](../../../../../../eigenvalue.md) explicitly:

$$
\begin{aligned}
[h,e_{\varepsilon_i-\varepsilon_j}]&=(\lambda_i-\lambda_j)e_{\varepsilon_i-\varepsilon_j},\\
[h,e_{\varepsilon_i+\varepsilon_j}]&=(\lambda_i+\lambda_j)e_{\varepsilon_i+\varepsilon_j},\\
[h,e_{-\varepsilon_i-\varepsilon_j}]&=-(\lambda_i+\lambda_j)e_{-\varepsilon_i-\varepsilon_j},\\
[h,e_{2\varepsilon_i}]&=2\lambda_i e_{2\varepsilon_i},\qquad
[h,e_{-2\varepsilon_i}]=-2\lambda_i e_{-2\varepsilon_i}.
\end{aligned}
$$

The diagonal vectors and difference-root vectors span every possible $P$ block. The sum-root and doubled-root vectors span all symmetric $Q$ and $R$ blocks. They are [linearly independent](../../../../../../linear-independence.md), as is evident from their disjoint independent block entries. Equivalently there are $l+2l^2=l(2l+1)$ of them, exactly the [dimension](../../../../../../dimension-vector-space.md) $l^2+2l(l+1)/2$ of $L$. The zero weight space is precisely $H$: a zero weight forces $P$ diagonal and every entry of $Q,R$ to vanish. Hence every nonzero [root space](../../../../../../root-space.md) is one-dimensional and

$$
\boxed{L=H\oplus\bigoplus_{r\in\{\pm(\varepsilon_i\pm\varepsilon_j):i<j\}\cup\{\pm2\varepsilon_i\}}\mathbb C e_r,\qquad [h,e_r]=r(h)e_r.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
