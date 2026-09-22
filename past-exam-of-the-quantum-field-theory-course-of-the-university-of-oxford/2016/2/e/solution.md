<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [Heisenberg picture](../../../../heisenberg-picture.md) evolution of the [annihilation operator](../../../../annihilation-operator.md) follows from $[H,a_{\mathbf p}]=-E_{\mathbf p}a_{\mathbf p}$. With $p^0=E_{\mathbf p}$, this gives the [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md)

$$
\phi(x)=\int_{\mathbf p}\frac1{\sqrt{2E_{\mathbf p}}}
\left(a_{\mathbf p}e^{-ip\cdot x}+a^\dagger_{\mathbf p}e^{ip\cdot x}\right).
$$

Define $\Delta^+(z)=\int_{\mathbf p}e^{-ip\cdot z}/(2E_{\mathbf p})$. The [time-ordered product](../../../../time-ordered-product.md) then gives the [Feynman propagator](../../../../feynman-propagator.md)

$$
\Delta_F(z)=\theta(z^0)\Delta^+(z)+\theta(-z^0)\Delta^+(-z)
=\int\frac{d^4p}{(2\pi)^4}\frac{i\,e^{-ip\cdot z}}{p^2-m^2+i0}.
$$

The last expression follows by closing the $p^0$ [contour integral](../../../../contour-integral.md) below for $z^0>0$ and above for $z^0<0$; the [scalar Feynman propagator pole prescription](../../../../scalar-feynman-propagator-pole-prescription.md) supplies the required positive- and negative-frequency terms.

For $z^0\ne0$ every term obeys the homogeneous [Klein-Gordon equation](../../../../klein-gordon-equation.md). At $z^0=0$, the equal-time [commutator](../../../../commutator.md) of the [fields](../../../../field.md) vanishes, so the [propagator](../../../../propagator.md) is continuous and there is no derivative of a [Dirac delta function](../../../../dirac-delta-function.md). Its first time derivative has the jump

$$
\left[\partial_{z^0}\Delta_F\right]_{0^-}^{0^+}
=\int_{\mathbf p}(-i)e^{i\mathbf p\cdot\mathbf z}
=-i\delta^3(\mathbf z).
$$

The second time derivative therefore supplies precisely the source:

$$
\boxed{(\Box_x+m^2)\Delta_F(x-y)=-i\delta^4(x-y).}
$$

Thus the defined [Feynman propagator](../../../../feynman-propagator.md) is a [Green's function](../../../../green-s-function-split.md) with source normalization $-i$; $i\Delta_F$ has source normalization $+1$. Keeping this factor avoids confusing the [vacuum expectation value](../../../../vacuum-expectation-value.md) convention with conventions which define the [propagator](../../../../propagator.md) after dividing by $i$.[Sections 2.7.1–2.7.2, time ordering, pole prescription and the inhomogeneous Klein-Gordon equation](../../../../quantum-field-theory-by-david-tong.md)

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
