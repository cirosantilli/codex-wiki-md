<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

There is an important [chain rule](../../../../../../chain-rule.md) qualification in this part. The printed value of $\gamma$ follows from the expansion. Its printed value of $\alpha$ follows only if transverse differentiation of the translated correction profiles is omitted. For a consistent [translation-covariant phase expansion](../../../../../../translation-covariant-phase-expansion.md), that omission is generally nonzero.

At the leading transverse threshold let

$$
LC_1=2Bw_0',\qquad LC_2=2Bw_0'',\qquad
\langle w_0'C_j\rangle=0,
$$

where the last conditions fix the phase gauge. Put $p=\phi_Y$, $r_1=\phi_{YY}$, $s_1=\phi_{YYY}$ and $t_1=\phi_{YYYY}$, and use $w_2=C_1(\xi)r_1+C_2(\xi)p^2$. At order $\varepsilon^4$ the [Fredholm solvability condition](../../../../../../fredholm-solvability-condition.md) gives

$$
N\phi_T=\lambda N r_1
-2\langle w_0'B\mathcal D_Y^2w_2\rangle
-\langle w_0'\mathcal D_Y^4w_0\rangle
-3\langle w_0'w_0w_2^2\rangle.
$$

The first two contributions follow directly by differentiating:

$$
\begin{aligned}
\mathcal D_Y^2w_2={}&C_1t_1+2(C_1'+C_2)ps_1+(C_1'+2C_2)r_1^2
 +(C_1''+5C_2')p^2r_1+C_2''p^4,\\
\mathcal D_Y^4w_0={}&w_0't_1+w_0''(4ps_1+3r_1^2)+6w_0'''p^2r_1+w_0''''p^4.
\end{aligned}
$$

Choose the reflection-symmetric roll with $w_0$ even. Then $C_1$ is odd and $C_2$ even. Projection onto the odd translation mode eliminates $ps_1$, $r_1^2$ and $p^4$, leaving exactly the symmetry-allowed [phase modulation](../../../../../../phase-modulation.md) equation. Its coefficients are

$$
\boxed{\gamma=\frac{\langle w_0'(2C_1+2C_1''+w_0')\rangle}{N},}
$$

and

$$
\boxed{\alpha_{\rm cov}=
\frac{6\langle w_0'(w_0'''+w_0C_1C_2)\rangle
+2\langle w_0'B(C_1''+5C_2')\rangle}{N}.}
$$

If one freezes $C_j$ at the unshifted coordinate when taking transverse derivatives, $\partial_Y^2w_2=C_1t_1+2C_2(r_1^2+ps_1)$, and its projection contributes only the $\gamma$ term. The other two projected terms then give the **printed expression** $\alpha_{\rm print}=6\langle w_0'(w_0'''+w_0C_1C_2)\rangle/N$. But freezing these profiles is inconsistent with the translated $w_0$ in $L$ for a general finite phase displacement. The printed expression needs the extra assumption $\langle w_0'B(C_1''+5C_2')\rangle=0$, which is not an identity.

A small-amplitude calculation demonstrates the difference. For a critical roll of leading amplitude $\eta$ and fast [wavenumber](../../../../../../wavenumber.md) $\kappa$, the steady equation and $J=0$ give

$$
\begin{aligned}
w_0&=\eta\cos(\kappa\xi)-\frac{\eta^3}{256}\cos(3\kappa\xi)+O(\eta^5),\\
\kappa&=1-\frac{9\eta^4}{16384}+O(\eta^6),\qquad
r=\frac34\eta^2+O(\eta^4),\\
C_1&=\frac{3\eta^3}{1024}\sin(3\kappa\xi)+O(\eta^5),\\
C_2&=\frac{\eta^3}{1024}\big[-3\cos(\kappa\xi)+9\cos(3\kappa\xi)\big]+O(\eta^5).
\end{aligned}
$$

The third harmonic coefficient in $w_0$ follows by dividing its cubic forcing $-\eta^3\cos(3\kappa\xi)/4$ by the fast [eigenvalue](../../../../../../eigenvalue.md) $-64$. Substituting in $LC_j$ gives the displayed correction profiles; the near-zero first-harmonic [eigenvalue](../../../../../../eigenvalue.md) in the even problem must be retained to obtain the first harmonic of $C_2$. Periodic orthogonality then gives

$$
\langle w_0'B(C_1''+5C_2')\rangle
=\frac{243\eta^6}{32768}+O(\eta^8),\qquad
\alpha_{\rm cov}-\alpha_{\rm print}
=\frac{243\eta^4}{8192}+O(\eta^6).
$$

Thus the supplied nonlinear coefficient is not generally an exact consequence of the finite-amplitude translated-roll expansion. The corrected coefficient above, the printed calculation under its additional freezing assumption, and the genuine near-threshold [phase modulation](../../../../../../phase-modulation.md) equation are all distinguished explicitly.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
