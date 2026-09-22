<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

Newton's equation and its energy [integral](../../../../../integral.md) are

$$
m\ddot x=-V'(x),\qquad \frac12m\dot x^2+V(x)=E.
$$

Thus

$$
T=\sqrt{2m}\int_{x_-}^{x_+}\frac{dx}{\sqrt{E-V(x)}}.
$$

Let $a=-V''(x_+^*)>0$. Near the maximum,

$$
V(x)=E^*-\frac a2(x-x_+^*)^2+O(|x-x_+^*|^3),
$$

and the nearby turning point has distance $\epsilon\sim\sqrt{2E^*\delta/a}$ from $x_+^*$. The singular part of the period is an $\operatorname{arcosh}$ [integral](../../../../../integral.md):

$$
\sqrt{2m}\sqrt{\frac2a}\int_\epsilon^c\frac{dy}{\sqrt{y^2-\epsilon^2}}
=\sqrt{\frac ma}\log(1/\delta)+O(1).
$$

Hence

$$
T=\sqrt{\frac m{-V''(x_+^*)}}\{\log(1/\delta)+O(1)\}.
$$

Physically, the limiting orbit approaches the [unstable equilibrium](../../../../../unstable-equilibrium.md) at the barrier top with vanishing speed and spends arbitrarily long there.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
