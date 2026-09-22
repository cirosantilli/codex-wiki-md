<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $l(R)=R^2\Omega=\sqrt{GMR}$ be the Keplerian [specific angular momentum](../../../../../../specific-angular-momentum.md). In a source-free steady interval, the sum of advected and viscously transported angular momentum is constant:

$$
\dot m,l-2\pi R^3\nu\Sigma\frac{d\Omega}{dR}=C.
$$

Inside the injection radius, $\dot m=\dot m_0$. The [zero-torque inner boundary condition](../../../../../../zero-torque-inner-boundary-condition.md) at $R_{\rm ISCO}$ sets $C=\dot m_0l_{\rm ISCO}$, and therefore

$$
\boxed{\nu\Sigma=\frac{\dot m_0}{3\pi}
\left[1-\left(\frac{R_{\rm ISCO}}R\right)^{1/2}\right],
\qquad R<R_0.}
$$

Outside $R_0$ there is no net mass flow in the stated steady distribution, but it must carry outward the angular momentum deposited by matter moving from $R_0$ to the ISCO. Its constant [viscous torque in an accretion disk](../../../../../../viscous-torque-in-an-accretion-disk.md) is therefore

$$
3\pi\nu\Sigma l=\dot m_0(l_0-l_{\rm ISCO}).
$$

Thus

$$
\boxed{\nu\Sigma=\frac{\dot m_0}{3\pi}
\left[\left(\frac{R_0}R\right)^{1/2}
-\left(\frac{R_{\rm ISCO}}R\right)^{1/2}\right],
\qquad R>R_0.}
$$

The two expressions agree at $R_0$; the jump in mass flux there is exactly the injected rate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
