<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For real $q$, write $\bar f(k)=\overline{f(\bar k)}$. The reduction symmetry and unit determinants give the [scattering data](../../../../../../scattering-data.md) parametrizations

$$
s=\begin{pmatrix}\bar a&b\\\lambda\bar b&a\end{pmatrix},\qquad
S=\begin{pmatrix}\bar A&B\\\lambda\bar B&A\end{pmatrix},\qquad
\bar aa-\lambda\bar bb=\bar AA-\lambda\bar BB=1.
$$

To see the symmetry, conjugate the coefficient matrices by $C=\begin{pmatrix}0&1\\\lambda&0\end{pmatrix}$ after taking complex conjugates at $\bar k$; $C\sigma_3C^{-1}=-\sigma_3$ and the real-$q$ reduction restore the original [Lax pair](../../../../../../lax-pair.md). Define

$$
d_+=\bar aA-\lambda\bar bB,\qquad d_-=\bar Aa-\lambda\bar Bb.
$$

If $\mu_j^{(l)}$ denotes column $l$, bounded columns produce the following normalized matrices:

$$
\begin{aligned}
M_1&=(\mu_3^{(1)}/d_+,\ \mu_1^{(2)}),&&k\in D_1,\\
M_2&=(\mu_3^{(1)}/\bar a,\ \mu_2^{(2)}),&&k\in D_2,\\
M_3&=(\mu_2^{(1)},\ \mu_3^{(2)}/a),&&k\in D_3,\\
M_4&=(\mu_1^{(1)},\ \mu_3^{(2)}/d_-),&&k\in D_4.
\end{aligned}
$$

Each divisor is exactly the determinant of the unscaled column pair, so $\det M_j=1$. The eigenfunctions and divisors tend to $I$ and one, respectively, giving $M\to I$ at infinity. The contour for the [sectorial half-line mKdV Riemann-Hilbert reconstruction](../../../../../../sectorial-half-line-mkdv-riemann-hilbert-reconstruction.md) is

$$
\boxed{\Sigma=\{k:\operatorname{Im}k=0\ \text{or}\ \operatorname{Im}k^3=0\}
=\bigcup_{m=0}^5\{re^{im\pi/3}:r\ge0\}.}
$$

It is six rays, not just the real axis or a four-quadrant contour. For the displayed meromorphic construction assume the divisors have no zeros on the contour; contour zeros require an indented or otherwise regularized formulation.

Here are explicit jump data without ambiguity about which side is used. Define

$$
\begin{aligned}
C_1&=\begin{pmatrix}\bar a/d_+&B\\\lambda\bar b/d_+&A\end{pmatrix},&
C_2&=\begin{pmatrix}1&0\\\lambda\bar b/\bar a&1\end{pmatrix},\\
C_3&=\begin{pmatrix}1&b/a\\0&1\end{pmatrix},&
C_4&=\begin{pmatrix}\bar A&b/d_-\\\lambda\bar B&a/d_-\end{pmatrix}.
\end{aligned}
$$

The connection formulas give $M_j=\mu_2e^{i\theta\widehat\sigma_3}C_j$. Orient each ray outwards and let plus mean its left side. If that ray separates domains $D_i$ on the minus side and $D_j$ on the plus side, its jump is

$$
\boxed{M_+=M_-J,\qquad J=e^{i\theta\widehat\sigma_3}(C_i^{-1}C_j).}
$$

This specifies every jump using only the spectral connection matrices; each jump has determinant one. Boundedness and consistency at the junction are inherited from the original eigenfunctions when the spectral data satisfy their global constraint.

If $a,\bar a,d_+$ or $d_-$ has zeros in its corresponding domain, their simple zeros generate poles and require [residue](../../../../../../residue.md) conditions. For example, at a simple zero $k_0$ of $a$ in $D_3$,

$$
\operatorname{Res}_{k=k_0}M^{(2)}
=\frac{b(k_0)e^{2i\theta(k_0)}}{a'(k_0)}M^{(1)}(k_0).
$$

At a simple zero of $d_+$ in $D_1$, the analogous coefficient for the first column is $\lambda\bar b\,e^{-2i\theta}/(A d_+')$ times the second column; in $D_4$ it is $b\,e^{2i\theta}/(\bar A d_-')$ for the second column. The $\bar a$ residue in $D_2$ is the conjugate first-column relation. These formulas assume the other displayed denominators are nonzero there; multiple or coincident zeros need their corresponding higher-order conditions. In a sufficiently small-data zero-free regime, the normalized [Riemann-Hilbert problem](../../../../../../riemann-hilbert-problem.md) has only the jumps. Finally the order-one term in $\mu_x-ik[\sigma_3,\mu]=Q\mu$ gives

$$
\boxed{q(x,t)=-2i\lim_{k\to\infty}kM_{12}(x,t,k).}
$$

The column normalizations do not change this off-diagonal leading coefficient.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
