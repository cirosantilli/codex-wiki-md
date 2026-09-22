<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Give $\mathcal O(U)$ the [compact-open topology](../../../../../compact-open-topology.md), that is, uniform convergence on every compact subset of $U$. Choose a bounded finite union of polygonal domains $D$ whose closure lies in $U$, whose interior contains $\sigma(x)$ and whose boundary avoids the spectrum. Orient its boundary $\Gamma$ positively, with holes oriented negatively. It has winding number one on the spectrum and zero outside $U$. For the [resolvent of an element](../../../../../resolvent-of-an-element.md) $R(\zeta,x)=(\zeta1-x)^{-1}$ define the [holomorphic functional calculus](../../../../../holomorphic-functional-calculus.md) by

$$
\boxed{\Theta_x(f)=\frac1{2\pi i}\int_\Gamma f(\zeta)R(\zeta,x)d\zeta.}
$$

This is an integral of a continuous [Banach space](../../../../../banach-space-split.md)-valued function. Its value is independent of the admissible contour: the integrand is holomorphic away from the spectrum, and the difference of two such cycles has winding number zero there, so the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) applies. The vector-valued theorem follows by applying bounded linear functionals and then the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md).

Linearity is immediate. To prove multiplicativity, choose two admissible contours with the inner domain compactly contained in the outer one, and use the [resolvent identity](../../../../../resolvent-identity.md)

$$
R(\zeta,x)R(\eta,x)=\frac{R(\zeta,x)-R(\eta,x)}{\eta-\zeta}.
$$

In the double integral for $\Theta_x(f)\Theta_x(g)$, integrate the first term in the outer variable $\eta$. The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) gives $g(\zeta)$. For the second term, integration of $f(\zeta)/(\eta-\zeta)$ over the inner contour is zero, since $\eta$ lies outside that inner domain. Therefore the double integral equals $\Theta_x(fg)$. The continuous integrands on disjoint compact contours justify exchanging the integrals.

For $f=1$ and $f=Z$, deform to a large circle and use the [Neumann series](../../../../../neumann-series.md) $R(\zeta,x)=\sum_{m\geq0}x^m\zeta^{-m-1}$. Its relevant coefficients give $\Theta_x(1)=1$ and $\Theta_x(Z)=x$. The estimate

$$
\|\Theta_x(f)\|\leq\frac{\operatorname{length}(\Gamma)}{2\pi}\sup_\Gamma\|R(\zeta,x)\|\sup_\Gamma|f|
$$

proves continuity in the stated topology.

For uniqueness, the [Runge approximation theorem](../../../../../runge-s-theorem.md) in the required form says that rational functions with poles outside $U$, allowing a pole at infinity, are dense in $\mathcal O(U)$ for uniform convergence on compact subsets. Every complex-linear unital homomorphism taking $Z$ to $x$ has prescribed values on polynomials and on $(Z-a)^{-1}$ for $a\notin U$: the latter value must be $(x-a1)^{-1}$. Hence its rational-function values are prescribed. Continuity and Runge approximation force its values on every holomorphic function. This proves [continuity and uniqueness of holomorphic functional calculus](../../../../../continuity-and-uniqueness-of-holomorphic-functional-calculus.md), including disconnected $U$.

To prove the [spectral mapping theorem](../../../../../spectral-mapping-theorem.md), first suppose $\mu\notin f(\sigma(x))$. On a smaller open neighborhood $U'$ of the spectrum, $f-\mu$ has no zeros, so $h=1/(f-\mu)$ is holomorphic there. The contour definition is compatible with this restriction. Multiplicativity gives $\Theta_x(f)-\mu1$ the inverse $\Theta_x(h)$, excluding $\mu$ from its spectrum.

Conversely, if $\mu=f(\lambda)$ for $\lambda\in\sigma(x)$, write $f(z)-\mu=(z-\lambda)g(z)$, defining $g(\lambda)=f'(\lambda)$ at its removable singularity. Then

$$
\Theta_x(f)-\mu1=(x-\lambda1)\Theta_x(g).
$$

These two factors commute. An invertible product of commuting elements makes each factor invertible, by multiplying the inverse of the product by the other factor. That would contradict $\lambda\in\sigma(x)$. Thus

$$
\boxed{\sigma(\Theta_x(f))=f(\sigma(x)).}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
