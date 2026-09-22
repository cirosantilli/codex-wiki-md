<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Source correction:** equation 11 on the original page has $\Gamma(\alpha-1/2)$. The dimensionally regulated integral instead contains $\Gamma(\alpha-d/2)$. This is not an interchangeable convention: for $\alpha=2$ and $d=4-\epsilon$, the correct factor $\Gamma(\epsilon/2)$ has a logarithmic [ultraviolet pole](../../../../ultraviolet-pole.md), whereas the printed $\Gamma(3/2)$ is finite.

To obtain the correct expression, shift the [loop momentum](../../../../loop-momentum.md) and perform a [Wick rotation](../../../../wick-rotation.md). For positive Euclidean $\mathcal M^2$, introduce a [Schwinger parameterization](../../../../schwinger-parameterization.md):

$$
\begin{aligned}
\int\frac{d^dq_E}{(2\pi)^d}\frac1{(q_E^2+\mathcal M^2)^\alpha}
&=\frac1{\Gamma(\alpha)}\int_0^\infty ds\,s^{\alpha-1}e^{-s\mathcal M^2}
\int\frac{d^dq_E}{(2\pi)^d}e^{-sq_E^2}\\
&=\frac{\Gamma(\alpha-d/2)}{(4\pi)^{d/2}\Gamma(\alpha)}(\mathcal M^2)^{d/2-\alpha}.
\end{aligned}
$$

The derivation first holds in the convergent range and defines the result elsewhere by [analytic continuation](../../../../analytic-continuation.md). For integer $\alpha$, rotating back gives

$$
\boxed{\int\frac{d^dq}{(2\pi)^d}\frac1{(q^2+2q\cdot p-m^2+i0)^\alpha}
=\frac{i(-1)^\alpha}{(4\pi)^{d/2}}\frac{\Gamma(\alpha-d/2)}{\Gamma(\alpha)}
(p^2+m^2)^{d/2-\alpha},}
$$

with the branch inherited from $i0$. This is the Lorentzian continuation of the [Euclidean massive loop integral](../../../../euclidean-massive-loop-integral.md).

Set $p=0$, $\alpha=1$, $d=4-\epsilon$. Since $\Gamma(-1+\epsilon/2)=-2/\epsilon+O(1)$,

$$
\int_k\frac1{k^2-m^2+i0}=\frac{im^2}{8\pi^2\epsilon}+O(1).
$$

Consequently the directed tadpole in part d gives

$$
\left.i\Gamma^{(2)}_{\mathrm{loop}}\right|_{\mathrm{div}}
=(-ig\mu^\epsilon)\left.i\int_k\frac1{k^2-m^2+i0}\right|_{\mathrm{div}}
=\frac{igm^2}{8\pi^2\epsilon}.
$$

The [counterterm](../../../../counterterm.md) is $-i\delta_{m^2}$, so cancelling only the pole in the [minimal subtraction scheme](../../../../minimal-subtraction-scheme.md) requires

$$
\boxed{\delta_{m^2}=\frac{gm^2}{8\pi^2\epsilon}.}
$$

This is the [quartic complex-scalar mass renormalization](../../../../quartic-complex-scalar-mass-renormalization.md) result. The scale factors and logarithms contribute finite terms at this order and do not change the displayed pole coefficient. A real-field check gives a tadpole coefficient $\tfrac12(3g/2+g/2)=g$, in agreement with the oriented complex-field computation.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
