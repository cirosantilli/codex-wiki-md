<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First resolve the [orientation sign in quadrant harmonic spectral inversion](../../../../../../orientation-sign-in-quadrant-harmonic-spectral-inversion.md). The printed spectral definitions traverse the physical boundary clockwise, whereas both reconstruction rays run outward from zero. Integrating first in $k$ gives the kernel $i/(z-w)$. The resulting clockwise [Cauchy integral](../../../../../../cauchy-transform.md) is the negative of the desired [holomorphic function](../../../../../../holomorphic-function.md). Thus, with exactly the spectral definitions used above, the consistent reconstruction is

$$
q_z(z)=-\frac1{2\pi}\left[\int_0^\infty e^{ikz}\widehat q_2(k)\,dk+
\int_0^{i\infty}e^{ikz}\widehat q_1(k)\,dk\right].
$$

The printed plus sign would reconstruct $-q_z$. For a concrete nonzero example, $q(z)=-2\operatorname{Re}[(1+i)/(z+1+i)]$ is real, [harmonic](../../../../../../harmonic-function.md), smooth on the closed quadrant and decays along both axes. With $\beta_1=\beta_2=0$, it has $h_1(0)=h_2(0)=1$ and $q_z=(1+i)/(z+1+i)^2$. The printed orientation returns the negative of this [derivative](../../../../../../derivative.md), so the issue persists even under the stated corner condition.

Let $a=\tfrac12e^{-i\beta_1-i\gamma}$. In the expressions from the preceding part, the coefficient of $\Phi$ on the imaginary ray is $a$, and the coefficient on the real ray is $-a e^{4i\gamma}$. For each of the three allowed sums, $e^{4i\gamma}=1$. The unknown part is therefore proportional to

$$
\int_0^{i\infty}e^{ikz}\Phi(k)\,dk-\int_0^\infty e^{ikz}\Phi(k)\,dk=0.
$$

Indeed, close the first spectral quadrant. For $z=x+iy$ with $x,y>0$, $|e^{ikz}|=e^{-(x\operatorname{Im}k+y\operatorname{Re}k)}$, so the large-arc contribution vanishes for bounded $\Phi$. The [Cauchy integral theorem](../../../../../../cauchy-s-integral-theorem.md) proves the equality and eliminates the single unknown [function](../../../../../../function-split.md).

Substituting only the known pieces leaves

$$
q_z(z)=\frac1{2\pi}\left[
e^{i\beta_2}\int_0^\infty e^{ikz}H_2(k)\,dk
-e^{i\beta_2+i\gamma}\int_0^\infty e^{ikz}H_1(-k)\,dk
-e^{-i\beta_1}\int_0^{i\infty}e^{ikz}H_1(k)\,dk
+e^{-i\beta_1-i\gamma}\int_0^{i\infty}e^{ikz}H_2(-k)\,dk
\right].
$$

This already determines the answer from $h_1,h_2$ alone. Evaluating the elementary ray kernels gives the more direct [rational-angle oblique derivative problem on a quadrant](../../../../../../rational-angle-oblique-derivative-problem-on-a-quadrant.md) formula

$$
\boxed{\begin{aligned}
q_z(z)=\frac{i}{2\pi}\bigg[
&e^{i\beta_2}\int_0^\infty\frac{h_2(x)}{z-x}\,dx
+e^{-i\beta_1-i\gamma}\int_0^\infty\frac{h_2(x)}{z+x}\,dx\\
&-e^{-i\beta_1}\int_0^\infty\frac{h_1(y)}{z-iy}\,dy
-e^{i\beta_2+i\gamma}\int_0^\infty\frac{h_1(y)}{z+iy}\,dy
\bigg].
\end{aligned}}
$$

No denominator vanishes for an interior point of the first quadrant.

For explicit formulas in the three cases, define

$$
I_2(z)=\int_0^\infty\frac{h_2(x)}{z^2-x^2}\,dx,\qquad
I_1(z)=\int_0^\infty\frac{h_1(y)}{z^2+y^2}\,dy,
$$



$$
K_2(z)=\int_0^\infty\frac{x h_2(x)}{z^2-x^2}\,dx,\qquad
K_1(z)=\int_0^\infty\frac{y h_1(y)}{z^2+y^2}\,dy.
$$

Combining the paired fractions and using $\beta_2=\gamma-\beta_1$ yields

$$
\boxed{q_z(z)=\frac{e^{-i\beta_1}}{\pi}
\begin{cases}
iz[I_2(z)-I_1(z)],&\gamma=0,\\
K_1(z)-K_2(z),&\gamma=\pi/2,\\
-iz[I_2(z)+I_1(z)],&\gamma=\pi.
\end{cases}}
$$

There is also a necessary [corner compatibility for collinear oblique derivative data](../../../../../../corner-compatibility-for-collinear-oblique-derivative-data.md). When $\gamma=\pi/2$, the two prescribed [derivative](../../../../../../derivative.md) directions are opposites, so a continuous corner [gradient](../../../../../../gradient.md) requires $h_2(0)=-h_1(0)$. Together with the stipulated equality, this forces **$h_1(0)=h_2(0)=0$ in that case**. Existence was assumed, so admissible data must satisfy this additional consequence. Smoothness at the corner and decay at infinity also exclude the [homogeneous corner ambiguity in a quadrant Laplace problem](../../../../../../homogeneous-corner-ambiguity-in-a-quadrant-laplace-problem.md); no extra singular or growing term is permitted in the boxed reconstruction.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 86](../../../paper-86-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
