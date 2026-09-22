<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Treat the Milky Way and M31 as a radial Kepler orbit of total mass $M$. At maximum separation $r=2a$ the radial speed vanishes, so conservation of energy gives

$$
\boxed{\frac12v^2-\frac{GM}{r}=-\frac{GM}{2a}}.
$$

Put $r=a(1-\cos2\eta)=2a\sin^2\eta$. Substitution into the energy equation and integration from the Big Bang gives the cycloidal orbit

$$
\boxed{2\eta-\sin2\eta=\left(\frac{GM}{a^3}\right)^{1/2}t}.
$$

Since $r^3=8a^3\sin^6\eta$,

$$
\boxed{\Omega t
=\sqrt{\frac{GM}{r^3}}\,t
=\frac{\eta-\sin\eta\cos\eta}{\sqrt2\,\sin^3\eta}}.
$$

Differentiating the parametric solution gives

$$
\boxed{\omega t=\frac vr\,t
=\frac{(\eta-\sin\eta\cos\eta)\cos\eta}{\sin^3\eta}}.
$$

Eliminating $\eta$ numerically gives the stated accurate fit

$$
\boxed{\Omega t+0.85\,\omega t=2^{-3/2}\pi}.
$$

A remote dwarf sees the Local Group primarily through its total monopole mass, so the same radial timing relation applies with its own $r_i,v_i$. Dimensional consistency requires

$$
\boxed{\Omega_i=\sqrt{\frac{GM}{r_i^3}}},
$$

rather than the cube-root exponent printed in the converted statement. Let $C=2^{-3/2}\pi$. At the zero-velocity radius $r_0$, $\omega_0=0$ and $\Omega_0t=C$. For the dwarf, $\Omega_it=C-0.85\,\omega_it$. Since $\Omega\propto r^{-3/2}$,

$$
\left(\frac{r_i}{r_0}\right)^{3/2}
=\frac{C}{C-0.85\,\omega_it}.
$$

Therefore

$$
\boxed{r_0=r_i\left[1-\frac{0.85}{2^{-3/2}\pi}\omega_it\right]^{2/3}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 346](../../../paper-346-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
