<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let a connected amputated [one-particle-irreducible Feynman diagram](../../../../../../one-particle-irreducible-feynman-diagram.md) have $L$ loops, $I$ internal lines, $V$ quartic vertices and $E$ external legs. Each loop integration contributes four momentum powers, each [scalar propagator](../../../../../../scalar-propagator.md) removes two, and the interaction adds none. Thus its [superficial degree of divergence](../../../../../../superficial-degree-of-divergence.md) is $D=4L-2I$. Counting half-edges and independent loops gives

$$
4V=2I+E,\qquad L=I-V+1,
\qquad\boxed{D=4-E.}
$$

This is simultaneous large-momentum scaling of the whole [Feynman diagram](../../../../../../feynman-diagram.md). It need not describe every subregion of loop-momentum space.

For a concrete counterexample, start with a six-point triangle of three quartic vertices, with two external legs at each vertex. Insert a one-loop [tadpole diagram](../../../../../../tadpole-diagram.md) self-energy in one internal line. The resulting [Feynman diagram](../../../../../../feynman-diagram.md) has $V=4$, $I=5$, $L=2$, $E=6$, and $D=-2$. It is still one-particle irreducible: each edge around the triangle has an alternative route, and cutting the tadpole loop does not disconnect the [Feynman diagram](../../../../../../feynman-diagram.md). Nevertheless the tadpole subgraph diverges when its [loop momentum](../../../../../../loop-momentum.md) tends to infinity while the triangle momentum is held fixed. In massive theory the divergent mass insertion is nonzero. This demonstrates that [a superficially convergent graph can have a divergent subgraph](../../../../../../a-superficially-convergent-graph-can-have-a-divergent-subgraph.md).

Write renormalized perturbation theory with

$$
\mathcal L=\frac12(\partial\phi)^2-\frac12m^2\phi^2-\frac\lambda{4!}\phi^4
+\frac12\delta Z(\partial\phi)^2-\frac12\delta m^2\phi^2
-\frac{\delta\lambda}{4!}\phi^4+\delta\mathcal L_0.
$$

The last term is a field-independent vacuum [counterterm](../../../../../../counterterm.md), needed if vacuum energies are retained. A normalized correlation functional removes that sector. The free [quantum field theory propagator](../../../../../../propagator.md) is $i/(p^2-m^2+i0)$; interaction and [counterterm](../../../../../../counterterm.md) insertions use

$$
\boxed{\text{quartic vertex: }-i\lambda,\qquad
\text{four-point counterterm: }-i\delta\lambda,\qquad
\text{two-point counterterm: }i(\delta Zp^2-\delta m^2).}
$$

Usual momentum-conservation delta functions accompany the vertices. The coefficients depend on the regulator and [renormalization](../../../../../../renormalization.md) conditions and are expanded order by order in the renormalized coupling.

The reason this list closes is locality of ultraviolet subtraction. After divergent proper subgraphs have been subtracted recursively, the remaining overall divergent part is a polynomial in external momenta of degree at most $D$. For $E=2$, $D=2$, Lorentz symmetry allows only a constant and a $p^2$ term, supplied by the mass and wavefunction [counterterms](../../../../../../counterterm.md). For $E=4$, $D=0$, only the constant quartic [counterterm](../../../../../../counterterm.md) is needed. Odd-point terms vanish by the field's $\phi\mapsto-\phi$ symmetry. For $E>4$, the overall degree is negative and there is no new overall [counterterm](../../../../../../counterterm.md) after [subdivergences](../../../../../../ultraviolet-subdivergence.md) have been removed. Vacuum graphs are handled separately.

[Counterterm](../../../../../../counterterm.md) insertions subtract each subgraph's local divergence, including overlapping subgraphs, and then the overall divergence. At each perturbative order the regulated sum has a finite ultraviolet limit for renormalized [correlation functions](../../../../../../correlation-function.md) at suitable nonexceptional momenta. This is why superficial [power counting](../../../../../../power-counting-in-quantum-field-theory.md) of every relevant subgraph determines the allowed [counterterms](../../../../../../counterterm.md), even though it does not alone establish that a bare [Feynman diagram](../../../../../../feynman-diagram.md) diverges or converges. Possible infrared or on-shell singularities are a separate issue; ultraviolet [renormalization](../../../../../../renormalization.md) is not a promise of finiteness in every kinematic limit.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
