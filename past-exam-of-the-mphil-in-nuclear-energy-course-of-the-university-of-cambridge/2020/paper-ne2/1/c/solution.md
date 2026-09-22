<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two outward surface normals point in opposite directions. With positive [heat flux](../../../../../heat-flux-density.md) defined as heat leaving each face, [Fourier's law](../../../../../fourier-s-law.md) gives

$$
q''_{\rm left}=kT'(0),\qquad q''_{\rm right}=-kT'(a).
$$

Using the derivative from part(a), **the removed fluxes per unit face area** are

$$
\boxed{q''_{\rm left}=\frac{q_0}{\mu}\left[1-\frac{1-e^{-\mu a}}{\mu a}\right]
=\frac{q_0}{\mu}(1-C),}
$$



$$
\boxed{q''_{\rm right}=\frac{q_0}{\mu}\left[\frac{1-e^{-\mu a}}{\mu a}-e^{-\mu a}\right]
=\frac{q_0}{\mu}(C-e^{-\beta}).}
$$

Both are positive because $e^{-\beta}<C<1$. Their sum satisfies the independent [conservation of energy](../../../../../conservation-of-energy.md) check

$$
q''_{\rm left}+q''_{\rm right}
=\frac{q_0}{\mu}(1-e^{-\mu a})
=\int_0^a q_0e^{-\mu x}\,dx.
$$

The illuminated face removes more [heat](../../../../../heat-split.md) because heating is concentrated nearer it. Equivalently, weighting each source slice by the fraction of its heat conducted to either equal-temperature boundary gives

$$
q''_{\rm left}=\int_0^a q'''(x)\frac{a-x}{a}\,dx,
\qquad
q''_{\rm right}=\int_0^a q'''(x)\frac{x}{a}\,dx.
$$

A decreasing source weights the left face more strongly. In the uniform-heating limit, **each face removes $q_0a/2$**. If a heat removal rate rather than a flux is wanted, multiply the relevant expression by the face area.

## ↑ Ancestors (10)

1. [C](../c.md)
2. [1](../../1.md)
3. [Module NE2](../../../paper-ne2-split.md)
4. [2020](../../../split.md)
5. [Past exam of the MPhil in nuclear energy course of the University of Cambridge](../../../../split.md)
6. [MPhil in nuclear energy course of the University of Cambridge](../../../../../mphil-in-nuclear-energy-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
