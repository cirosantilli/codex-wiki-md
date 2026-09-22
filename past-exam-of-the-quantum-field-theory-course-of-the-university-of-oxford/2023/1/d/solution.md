<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $I,L,V$ count internal lines, independent loops, and [interaction vertices](../../../../interaction-vertex.md) of a [connected Feynman diagram](../../../../connected-feynman-diagram.md). The graph identity $L=I-V+1$ and the two inverse powers from each [scalar propagator](../../../../scalar-propagator.md) give its [superficial degree of divergence](../../../../superficial-degree-of-divergence.md):

$$
\boxed{\omega=2L-2I=2(1-V).}
$$

The same formula applies to every connected subgraph. Graphs with $V\geq2$ have negative [superficial degree of divergence](../../../../superficial-degree-of-divergence.md), but this alone does not remove a possible [ultraviolet subdivergence](../../../../ultraviolet-subdivergence.md). A one-vertex subgraph with external legs in the [quartic scalar field theory](../../../../quartic-interaction.md) can diverge only by a [tadpole diagram](../../../../tadpole-diagram.md), whose subtraction was fixed in [c](../c.md). Subtract every such [tadpole diagram](../../../../tadpole-diagram.md); every remaining loop subgraph then has $V\geq2$ and negative [superficial degree of divergence](../../../../superficial-degree-of-divergence.md). Its [ultraviolet divergence](../../../../ultraviolet-divergence.md) is absent. Equivalently, [normal ordering](../../../../normal-ordering.md) the [quartic interaction](../../../../quartic-interaction.md) removes all self-contractions at a single [interaction vertex](../../../../interaction-vertex.md). Thus **no new divergent field-dependent counterterm structure is needed**, and in a [normal-ordering subtraction scheme in two dimensions](../../../../normal-ordering-subtraction-scheme-in-two-dimensions.md) the one-loop mass subtraction exhausts these divergent coefficients.

The literal assertion that there are no further [counterterm](../../../../counterterm.md) contributions in the [on-shell renormalization scheme](../../../../on-shell-renormalization-scheme.md) is stronger and generally false. A concrete counterexample is the two-loop [sunset diagram](../../../../sunset-diagram.md). After analytic continuation below its three-particle threshold, the magnitude of its [self-energy](../../../../self-energy.md) at $p^2=m^2$ contains the strictly positive finite integral

$$
\left|\Sigma_{\rm sunset}(m^2)\right|
=\frac{g_4^2}{6(4\pi)^2m^2}
\int_{x,y,z\geq0}dx\,dy\,dz\,
\frac{\delta(1-x-y-z)}{xy+xz+yz-xyz}>0
\quad(g_4\ne0).
$$

The integrable corners do not spoil convergence. Its nonzero value shifts the [pole mass](../../../../pole-mass.md), requiring an additional _finite_ [mass counterterm](../../../../mass-counterterm.md) if $m$ is to remain the exact [pole mass](../../../../pole-mass.md); its derivative can likewise change the [pole residue](../../../../pole-residue.md). These are compatible with the [power counting](../../../../power-counting-in-quantum-field-theory.md) result. If [vacuum diagrams](../../../../vacuum-feynman-diagram.md) are retained rather than divided out in normalized [correlation functions](../../../../correlation-function.md), a separate constant [vacuum energy](../../../../vacuum-energy.md) [counterterm](../../../../counterterm.md) is also required: the one-vertex double-loop [vacuum diagram](../../../../vacuum-feynman-diagram.md) is already divergent. The claim about the mass subtraction concerns field-dependent [counterterms](../../../../counterterm.md) and normalized [correlation functions](../../../../correlation-function.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
