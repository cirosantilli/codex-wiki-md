<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

By the tip correspondence in the conjugacy,

$$
\xi_t^*=\Phi_t(\xi_t),\qquad \xi_t=\sqrt6\,B_t.
$$

The time-dependent [Itô formula](../../../../../../ito-s-lemma.md) is valid after localization away from the pole and the terminal time $S$. The map's time variation is of [finite variation](../../../../../../total-variation-of-a-function.md), so there is no extra stochastic cross-variation term. Using the supplied conjugacy [derivative](../../../../../../derivative.md),

$$
\begin{aligned}
d\xi_t^*&=\Phi_t'(\xi_t)\sqrt6\,dB_t
+\left(\dot\Phi_t(\xi_t)+3\Phi_t''(\xi_t)\right)dt\\
&=\sqrt6\,\Phi_t'(\xi_t)dB_t.
\end{aligned}
$$

Consequently

$$
\boxed{\xi_t^*\text{ is a continuous local martingale on }[0,S),\qquad
[\xi^*]_t=6u(t).}
$$

The cancellation is special to $\kappa=6$: for a general [SLE](../../../../../../schramm-loewner-evolution.md) parameter the drift would be $(\kappa/2-3)\Phi_t''(\xi_t)dt$. This is the [transformed SLE driving function](../../../../../../transformed-sle-driving-function.md), and explains the special [Locality property of SLE](../../../../../../locality-property-of-sle.md) at six.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
