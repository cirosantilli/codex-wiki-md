<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $1\to H\to G\to Q\to1$, filter a bar resolution of $G$ by the number of quotient variables, or equivalently use the double complex obtained from projective resolutions over $\mathbb ZH$ and $\mathbb ZQ$. Taking cohomology first in the $H$-direction and then in the $Q$-direction produces the [Lyndon–Hochschild–Serre spectral sequence](../../../../../lyndon-hochschild-serre-spectral-sequence.md)

$$
E_2^{p,q}=H^p\!\left(Q,H^q(H,\mathbb Z)\right)
\Longrightarrow H^{p+q}(G,\mathbb Z).
$$

The quotient acts on $H^q(H,\mathbb Z)$ through conjugation. Differentials have bidegree $(r,1-r)$; after determining the $E_2$-page, one follows these differentials and then resolves the filtration extensions on each total degree.

For the dihedral group of order ten, write $G=D_{10}=C_5\rtimes C_2$, with $H=C_5$ and $Q=C_2$. The [integral cohomology of a finite cyclic group](../../../../../integral-cohomology-of-a-finite-cyclic-group.md) is

$$
H^q(C_5,\mathbb Z)=
\begin{cases}
\mathbb Z,&q=0,\\
\mathbb Z/5,&q>0\text{ even},\\
0,&q\text{ odd}.
\end{cases}
$$

If $u$ generates $H^2(C_5,\mathbb Z)$, inversion acts by $u\mapsto-u$, and hence by $(-1)^r$ on $u^r\in H^{2r}(C_5,\mathbb Z)$. Since multiplication by $2$ is invertible on $\mathbb Z/5$, every positive-degree cohomology group of $C_2$ with coefficients in this module vanishes. Its invariants are $\mathbb Z/5$ when $q$ is divisible by four and zero when $q\equiv2\pmod4$.

Thus the only nonzero terms are

$$
E_2^{0,4r}=\mathbb Z/5\quad(r\geq1),
$$

together with the bottom row

$$
E_2^{0,0}=\mathbb Z,
\qquad
E_2^{2r,0}=\mathbb Z/2\quad(r\geq1).
$$

Degree considerations leave no possible nonzero differential, so the spectral sequence collapses. In total degrees divisible by four, the $\mathbb Z/2$ and $\mathbb Z/5$ filtration factors combine uniquely as $\mathbb Z/10$ because their orders are coprime. Therefore the [integral cohomology of the dihedral group of order ten](../../../../../integral-cohomology-of-the-dihedral-group-of-order-ten.md) is

$$
H^n(D_{10},\mathbb Z)\cong
\begin{cases}
\mathbb Z,&n=0,\\
0,&n\text{ odd},\\
\mathbb Z/2,&n\equiv2\pmod4,\\
\mathbb Z/10,&n>0\text{ and }n\equiv0\pmod4.
\end{cases}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 151](../../paper-151-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
