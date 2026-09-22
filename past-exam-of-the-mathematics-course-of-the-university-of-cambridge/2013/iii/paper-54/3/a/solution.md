<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The conventional complete-flyby [impulse approximation](../../../../../../impulse-approximation.md) uses a straight incoming path $x=x_0$, $y=-Sx_0t$, with $S>0$. Integrate the satellite's transverse acceleration over the whole encounter. For $x_0>0$,

$$
\Delta v_x=-\frac{GM_s}{x_0^2}\int_{-\infty}^{\infty}(1+S^2t^2)^{-3/2}dt
=-\frac{2GM_s}{Sx_0^2}.
$$

The hint's integral is one over a half encounter, and two over the full encounter. The leading longitudinal impulse vanishes by oddness. In weak elastic scattering, conservation of the relative speed $V=S|x_0|$ gives the next-order change along the original [velocity](../../../../../../velocity.md) as $-\Delta v_x^2/(2V)$. With the original outer flow along negative $y$, this means

$$
\boxed{\Delta v_y\simeq\frac{2(GM_s)^2}{S^3x_0^5}.}
$$

The same signed expression holds for inner particles and has the opposite sign there. This is the [complete-flyby gravitational impulse](../../../../../../complete-flyby-gravitational-impulse.md). Its weak-deflection requirement is $GM_s/(S^2|x_0|^3)\ll1$. Rotation and tidal dynamics retained throughout the encounter give a more detailed response; this impulse model does not claim to solve the full Hill scattering problem exactly.

The printed coefficient $1/2$ is four times smaller than this complete-flyby value. It is obtained if the single-sided transverse impulse $GM_s/(Sx_0^2)$ is inserted into the same quadratic longitudinal estimate, leaving out the other half. Thus the scaling and sign agree, but that numerical coefficient is not derived by the usual full-encounter prescription. To keep the subsequent requested formulas unambiguous, write the [satellite impulse normalization](../../../../../../satellite-impulse-normalization.md)

$$
\Delta v_y=\chi\frac{(GM_s)^2}{S^3x_0^5}:
\qquad\chi=\tfrac12\ \text{for the supplied model},\quad\chi=2\ \text{for the complete-flyby model}.
$$

The following parts are derived for general $\chi$ and specialize to the supplied value. The complete-flyby one-sided [torque](../../../../../../torque.md) coefficient $8/27$ is also the normalization used in [the primary coplanar impulse calculation summarized by Chametla and collaborators](https://academic.oup.com/mnras/article/468/4/4610/3098191).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
