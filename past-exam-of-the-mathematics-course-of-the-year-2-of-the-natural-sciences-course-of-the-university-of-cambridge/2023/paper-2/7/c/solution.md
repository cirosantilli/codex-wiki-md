<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the stated geometry and numerical masses, the inertia and [stiffness matrices](../../../../../stiffness-matrix.md) are

$$
M=\operatorname{diag}\left(2,\frac14,\frac2{25}\right),\qquad
K=\begin{pmatrix}5&-2&0\\-2&3&-1\\0&-1&1\end{pmatrix}.
$$

A [normal mode](../../../../../normal-mode.md) $\boldsymbol\theta=\mathbf v e^{i\omega t}$ requires $(K-\omega^2M)\mathbf v=0$. Writing $z=\omega^2$, its [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) is

$$
\det(K-zM)=-\frac{4z^3-108z^2+613z-600}{100}=0.
$$

At the claimed $z=6$, this determinant is $-27/50\ne0$. Hence **the printed claim that $\sqrt6$ is a normal frequency is false for the stated data**, and there is no corresponding nonzero [normal mode](../../../../../normal-mode.md).

The complete geometry-based answer is obtained from the three positive roots $z_j$:

$$
\boxed{\begin{aligned}
4z_j^3-108z_j^2+613z_j-600&=0,\\
(\omega_{\rm low},\omega_{\rm middle},\omega_{\rm high})
&\simeq(1.111471775,\ 2.491790287,\ 4.422172730).
\end{aligned}}
$$

An exact closed form for the squared [angular frequencies](../../../../../angular-frequency.md) is

$$
z_j=9+\sqrt{\frac{359}{3}}\cos\left[\frac13\arccos\frac{2745\sqrt3}{359^{3/2}}-\frac{2\pi j}{3}\right],\qquad j=0,1,2.
$$

They are approximately $19.555611657$, $6.209018836$ and $1.235369507$, respectively. For any of these roots, a corresponding [eigenvector](../../../../../eigenvector.md) can be chosen as

$$
\boxed{\mathbf v(z)=\begin{pmatrix}
\tfrac12\left[(3-z/4)(1-2z/25)-1\right]\\
1-2z/25\\
1
\end{pmatrix}.}
$$

The last two rows of $(K-zM)\mathbf v=0$ give this expression directly; the first is the characteristic equation. These three modes span all motion, with arbitrary sine and cosine amplitudes. Positivity of $M$ and of the spring [potential energy](../../../../../potential-energy.md) ensures that all squared [angular frequencies](../../../../../angular-frequency.md) are positive.

If instead one takes the PDF's printed $I_1=m_1a^2/6$ as a stipulated inertia, then $M=\operatorname{diag}(1/2,1/4,2/25)$ and

$$
\det(K-zM)=-\frac{2z^3-69z^2+626z-1200}{200}.
$$

The corresponding [angular frequencies](../../../../../angular-frequency.md) are approximately

$$
\boxed{(1.616170898,\ 3.315716400,\ 4.570997307).}
$$

The same formula for $\mathbf v(z)$ applies, because its derivation used only the second and third rows. Here the determinant at $z=6$ is $-63/25\ne0$, so following the printed inertia does not repair the frequency claim. The PDF therefore needs a further correction to its numerical data or asserted frequency; the intended correction cannot be inferred uniquely.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
