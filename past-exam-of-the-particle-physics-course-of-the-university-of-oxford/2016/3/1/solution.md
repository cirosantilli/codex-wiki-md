<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Strictly, it is the infinitesimal generators, not every [unitary matrix](../../../../unitary-matrix.md) with unit [determinant](../../../../determinant.md), that are traceless. For a continuous one-parameter family $U(\epsilon)=\exp(i\epsilon T)$, [unitarity](../../../../unitary-operator.md) requires the generator $T$ to be [Hermitian](../../../../hermitian-operator.md). The [determinant](../../../../determinant.md) condition gives

$$
1=\det U(\epsilon)=\exp\left(i\epsilon\operatorname{tr}T\right)\quad\hbox{for every real }\epsilon.
$$

Differentiating at $\epsilon=0$ yields $\operatorname{tr}T=0$. A [Hermitian matrix](../../../../hermitian-operator.md) has $n$ real diagonal parameters and $n(n-1)$ real off-diagonal parameters; one real trace constraint leaves $n^2-1$ independent generators. Thus

$$
\boxed{\dim SU(n)=n^2-1}.
$$

The identity matrix supplies a concrete counterexample to interpreting the claim as one about arbitrary group elements: $I_n\in SU(n)$ but $\operatorname{tr}I_n=n$. Also, $e^{i\operatorname{tr}T}=1$ at a single parameter value only fixes the trace modulo $2\pi$; the continuous neighbourhood is essential.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [3](../../3.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
