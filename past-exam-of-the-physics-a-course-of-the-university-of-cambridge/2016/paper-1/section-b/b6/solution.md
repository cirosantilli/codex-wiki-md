<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

For the oppositely travelling components, write $u=c_1e^{ikx}$ and $v=c_2e^{-ikx}$ after removing the common time phase. Then $\partial_x\psi=ik(u-v)e^{-i\omega t}$. In $\operatorname{Im}(\psi^*\partial_x\psi)$ the [interference](../../../../../interference-wave-propagation.md) terms contribute no imaginary part, so

$$
\boxed{J=\frac{\hbar k}{m}(|c_1|^2-|c_2|^2).}
$$

A standing-wave [interference](../../../../../interference-wave-propagation.md) pattern can therefore change density without adding a cross-term to the net current.

For **[barrier-top scattering](../../../../../barrier-top-scattering.md)**, the stationary equation inside the barrier is $-\hbar^2\psi_2''/(2m)=0$. Thus its spatial part is linear: $\psi_2=(bx+c)e^{-i\omega t}$. Take incident amplitude one, $k=\sqrt{2mE}/\hbar$ and $\omega=E/\hbar$. Continuity of the spatial [wave function](../../../../../wave-function-split.md) and its derivative at the two finite steps gives

$$
\begin{aligned}
e^{-ika}+re^{ika}&=-ab+c,& ik(e^{-ika}-re^{ika})&=b,\\
te^{ika}&=ab+c,& ikte^{ika}&=b.
\end{aligned}
$$

Solving these four equations yields

$$
\boxed{r=-\frac{ika\,e^{-2ika}}{1-ika},\qquad t=\frac{e^{-2ika}}{1-ika}.}
$$

The equal exterior velocities mean flux ratios are squared amplitude ratios:

$$
\boxed{T=|t|^2=\frac1{1+k^2a^2}=\left(1+\frac{2mEa^2}{\hbar^2}\right)^{-1},\qquad R=\frac{k^2a^2}{1+k^2a^2},\qquad R+T=1.}
$$

This is the threshold limit of finite-barrier scattering, not exponential decay with a nonzero interior decay constant.

The interior constants are

$$
\boxed{b=\frac{ik e^{-ika}}{1-ika},\qquad c=e^{-ika}.}
$$

Since $\operatorname{Im}[(bx+c)^*b]=\operatorname{Im}(c^*b)=k/(1+k^2a^2)$,

$$
\boxed{J_2=\frac{\hbar k/m}{1+k^2a^2}=J_{\rm incident}T.}
$$

It is positive and independent of [position](../../../../../position.md), matching the transmitted flux. Although the classical kinetic energy inside is zero, the complex linear quantum [wave function](../../../../../wave-function-split.md) carries conserved [probability current](../../../../../probability-current.md); its phase varies with [position](../../../../../position.md).

<a id="section-b/b6/image-at-the-barrier-top-energy-the-complex-amplitude-is-linear-while-its-probability-current-remains-constant"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1-barrier-top-current.png)

**[Figure 2](#section-b/b6/image-at-the-barrier-top-energy-the-complex-amplitude-is-linear-while-its-probability-current-remains-constant). At the barrier-top energy the complex amplitude is linear while its probability current remains constant**. [Source](paper-1-barrier-top-current.py).

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
