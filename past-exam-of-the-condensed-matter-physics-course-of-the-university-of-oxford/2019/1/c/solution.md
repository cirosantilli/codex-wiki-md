<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Translate the integration variable by an arbitrary [lattice vector](../../../../lattice-vector.md) and use the periodicity of $V$:

$$
V_{\mathbf q}=\int d^3x\,e^{i\mathbf q\cdot\mathbf x}V(\mathbf x)
=e^{i\mathbf q\cdot\mathbf R}\int d^3y\,e^{i\mathbf q\cdot\mathbf y}V(\mathbf y)
=e^{i\mathbf q\cdot\mathbf R}V_{\mathbf q}.
$$

Thus $(1-e^{i\mathbf q\cdot\mathbf R})V_{\mathbf q}=0$ for every $\mathbf R$. A nonzero coefficient requires $e^{i\mathbf q\cdot\mathbf R}=1$ for every lattice translation, which is precisely the defining condition for $\mathbf q\in\Lambda^*$.

For an infinite crystal the integral is a [Fourier transform of a periodic distribution](../../../../fourier-transform-of-a-periodic-distribution.md), rather than an ordinary convergent integral. More explicitly, the [Fourier series](../../../../fourier-series-split.md)

$$
V(\mathbf x)=\sum_{\mathbf G\in\Lambda^*}v_{\mathbf G}e^{-i\mathbf G\cdot\mathbf x},\qquad
v_{\mathbf G}=\frac1{\Omega_c}\int_{\mathrm{cell}}d^3x\,e^{i\mathbf G\cdot\mathbf x}V(\mathbf x)
$$

gives

$$
\boxed{V_{\mathbf q}=(2\pi)^3\sum_{\mathbf G\in\Lambda^*}v_{\mathbf G}\delta^{(3)}(\mathbf q-\mathbf G).}
$$

This is the precise meaning of zero away from the [reciprocal lattice](../../../../reciprocal-lattice.md). A finite specimen instead has broadened [reciprocal-lattice peaks of a finite crystal](../../../../reciprocal-lattice-peaks-of-a-finite-crystal.md); exact delta-function support is an infinite-periodicity idealization.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
