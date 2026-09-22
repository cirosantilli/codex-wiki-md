<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Set the renormalized $g_3$ to zero. For a six-scalar vertex, [b](../b.md) gives $\omega=-n_2$, so a new overall [logarithmic divergence](../../../../logarithmic-divergence.md) can only occur in graphs with $n_2=0$. With $b=6,f=0$, the line counts become $I_f=n_1$ and $I_b=n_1-3$, hence $L=n_1-2$.

At one loop this forces $n_1=3$ and $I_b=0$: the only candidate is a closed [triangle Feynman diagram](../../../../triangle-feynman-diagram.md) with two external scalar legs at each vertex. Its numerator at large [loop momentum](../../../../loop-momentum.md) is proportional to

$$
\operatorname{tr}[(\not k)^3]=k^2\operatorname{tr}(\not k)=0.
$$

This vanishes for the specified two-component [gamma matrices](../../../../gamma-matrices.md), each of which is traceless. Replacing one leading $\not k$ by the fermion mass or an external [momentum](../../../../momentum-split.md) lowers the [superficial degree of divergence](../../../../superficial-degree-of-divergence.md) from zero to at most $-1$. Thus the apparent logarithm cancels. Graphs with a $g_2$ vertex already have negative overall degree; the pure-scalar one-loop triangle, for instance, has $\omega=-3$. There is no one-loop [ultraviolet subdivergence](../../../../ultraviolet-subdivergence.md) inside these proper one-loop vertices. Therefore

$$
\boxed{\delta g_3^{\text{one loop}}=0.}
$$

The six-point [correlation function](../../../../correlation-function.md) need not vanish: finite terms are allowed. Nor is it correct to say that all odd [gamma-matrix traces](../../../../gamma-matrix-trace.md) vanish in $2+1$ dimensions. In this representation,

$$
\gamma^0\gamma^1\gamma^2=-iI_2,\qquad\operatorname{tr}(\gamma^0\gamma^1\gamma^2)=-2i\ne0.
$$

The cancellation above follows from repeating the same leading [loop momentum](../../../../loop-momentum.md), not from a false four-dimensional trace rule.

At two loops, $n_1=4$, $I_f=4$ and $I_b=1$ are possible. A closed fermion box with a scalar line joining two of its vertices leaves six external scalar legs. It has $L=2$, $\omega=0$, and four leading [gamma matrices](../../../../gamma-matrices.md); the one-loop odd-numerator argument no longer applies.

A background-field check demonstrates that its logarithm is actually nonzero. Put $\phi=v+\eta$ with constant $v$. Define the background fermion mass $\mu=m+g_1v^2/2$, the background scalar squared mass $\mathcal B^2=M^2+g_2v^2/2$, and the induced three-leg [Yukawa coupling](../../../../yukawa-interaction.md) $y=g_1v$. The two-loop [quantum effective potential](../../../../quantum-effective-potential.md) contains the [sunset diagram](../../../../sunset-diagram.md) with two fermion lines and one scalar line. After a [Wick rotation](../../../../wick-rotation.md), its relevant integral, apart from a nonzero overall combinatorial factor, is

$$
y^2\int\frac{d^3k\,d^3l}{(2\pi)^6}\frac{2(-k\cdot l+\mu^2)}{(k^2+\mu^2)(l^2+\mu^2)((k-l)^2+\mathcal B^2)}.
$$

Here the dots and [gamma-matrix traces](../../../../gamma-matrix-trace.md) are Euclidean. With $A=k^2+\mu^2$, $B=l^2+\mu^2$, $C=(k-l)^2+\mathcal B^2$, its numerator is exactly

$$
2(-k\cdot l+\mu^2)=-A-B+C+4\mu^2-\mathcal B^2.
$$

The first three terms reduce to products of one-loop [tadpole integrals](../../../../tadpole-integral.md), which have no logarithmic pole near three dimensions in [dimensional regularization](../../../../dimensional-regularization.md). The remaining term is

$$
y^2(4\mu^2-\mathcal B^2)H,\qquad H=\int\frac{d^3k\,d^3l}{(2\pi)^6}\frac1{ABC}.
$$

For positive regulator masses, the large-momentum region of $H$ has a positive, nonzero logarithmic divergence. One can see this directly by restricting the relative angles and the ratio $|k|/|l|$ to compact intervals away from zero: the remaining common radial integral is proportional to $\int^\Lambda dr/r$. Its proper one-loop subgraphs are ultraviolet convergent.

Finally, the coefficient multiplying $H$ contains

$$
y^2(4\mu^2-\mathcal B^2)=g_1^2v^2\left[4m^2- M^2+\left(4mg_1-\frac{g_2}{2}\right)v^2+g_1^2v^4\right].
$$

The [two-loop sextic counterterm in quartic Yukawa theory](../../../../two-loop-sextic-counterterm-in-quartic-yukawa-theory.md) follows because its $v^6$ coefficient is $g_1^4\ne0$ for a nonzero coupling. Other two-loop vacuum topologies reduce to products of finite-in-dimensional-regularization tadpoles and do not cancel this logarithmic pole. Thus

$$
\boxed{\delta g_3^{\text{two loops}}\ \text{is generically nonzero and proportional to }g_1^4.}
$$

A sextic [counterterm](../../../../counterterm.md) is required even if the renormalized sextic coupling is set to zero at a chosen [renormalization scale](../../../../renormalization-scale.md). A theory constrained to $g_3=0$ at every scale lacks [counterterm closure](../../../../counterterm-closure.md) when $g_1\ne0$. The decoupled exception $g_1=0$ is the three-dimensional scalar [quartic interaction](../../../../quartic-interaction.md), which needs no sextic [counterterm](../../../../counterterm.md) by [power counting](../../../../power-counting-in-quantum-field-theory.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
