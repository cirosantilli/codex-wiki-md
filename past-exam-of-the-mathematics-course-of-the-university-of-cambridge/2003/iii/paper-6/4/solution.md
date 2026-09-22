<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $K=\sigma_A(x)$ and $R(\lambda)=(\lambda1-x)^{-1}$. Choose a bounded finite union of small polygonal regions $V$ with $K\subset V$, $\overline V\subset U$ and $\partial V\cap K=\varnothing$. Its positively oriented boundary cycle $\Gamma$ has winding number one on $K$ and zero outside $V$; boundaries of holes have negative orientation. Such regions can be obtained from a sufficiently fine grid around the compact set $K$. This accommodates disconnected spectra and neighborhoods with holes.

Define the [holomorphic functional calculus](../../../../../holomorphic-functional-calculus.md) by the norm-convergent contour integral

$$
\Theta_x(f)=\frac1{2\pi i}\int_\Gamma f(\lambda)R(\lambda)\,d\lambda.
$$

The integrand is continuous on a finite rectifiable cycle, so the integral exists in the [Banach space](../../../../../banach-space-split.md) $A$. Its value is independent of the chosen cycle: on $U\setminus K$ the integrand is holomorphic, and cycles with the stated winding numbers are homologous there. Apply the scalar [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) to every [bounded linear functional](../../../../../continuous-linear-functional.md) and then use the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) to recover equality of the algebra-valued integrals. Equivalently, a common refinement of the polygonal regions gives the same contour-deformation argument.

Linearity is immediate. For the [entire functions](../../../../../entire-function.md) $1,Z$, enlarge the integration cycle to a sufficiently large circle in the resolvent set, using their entire extension. Integrating the uniformly convergent [Neumann series](../../../../../neumann-series.md) term by term gives

$$
\Theta_x(1)=1,\qquad \Theta_x(Z)=x.
$$

To prove multiplicativity, choose two nested admissible cycles, $\Gamma_o$ outside $\Gamma_i$, both surrounding $K$ and lying in $U$. The [resolvent identity](../../../../../resolvent-identity.md) gives

$$
R(\lambda)R(\mu)=\frac{R(\mu)-R(\lambda)}{\lambda-\mu}.
$$

Use $\Gamma_o$ for $f$ and $\Gamma_i$ for $g$, multiply the two integrals, and insert this identity. In the term with $R(\mu)$, the outer [Cauchy integral formula](../../../../../cauchy-integral-formula.md) replaces $f(\lambda)/(\lambda-\mu)$ by $f(\mu)$. In the term with $R(\lambda)$, the inner integral of $g(\mu)/(\lambda-\mu)$ is zero because $\lambda$ is outside the inner region. Thus

$$
\Theta_x(f)\Theta_x(g)=\frac1{2\pi i}\int_{\Gamma_i}f(\mu)g(\mu)R(\mu)\,d\mu=\Theta_x(fg).
$$

The exchanges of integrals are justified by continuous integrands on compact separated cycles. This proves the unital algebra-homomorphism property, not just an identity of [algebra character](../../../../../character-of-an-algebra.md) values.

For continuity in [local uniform convergence](../../../../../locally-uniform-convergence.md), fix one cycle and bound

$$
\|\Theta_x(f)\|\leq\frac{\operatorname{length}\Gamma}{2\pi}\sup_\Gamma\|R(\lambda)\|\,\sup_\Gamma|f(\lambda)|.
$$

The last supremum is a defining compact-set [seminorm](../../../../../seminorm.md) of $\mathcal O(U)$. Hence the map is continuous.

If another continuous unital [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md) $\Psi$ sends $Z$ to $x$, its values on polynomials are forced. For every $\zeta\notin U$, the function $(Z-\zeta)^{-1}$ exists in $\mathcal O(U)$, so multiplicativity forces

$$
\Psi((Z-\zeta)^{-1})=(x-\zeta1)^{-1}.
$$

Therefore $\Psi$ and $\Theta_x$ agree on all rational functions with poles outside $U$. The permitted [Runge theorem](../../../../../runge-s-theorem.md) makes these functions dense in $\mathcal O(U)$ for [local uniform convergence](../../../../../locally-uniform-convergence.md), including when $U$ is disconnected. Continuity makes the maps agree everywhere. Thus

$$
\boxed{\Theta_x\text{ is the unique continuous unital algebra homomorphism with }\Theta_x(Z)=x}.
$$

This proves the [continuity and uniqueness of holomorphic functional calculus](../../../../../continuity-and-uniqueness-of-holomorphic-functional-calculus.md) with the exact topology required.

For an [algebra character](../../../../../character-of-an-algebra.md) $\phi$, multiplicativity and nonzeroness give $\phi(1)=1$. An invertible element cannot have zero [algebra character](../../../../../character-of-an-algebra.md) value, so $\phi(x)\in\sigma_A(x)$. The same observation for each algebra element and the spectral bound from Question 3 gives $|\phi(b)|\leq\|b\|$; thus a [algebra character](../../../../../character-of-an-algebra.md) is automatically a [bounded linear functional](../../../../../continuous-linear-functional.md). In particular,

$$
\phi(R(\lambda))=\frac1{\lambda-\phi(x)}.
$$

Apply $\phi$ inside the contour integral and use the [Cauchy integral formula](../../../../../cauchy-integral-formula.md) with winding number one at $\phi(x)$:

$$
\boxed{\phi(\Theta_x(f))=f(\phi(x))}.
$$

No separation of algebra elements by [algebra characters](../../../../../character-of-an-algebra.md) is used; such separation can fail for a general commutative [Banach algebra](../../../../../banach-algebra-split.md).

For the final clause, the two closed spectral pieces $X,Y$ are compact and have positive distance. Choose disjoint open neighborhoods $U_X,U_Y$ and let $f$ be identically one on $U_X$ and zero on $U_Y$. This locally constant function is holomorphic on their union, and $f^2=f$. Set $e=\Theta_a(f)$. Multiplicativity gives $e^2=e$, and the proved [algebra character](../../../../../character-of-an-algebra.md) formula gives

$$
\boxed{\phi(e)=\begin{cases}1,&\phi(a)\in X,\\0,&\phi(a)\in Y.\end{cases}}
$$

This is the [spectral idempotent from a separated spectrum](../../../../../spectral-idempotent-from-a-separated-spectrum.md). It is also nontrivial without assuming that [algebra characters](../../../../../character-of-an-algebra.md) separate points. If $e=0$, choose $\lambda\in X$ and define $g=0$ on $U_X$, $g(z)=1/(z-\lambda)$ on $U_Y$. Then $(Z-\lambda)g=1-f$, so $(a-\lambda1)\Theta_a(g)=1$, with commuting factors, making $a-\lambda1$ invertible despite $\lambda\in\sigma_A(a)$. This is impossible. If $e=1$, exchange the two pieces and use $\lambda\in Y$ for the analogous contradiction. Hence $e\ne0,1$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
