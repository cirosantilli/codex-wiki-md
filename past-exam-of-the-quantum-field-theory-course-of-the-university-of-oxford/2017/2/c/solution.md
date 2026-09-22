<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the amputated [one-particle-irreducible vertex](../../../../one-particle-irreducible-vertex.md), every internal bridge is forbidden. Define the [Feynman integrals](../../../../feynman-integral.md)

$$
D(k)=\frac{i}{k^2-m^2+i0},\qquad \int_k=\int\frac{d^dk}{(2\pi)^d},
$$



$$
I_2(P)=\int_kD(k)D(k+P),\qquad
I_3(P,Q,R)=\int_kD(k)D(k+P)D(k-R),\quad P+Q+R=0.
$$

For $E=3,L=1$, the counting identity in part b gives $V_3+2V_4=3$. The only [one-particle-irreducible Feynman diagrams](../../../../one-particle-irreducible-feynman-diagram.md) are a triangle of three cubic vertices and a two-propagator bubble joining one cubic and one quartic vertex. Write $\mathcal V_3$ for the amputated Feynman vertex, including its overall factor of $i$. With all external [momenta](../../../../momentum-split.md) incoming,

$$
\boxed{\mathcal V_{3,\,1\text{-loop}}(p_1,p_2,p_3)
=v_3^3 I_3(p_1,p_2,p_3)
+\frac{v_3v_4}{2}\sum_{i=1}^3 I_2(p_i).}
$$

The triangle has $S=1$ for labelled external legs. The mixed bubble has $S=2$ because its two internal lines may be interchanged. There are three distinct terms, according to which external leg is attached to the cubic vertex; the other two attach to the quartic vertex. No tadpole attached by a bridge is [one-particle irreducible](../../../../one-particle-irreducible-feynman-diagram.md).

The requested position-space three-point [correlation function](../../../../correlation-function.md) is obtained by restoring the external [propagators](../../../../propagator.md) and a [Fourier transform](../../../../fourier-transform-split.md):

$$
G^{(3)}_{\mathrm{1PI},\,1\text{-loop}}(x,y,z)
=\int_{p_1}\int_{p_2}\int_{p_3}(2\pi)^d\delta^d(p_1+p_2+p_3)
 e^{-i(p_1x+p_2y+p_3z)}D(p_1)D(p_2)D(p_3)
\mathcal V_{3,\,1\text{-loop}}.
$$

The tree-level contribution would replace the last factor by $v_3$. This explicitly distinguishes the amputated vertex from the [correlation function](../../../../correlation-function.md) while giving all loop integrations in [momentum](../../../../momentum-split.md) space.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
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
