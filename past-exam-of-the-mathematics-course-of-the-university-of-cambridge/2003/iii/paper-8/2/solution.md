<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Work locally in $z$ where $u\ne0$, and take the [matrix](../../../../../matrix.md) entries literally as they appear in the original PDF. At fixed $z$, abbreviate

$$
D=\operatorname{diag}(1,-1),\quad U=u,\quad P=u',\quad
V=-\frac{zw}{u},\quad R=\frac{2u'w}{u^2},\quad d=w+\frac z2.
$$

Then $A=D\lambda^2+\left(\begin{smallmatrix}0&U\\V&0\end{smallmatrix}\right)\lambda+\left(\begin{smallmatrix}d&P\\R&-d\end{smallmatrix}\right)$. Define

$$
h=d+\frac{UV}{2},\qquad \theta=\frac{UR+VP}{2},\qquad
\rho=\frac{UV(d+h)}4-\frac{PR}{2}.
$$

The literal coefficients give

$$
\boxed{h=\frac z2+\left(1-\frac z2\right)w,\qquad
\theta=\frac{(2-z)u'w}{2u}.}
$$

In general neither $h=z/2$ nor $\theta=0$ is valid for the printed system.

The normalized formal [fundamental matrix](../../../../../fundamental-matrix-of-a-linear-differential-equation.md) is

$$
\boxed{\widehat Y=\left(I+\frac{G_1}{\lambda}+\frac{G_2}{\lambda^2}+\cdots\right)
\lambda^{\theta D}\exp\left[\left(\frac{\lambda^3}{3}+h\lambda\right)D\right],}
$$

with a chosen [logarithm](../../../../../logarithm.md) branch. In particular the diagonal normal form has $\Lambda_1=0$, $\Lambda_2=hD$, $\Lambda_3=\theta D$. Its first two prefactor coefficients are

$$
\boxed{G_1=\begin{pmatrix}\rho&-U/2\\V/2&-\rho\end{pmatrix},}
$$



$$
\boxed{G_2=\begin{pmatrix}
\rho^2/2-UV/8+h\theta/2&(U\rho-P)/2\\
(V\rho+R)/2&\rho^2/2-UV/8-h\theta/2
\end{pmatrix}.}
$$

These formulas include the diagonal terms required by the [derivative](../../../../../derivative.md) of the prefactor. Setting every diagonal prefactor coefficient to zero while retaining only the displayed exponent would generally fail the [differential equation](../../../../../differential-equation-split.md).

Here is the coefficient calculation and the full recursion. Write $A_1=\left(\begin{smallmatrix}0&U\\V&0\end{smallmatrix}\right)$, $A_2=\left(\begin{smallmatrix}d&P\\R&-d\end{smallmatrix}\right)$ and $G_0=I$, with negative-index $G_j=0$. Substitution into the [gauge transformation of a linear differential system](../../../../../gauge-transformation-of-a-linear-differential-system.md) gives, for $m\ge1$,

$$
[D,G_m]=-A_1G_{m-1}-A_2G_{m-2}+G_{m-2}hD
+G_{m-3}[\theta D-(m-3)I].
$$

At $m=1$, the [commutator](../../../../../commutator.md) determines $(G_1)_{12}=-U/2$, $(G_1)_{21}=V/2$ and the absence of a linear diagonal term. The diagonal part at $m=2$ gives $h=d+UV/2$. The next diagonal part gives $\theta=(UR+VP)/2$. At $m=4$ diagonal solvability gives $-\rho=PR/2-UV(d+h)/4$; the next order fixes the two diagonal entries of $G_2$ above. The off-diagonal entries are fixed at each stage because $[D,X]_{12}=2X_{12}$ and $[D,X]_{21}=-2X_{21}$. Later diagonal solvability fixes the remaining normalization coefficients. Thus this is a complete formal solution, not a convergence assertion. It is the [formal cubic-exponential two-by-two system](../../../../../formal-cubic-exponential-two-by-two-system.md) expansion. The printed hint's second prefactor term must have denominator $\lambda^2$, and the remainder after the $1/\lambda$ term of the diagonal expansion must start at $1/\lambda^2$.

Now impose an [isomonodromic deformation](../../../../../isomonodromic-deformation.md) in the full irregular sense: its [Stokes matrices](../../../../../stokes-matrix.md) and formal exponent are fixed in $z$, with the leading formal normalization fixed. Sectorial [matrices](../../../../../matrix.md) satisfy $Y_{j+1}=Y_jC_j$ with $(C_j)_z=0$, so $B_j=(Y_j)_zY_j^{-1}$ is the same on overlaps. Since the spectral system has no finite singularities, its [fundamental matrix](../../../../../fundamental-matrix-of-a-linear-differential-equation.md) and inverse are entire in $\lambda$, making $B$ entire. Differentiating the formal expression, using $\theta_z=0$, gives

$$
B=G_zG^{-1}+G(h_z\lambda D)G^{-1}
=h_z\lambda D+h_z[G_1,D]+O(\lambda^{-1}).
$$

But $[G_1,D]=A_1$. The sectorial cover makes this a global growth bound, so [Liouville's theorem](../../../../../liouville-theorem.md) applied to $B-h_z(\lambda D+A_1)$ gives the literal consequence

$$
\boxed{B=h_z\begin{pmatrix}\lambda&u\\-zw/u&-\lambda\end{pmatrix}.}
$$

An arbitrary parameter dependence of $u,w$ need not be isomonodromic; this analytic argument presupposes the stated constancy of generalized [monodromy](../../../../../monodromy.md) data.

The requested [matrix](../../../../../matrix.md) would require $h_z=1/2$ from its diagonal and upper entry, and then its lower entry would require $(z-2)w=0$. On an open deformation domain this forces $w\equiv0$. Thus that requested expression is not the general deformation [matrix](../../../../../matrix.md) for the printed coefficients.

There is a consistent nearby correction: replace the lower entry of $A_1$ by $-2w/u$. Then $V=-2w/u$, so $h=z/2$ and $\theta=0$, and the same derivation proves exactly

$$
\boxed{Y_z=\begin{pmatrix}\lambda/2&u/2\\-w/u&-\lambda/2\end{pmatrix}Y.}
$$

For this corrected system use the same prefactor formulas with $V=-2w/u$: $\rho=-w(w+z)/2-w(u'/u)^2$ and both diagonal entries of $G_2$ are $\rho^2/2+w/4$. Compatibility determines the allowed $u,w$ in the next solution. This correction is stated explicitly rather than silently substituting it for the original PDF.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
