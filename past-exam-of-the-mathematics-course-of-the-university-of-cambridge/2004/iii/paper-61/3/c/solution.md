<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $F^\sharp(k)=\overline{F(\bar k)}$. The defocusing reduction of the [Lax pair](../../../../../../lax-pair.md) is $\mu(k)=\sigma_1\overline{\mu(\bar k)}\sigma_1$, so the [half-line NLS spectral functions](../../../../../../half-line-nls-spectral-functions.md) have the form

$$
s=\begin{pmatrix}a^\sharp&b\\b^\sharp&a\end{pmatrix},\qquad S=\begin{pmatrix}A^\sharp&B\\B^\sharp&A\end{pmatrix},\qquad aa^\sharp-bb^\sharp=AA^\sharp-BB^\sharp=1.
$$

Put $d=aA^\sharp-bB^\sharp$. Select bounded analytic columns and divide by their determinants to define

$$
M=\begin{cases}([\mu_2]_1/a,[\mu_3]_2),&k\in D_1,\\([\mu_1]_1/d,[\mu_3]_2),&k\in D_2,\\([\mu_3]_1,[\mu_1]_2/d^\sharp),&k\in D_3,\\([\mu_3]_1,[\mu_2]_2/a^\sharp),&k\in D_4.\end{cases}
$$

For example, $[\mu_3]_2=b e^{-2i\theta}[\mu_2]_1+a[\mu_2]_2$, so the first pair has determinant $a$ before division. The corresponding determinant for the second pair is $d$. The other two are their reflected counterparts. Hence $\det M=1$ and $M\to I$ at spectral infinity.

Here are explicit connection matrices furnishing every jump. Write $E=e^{-2i\theta}$; wherever the boundary values coexist, $M_j=\mu_2C_j$, with

$$
C_1=\begin{pmatrix}1/a&bE\\0&a\end{pmatrix},\quad C_2=\begin{pmatrix}A^\sharp/d&bE\\B^\sharp E^{-1}/d&a\end{pmatrix},\quad C_3=\begin{pmatrix}a^\sharp&BE/d^\sharp\\b^\sharp E^{-1}&A/d^\sharp\end{pmatrix},\quad C_4=\begin{pmatrix}a^\sharp&0\\b^\sharp E^{-1}&1/a^\sharp\end{pmatrix}.
$$

Orient each ray away from zero; the plus side is its left side. Then $M_+=M_-J$, with **$J=C_-^{-1}C_+$**, entirely determined by the spectral functions. For instance, on the positive real axis,

$$
J=C_4^{-1}C_1=\begin{pmatrix}1/(aa^\sharp)&(b/a^\sharp)e^{-2i\theta}\\-(b^\sharp/a)e^{2i\theta}&1\end{pmatrix}.
$$

The relevant [Riemann-Hilbert problem](../../../../../../riemann-hilbert-problem.md) contour is therefore

$$
\boxed{\Sigma=\mathbb R\cup i\mathbb R.}
$$

It is a cross because time analyticity involves the sign of $\operatorname{Im}k^2$, not just $\operatorname{Im}k$. Zeros of the denominators require residue conditions or small contour detours; they may not simply be ignored. The [half-line NLS Riemann-Hilbert reconstruction](../../../../../../half-line-nls-riemann-hilbert-reconstruction.md) recovers $q=2i\lim_{k\to\infty}kM_{12}$, by matching the constant term $i[\sigma_3,M_1]=Q$ in the spatial [Lax pair](../../../../../../lax-pair.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
