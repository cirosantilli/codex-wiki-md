<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

With $Z[J]=e^{iW[J]}$, the logarithm $W$ is the [connected generating functional](../../../../../connected-generating-functional.md). Its derivative $\varphi=\delta W/\delta J$ is the mean field. The specified [Legendre transform](../../../../../convex-conjugate.md) satisfies $\delta\Gamma/\delta\varphi=J$, and the [quantum effective action](../../../../../effective-action.md) generates amputated [one-particle-irreducible vertices](../../../../../one-particle-irreducible-vertex.md) by further [functional derivatives](../../../../../functional-derivative.md). In this question $\Gamma=-W+\int J\varphi$ is the negative of the commonly used Minkowski effective-action convention; consequently its tree term is $-S[\varphi]$. Its diagrammatic content is unchanged if the convention is used consistently.

Expand the action around a stationary background in the presence of the source. For $\phi=\varphi+f$, [integration by parts](../../../../../integration-by-parts.md) gives

$$
S[\varphi+f]+\int J(\varphi+f)=S[\varphi]+\int J\varphi+\int\left(\frac{\delta S}{\delta\varphi}+J\right)f-\frac12\int f\Delta f+O(f^3),\qquad\Delta=-\partial^2+V''(\varphi).
$$

The linear term vanishes at the tree-level saddle, $\delta S/\delta\varphi+J=0$. Keeping the [Gaussian fluctuation approximation](../../../../../gaussian-fluctuation-approximation.md), and fixing the field-independent normalization, gives

$$
Z[J]\simeq e^{iS[\varphi]+i\int J\varphi}(\det\Delta_F)^{-1/2},\qquad W[J]=S[\varphi]+\int J\varphi+\frac i2\log\det\Delta_F
$$

to one-loop order. The shift from the tree saddle to the exact mean field cancels from the tree Legendre transform at this order. Hence the [one-loop scalar effective action](../../../../../one-loop-scalar-effective-action.md) in the question's convention is

$$
\boxed{\Gamma[\varphi]=-S[\varphi]+\frac1{2i}\log\det\Delta_F.}
$$

The [functional determinant](../../../../../functional-determinant.md) has a [Feynman i-epsilon prescription](../../../../../feynman-i-epsilon-prescription.md) before [Wick rotation](../../../../../wick-rotation.md). Higher loops come from the omitted cubic and higher fluctuation vertices.

To see the one-loop [one-particle-irreducible Feynman diagrams](../../../../../one-particle-irreducible-feynman-diagram.md), write $\Delta=\Delta_0+U(\varphi)$. Its determinant expansion is

$$
\operatorname{Tr}\log\Delta=\operatorname{Tr}\log\Delta_0+\sum_{r\ge1}\frac{(-1)^{r+1}}r\operatorname{Tr}\bigl[(\Delta_0^{-1}U)^r\bigr].
$$

Each trace closes a single scalar loop, with propagators $\Delta_0^{-1}$ and background insertions $U$. No internal edge is a bridge, so these graphs are [one-particle irreducible](../../../../../one-particle-irreducible-feynman-diagram.md). Expanding the background factors produces their external legs.

For a constant $\varphi$, set $A=V''(\varphi)>0$. The [quantum effective potential](../../../../../quantum-effective-potential.md) is defined here by $\Gamma[\varphi]=\int d^dx\,V_{\rm eff}(\varphi)$. A plane-wave basis diagonalizes $\Delta$, and the supplied [Wick rotation](../../../../../wick-rotation.md) converts its correction per unit volume to

$$
V_1(A)=\frac12\mu^\epsilon\int\frac{d^{4-\epsilon}k_E}{(2\pi)^{4-\epsilon}}\log(k_E^2+A)=-\frac{\mu^\epsilon\Gamma(-2+\epsilon/2)}{2(4\pi)^{2-\epsilon/2}}A^{2-\epsilon/2}.
$$

Here the power of the [renormalization scale](../../../../../renormalization-scale.md) keeps the continued integral in four-dimensional units. The [Gamma function recurrence](../../../../../gamma-function-recurrence.md) and expansion give

$$
\Gamma(-2+\epsilon/2)=\frac1\epsilon+\frac34-\frac\gamma2+O(\epsilon),\qquad A^{2-\epsilon/2}=A^2\left(1-\frac\epsilon2\log A+O(\epsilon^2)\right).
$$

Consequently

$$
V_1(A)=-\frac{A^2}{32\pi^2\epsilon}+\frac{A^2}{64\pi^2}\left(\log\frac A{\mu^2}-\frac32+\gamma-\log4\pi\right)+O(\epsilon).
$$

The divergence is local, so subtract it with a potential [counterterm](../../../../../counterterm.md). In the [modified minimal subtraction scheme](../../../../../modified-minimal-subtraction-scheme.md), remove its associated $\gamma-\log4\pi$ constants as well. The [one-loop scalar effective potential](../../../../../one-loop-scalar-effective-potential.md) becomes

$$
\boxed{V_{\rm eff}(\varphi)=V(\varphi)+\frac{[V''(\varphi)]^2}{64\pi^2}\left(\log\frac{V''(\varphi)}{\mu^2}-\frac32\right),}
$$

up to an arbitrary field-independent vacuum-energy constant. Another allowed finite subtraction replaces the nonlogarithmic constant. Restoring a loop-counting parameter would multiply the displayed correction by $\hbar$. The logarithm assumes positive curvature $A$; a background with negative curvature requires an analytic continuation and can have an imaginary part signalling instability.

The quartic case is special because of [quartic closure of scalar effective-potential counterterms](../../../../../quartic-closure-of-scalar-effective-potential-counterterms.md). If $V$ has degree at most four, then $V''$ has degree at most two and $(V'')^2$ has degree at most four: its pole is removable by the original polynomial couplings and a constant. For example, $V=m^2\varphi^2/2+\lambda\varphi^4/4!$ gives

$$
\frac{(V'')^2}{32\pi^2\epsilon}=\frac{m^4}{32\pi^2\epsilon}+\frac{\lambda m^2\varphi^2}{32\pi^2\epsilon}+\frac{\lambda^2\varphi^4}{128\pi^2\epsilon}.
$$

The last two terms reproduce the [one-loop massive phi-fourth counterterms](../../../../../one-loop-massive-phi-fourth-counterterms.md), and the first is a vacuum-energy subtraction. A degree-$r$ potential with $r>4$ instead generates degree $2r-4>r$, forcing new operators. This is the potential-level manifestation of [power counting in quantum field theory](../../../../../power-counting-in-quantum-field-theory.md) and four-dimensional [renormalizability](../../../../../renormalizable-quantum-field-theory.md), even though the finite effective potential itself need not remain polynomial.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
