<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $K=\sigma_A(x)$ and $R_x(\zeta)=(\zeta1-x)^{-1}$. Suppose first that a unital complex-algebra homomorphism sends $Z$ to $x$. If $\lambda\notin U$, the [holomorphic function](../../../../../holomorphic-function.md) $1/(Z-\lambda)$ belongs to $\mathcal O(U)$ and is the multiplicative inverse of $Z-\lambda$. Its image is an inverse for $x-\lambda1$. Thus **existence forces $K\subset U$**, even before continuity is used.

For the converse, assume $K\subset U$. Choose a bounded finite union of polygonal regions $V$ with $K\subset V$, $\overline V\subset U$, and boundary avoiding $K$. Orient its boundary cycle $\Gamma$ positively around $V$, including negative orientations on holes. Its winding number is one near $K$ and zero outside $U$. Define

$$
\boxed{\Theta_x(f)=\frac1{2\pi i}\int_\Gamma f(\zeta)R_x(\zeta)\,d\zeta.}
$$

The integral exists in $A$ because the integrand is continuous on finitely many compact contour pieces. The [Cauchy theorem](../../../../../cauchy-s-integral-theorem.md) shows it is unchanged by replacing $\Gamma$ with another such spectral cycle: the difference has zero winding around the possible singularities in $K$. Banach-valued Cauchy statements follow by applying [bounded linear functionals](../../../../../continuous-linear-functional.md). We use the scalar [Cauchy integral formula](../../../../../cauchy-integral-formula.md) in its cycle form: a cycle with index one at a point and surrounding only a holomorphy region integrates $f(\zeta)/(\zeta-z)$ to $2\pi i f(z)$.

Linearity is immediate and, for a fixed cycle,

$$
\|\Theta_x(f)\|\le\frac{\operatorname{length}\Gamma}{2\pi}
\max_\Gamma\|R_x(\zeta)\|\,\sup_\Gamma|f|.
$$

This is a bound by one compact-uniform seminorm, proving continuity for [local uniform convergence](../../../../../locally-uniform-convergence.md). To obtain $\Theta_x(1)=1$, deform the resolvent integral, which is holomorphic on $\mathbb C\setminus K$, to a large circle and integrate its [Neumann series](../../../../../neumann-series.md). Similarly $\zeta R_x(\zeta)=1+xR_x(\zeta)$ gives $\Theta_x(Z)=x$.

For multiplicativity choose an outer spectral cycle for $f$ and an inner one for $g$, nested in $U$ so the inner cycle lies inside the outer region. The [resolvent identity](../../../../../resolvent-identity.md) is

$$
R_x(\zeta)R_x(\eta)=\frac{R_x(\eta)-R_x(\zeta)}{\zeta-\eta}.
$$

Substitute it into the double integral for $\Theta_x(f)\Theta_x(g)$. In the term containing $R_x(\eta)$, first integrate $f(\zeta)/(\zeta-\eta)$ around the outer cycle, obtaining $f(\eta)$. In the term containing $R_x(\zeta)$, first integrate $g(\eta)/(\zeta-\eta)$ around the inner cycle, obtaining zero because $\zeta$ lies outside it. Interchange is valid for the continuous integrands on disjoint compact cycles. Hence

$$
\Theta_x(f)\Theta_x(g)=\Theta_x(fg).
$$

This proves the required continuous unital homomorphism, the [holomorphic functional calculus](../../../../../holomorphic-functional-calculus.md).

For uniqueness use the following version of the allowed [Runge theorem](../../../../../runge-s-theorem.md): on any open $U\subseteq\mathbb C$, [rational functions](../../../../../rational-function.md) with all finite poles outside $U$ approximate each [holomorphic function](../../../../../holomorphic-function.md) locally uniformly; poles at infinity are allowed, giving [polynomials](../../../../../polynomial-split.md). A unital homomorphism sending $Z$ to $x$ is forced on [polynomials](../../../../../polynomial-split.md) and on every inverse $(Z-\lambda)^{-1}$, $\lambda\notin U$, and hence on these [rational functions](../../../../../rational-function.md). Continuity then forces its value on their limits. Thus **$\Theta_x$ is unique**. This argument works for disconnected $U$ as well and does not assume [polynomials](../../../../../polynomial-split.md) alone are dense. It proves [continuity and uniqueness of holomorphic functional calculus](../../../../../continuity-and-uniqueness-of-holomorphic-functional-calculus.md).

We will use the character description of [spectra](../../../../../spectrum-functional-analysis.md), with a short justification. A [character of an algebra](../../../../../character-of-an-algebra.md) $\varphi$ is a nonzero complex multiplicative [linear functional](../../../../../linear-functional.md); it satisfies $\varphi(1)=1$. Applying it to an inverse shows $\varphi(a)\in\sigma_A(a)$, so $|\varphi(a)|\le\|a\|$ and the character is automatically continuous. Conversely, for noninvertible $a-\lambda1$, its [principal ideal](../../../../../principal-ideal.md) is proper because $A$ is commutative. Put it in a [maximal ideal](../../../../../maximal-ideal.md) $M$. The closure of $M$ is proper: an ideal containing an element sufficiently close to one contains an invertible element and thus the identity. Maximality makes $M$ closed. The quotient is a complex Banach division algebra. By the nonempty-spectrum result of Question 3, each quotient element differs from some scalar by a noninvertible element, which in a division algebra must be zero. Thus the quotient is $\mathbb C$ and its quotient map is a character taking $a$ to $\lambda$. This proves

$$
\sigma_A(a)=\{\varphi(a):\varphi\text{ a character of }A\}.
$$

It is the [spectrum equals character values in a commutative Banach algebra](../../../../../spectrum-equals-character-values-in-a-commutative-banach-algebra.md) statement and does not assume semisimplicity.

For any character, continuity permits passing it inside the contour integral. Since $\varphi(R_x(\zeta))=(\zeta-\varphi(x))^{-1}$ and $\varphi(x)\in K$, the scalar Cauchy formula gives

$$
\boxed{\varphi(\Theta_x(f))=\frac1{2\pi i}\int_\Gamma
\frac{f(\zeta)}{\zeta-\varphi(x)}\,d\zeta=f(\varphi(x)).}
$$

Apply the character description first to $\Theta_x(f)$ and then to $x$ to obtain the [holomorphic spectral mapping theorem](../../../../../holomorphic-spectral-mapping-theorem.md)

$$
\boxed{\sigma_A(\Theta_x(f))=f(\sigma_A(x)).}
$$

On $\Pi_+$, use the analytic logarithm with argument in $(-\pi/2,\pi/2)$ and set $s(z)=\exp(\tfrac12\operatorname{Log} z)$. It satisfies $s(z)^2=z$ and takes its values in $\Pi_+$. The [principal square root in a commutative Banach algebra](../../../../../principal-square-root-in-a-commutative-banach-algebra.md) is

$$
\boxed{y=\Theta_x(s),\qquad y^2=x,\qquad\sigma_A(y)\subset\Pi_+.}
$$

For uniqueness let $v$ be another root with [spectrum](../../../../../spectrum-functional-analysis.md) in $\Pi_+$. For each character, $\varphi(y)$ and $\varphi(v)$ are scalar roots of $\varphi(x)$ with positive real part, so both equal $s(\varphi(x))$. Hence every character takes the nonzero value $2s(\varphi(x))$ at $y+v$. The character description implies $y+v$ is invertible. Commutativity gives $(y-v)(y+v)=y^2-v^2=0$, and multiplying by the inverse yields $y=v$. Equal character values alone would not imply equality in a possibly nonsemisimple algebra; the invertible sum is the essential extra step.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
