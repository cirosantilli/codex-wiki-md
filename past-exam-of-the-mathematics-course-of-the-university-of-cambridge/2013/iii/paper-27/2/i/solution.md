<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) with [Loewner driving function](../../../../../../loewner-driving-function.md) $\xi_t=\sqrt\kappa W_t$, and set $Z_t=g_t(z)-\xi_t=X_t+iY_t$. Before the [Loewner swallowing time](../../../../../../interior-point-swallowing-time-for-a-loewner-chain.md),

$$
dZ_t=\frac2{Z_t}\,dt-\sqrt\kappa\,dW_t.
$$

The upper-half-plane branch of the logarithm has imaginary part $h_t$. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
d\log Z_t=\frac{4-\kappa}{2Z_t^2}\,dt
-\frac{\sqrt\kappa}{Z_t}\,dW_t,
$$

and therefore the [SLE angle process](../../../../../../sle-angle-process.md) satisfies

$$
\boxed{dh_t=(\kappa-4)\frac{X_tY_t}{|Z_t|^4}\,dt
+\sqrt\kappa\,\frac{Y_t}{|Z_t|^2}\,dW_t.}
$$

At $\kappa=4$ the drift vanishes. Since $0<h_t<\pi$, the stopped [local martingale](../../../../../../local-martingale.md) is a true bounded [martingale](../../../../../../martingale-split.md), and the [SLE4 angle martingale](../../../../../../sle4-angle-martingale.md) is global for each fixed point almost surely, using [fixed-interior-point avoidance of SLE4](../../../../../../fixed-interior-point-avoidance-of-sle4.md) for the simple parameter-four [Loewner trace](../../../../../../trace-of-a-loewner-chain.md).

Conversely, take $\kappa>0$. If this [semimartingale](../../../../../../semimartingale.md) were a [local martingale](../../../../../../local-martingale.md), uniqueness of its finite-variation decomposition would force $(\kappa-4)X_tY_t=0$ throughout every compact interval before swallowing. Because $Y_t>0$, for $\kappa\ne4$ this would force $X_t$ to be identically zero on such an interval. Its Brownian component has [quadratic variation](../../../../../../quadratic-variation.md) $\kappa t$, which makes that impossible. Thus **for positive $\kappa$, the martingale parameter is exactly four**.

If the degenerate value $\kappa=0$ is admitted, there is one exception to a fixed-point reading of the assertion: for $z$ on the positive imaginary axis the deterministic flow stays on that axis until swallowing, and $h_t=\pi/2$ is constant. For all starting points simultaneously, the unique parameter giving the martingale property is still four.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
