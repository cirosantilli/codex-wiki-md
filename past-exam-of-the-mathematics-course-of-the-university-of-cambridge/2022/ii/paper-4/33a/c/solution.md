<h1 id="33a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The required dipole matrix element is

$$
\begin{aligned}
\langle k,-|x|0\rangle
&=2\sqrt{\frac K\pi}\int_0^\infty
x e^{-Kx}\sin(kx)\,dx\\
&=\frac{4Kk\sqrt{K/\pi}}{(K^2+k^2)^2},
\end{aligned}
$$

where differentiating the elementary Laplace integral for $\sin(kx)$ evaluates the last integral. Hence

$$
|\langle k,-|x|0\rangle|^2
=\frac{16K^3k^2}{\pi(K^2+k^2)^4}.
$$

Put $E_f=E_0+\hbar\omega>0$ and $k_f=\sqrt{2mE_f}/\hbar$. The [continuum transition probability at long times](../../../../../../continuum-transition-probability-at-long-times.md) uses

$$
\frac{\sin^2(\Omega_kt/2)}{(\Omega_k/2)^2}
\longrightarrow2\pi t\,\delta(\Omega_k).
$$

Since

$$
\delta(\Omega_k)
=\frac{m}{\hbar k_f}\delta(k-k_f),
$$

the total escape probability becomes

$$
\begin{aligned}
P_{\rm free}(t)
&=\int_0^\infty|c_k(t)|^2\,dk\\
&\sim\frac{2\pi F^2t}{\hbar^2}
\frac{m}{\hbar k_f}
\frac{16K^3k_f^2}{\pi(K^2+k_f^2)^4}\\
&=\frac{32F^2tmK^3k_f}
{\hbar^3(K^2+k_f^2)^4}.
\end{aligned}
$$

For the attractive [delta potential](../../../../../../delta-potential.md),

$$
|E_0|=\frac{\hbar^2K^2}{2m},
\qquad
\frac{k_f^2}{K^2}=\frac{E_f}{|E_0|}.
$$

Substitution gives the requested leading-order result:

$$
\boxed{
P_{\rm free}(t)
=\frac{8\hbar F^2t}{mE_0^2}
\frac{\sqrt{E_f/|E_0|}}
{(1+E_f/|E_0|)^4}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [33A](../../33a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
