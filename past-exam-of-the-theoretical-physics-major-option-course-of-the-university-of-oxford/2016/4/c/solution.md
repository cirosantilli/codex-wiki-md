<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Integrate the two velocity factors over the time square $0\le s,s'\le t$. The [white noise](../../../../white-noise.md) contribution is $4Dt$. The orientation contribution depends only on the time separation, giving

$$
M(t)\equiv\langle|\mathbf r(t)-\mathbf r(0)|^2\rangle
=4Dt+2v^2\int_0^t(t-s)e^{-D_rs}\cos(\omega s)ds.
$$

This double-integral derivation fixes the delta contribution without ambiguity about a half-weight at an endpoint. Put $z=D_r-i\omega$. Elementary integration gives

$$
\boxed{M(t)=4Dt+2v^2\operatorname{Re}\left[\frac t z-\frac{1-e^{-zt}}{z^2}\right].}
$$

Using $\operatorname{Re}(1/z)=D_r/(D_r^2+\omega^2)$ and multiplying out the second term yields

$$
\boxed{\begin{aligned}
M(t)={}&4Dt+\frac{2v^2D_rt}{D_r^2+\omega^2}+\frac{2v^2(\omega^2-D_r^2)}{(D_r^2+\omega^2)^2}\\
&+\frac{2v^2e^{-D_rt}}{(D_r^2+\omega^2)^2}
\left[(D_r^2-\omega^2)\cos\omega t-2D_r\omega\sin\omega t\right].
\end{aligned}}
$$

The constant and decaying terms cancel at $t=0$, as required. The apparently singular case $D_r=\omega=0$ is evaluated from the integral, giving $M=4Dt+v^2t^2$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
