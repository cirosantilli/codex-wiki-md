<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Gelfand-Mazur theorem](../../../../../gelfand-mazur-theorem.md) says that a nonzero complex unital [Banach algebra](../../../../../banach-algebra-split.md) in which every nonzero element is invertible is the complex field itself: $a\mapsto\lambda$ where $a=\lambda1$. This is an isometric isomorphism under the usual normalization $\|1\|=1$; without that normalization its norm is simply $\|\lambda1\|=|\lambda|\|1\|$. We first prove the required spectral and resolvent facts rather than assume them.

For any element $a$ of a complex unital [Banach algebra](../../../../../banach-algebra-split.md) $A$, define its [spectrum of an element](../../../../../spectrum-of-an-element.md) by

$$
\sigma_A(a)=\{\lambda\in\mathbb C:\lambda1-a\text{ is not invertible}\}.
$$

If $\|b\|<1$, the partial sums of $\sum_{n\ge0}b^n$ converge in the complete algebra. Multiplying a partial sum by $1-b$ on either side gives $1-b^{N+1}\to1$, proving the [Neumann series](../../../../../neumann-series.md) inverse. For $|\lambda|>\|a\|$ this gives

$$
R(\lambda,a)=(\lambda1-a)^{-1}=\sum_{n=0}^\infty\frac{a^n}{\lambda^{n+1}}.
$$

Thus the spectrum is bounded. Under $\|1\|=1$, $\|R(\lambda,a)\|\le(|\lambda|-\|a\|)^{-1}$; for an unnormalized identity the same estimate with numerator $\|1\|$ suffices. Also $\lambda R(\lambda,a)\to1$ as $|\lambda|\to\infty$.

If $\lambda_0$ is outside the spectrum and $R_0=R(\lambda_0,a)$, then for $|h|\|R_0\|<1$,

$$
R(\lambda_0+h,a)=\sum_{n=0}^\infty(-h)^nR_0^{n+1}.
$$

This follows by factoring $(\lambda_0+h)1-a=(\lambda_0 1-a)(1+hR_0)$ and applying the just-proved series. The series converges locally in norm, proving that the resolvent set is open, the spectrum is closed, and the [resolvent of an element](../../../../../resolvent-of-an-element.md) is holomorphic. Subtracting inverse equations also gives the [resolvent identity](../../../../../resolvent-identity.md)

$$
R(\lambda,a)-R(\mu,a)=(\mu-\lambda)R(\lambda,a)R(\mu,a),
$$

consistent with the derivative $R'(\lambda,a)=-R(\lambda,a)^2$ from the local series.

The spectrum is nonempty. If it were empty, the resolvent would be an entire algebra-valued function tending to zero at infinity. Choose a [bounded linear functional](../../../../../continuous-linear-functional.md) $\ell:A\to\mathbb C$ with $\ell(1)=1$, extending the functional on $\mathbb C1$ by the complex [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). Then $\ell(R(\lambda,a))$ is an [entire function](../../../../../entire-function.md), bounded outside a disk by the Neumann estimate and bounded inside by continuity and compactness. The [Liouville theorem](../../../../../liouville-theorem.md) makes it constant, and its decay makes that constant zero. But $\lambda\ell(R(\lambda,a))\to\ell(1)=1$, a contradiction. We have proved that every spectrum is a nonempty compact subset of the disk $|\lambda|\le\|a\|$.

Now assume every nonzero element of $A$ is invertible. For any $a$, choose $\lambda\in\sigma_A(a)$. The noninvertible element $a-\lambda1$ must be zero. Thus every element is a scalar multiple of the identity, uniquely because $1\ne0$, and

$$
\boxed{A=\mathbb C1\cong\mathbb C.}
$$

No commutativity assumption was needed for this part; it is forced by the conclusion. Complex scalars are essential to the spectral argument.

For the [maximal ideal space](../../../../../maximal-ideal-space-of-a-commutative-banach-algebra.md) and its correspondence with [characters of an algebra](../../../../../character-of-an-algebra.md), now take $A$ to be a commutative complex unital [Banach algebra](../../../../../banach-algebra-split.md). Every proper ideal lies in an algebraic [maximal ideal](../../../../../maximal-ideal.md) by [Zorn's lemma](../../../../../zorn-s-lemma.md): a chain's union is an ideal not containing $1$. Every proper ideal also has proper closure. Otherwise it contains an element $m$ with $\|1-m\|<1$, which is invertible by the Neumann series, forcing the ideal to contain $1$. A maximal ideal $I$ is therefore closed, since its closure is a proper ideal containing it.

The quotient $A/I$, with its quotient norm, is a complex [Banach algebra](../../../../../banach-algebra-split.md). Completeness follows from closedness of $I$, and submultiplicativity follows by taking infima over representatives. It is a division algebra: if $a\notin I$, maximality gives $I+Aa=A$, so $ba+i=1$ for some $b\in A$, $i\in I$. Hence $a+I$ is invertible. By the proved [Gelfand-Mazur theorem](../../../../../gelfand-mazur-theorem.md), $A/I\cong\mathbb C$, with the identity mapping to $1$. Composing this isomorphism with the quotient map produces a nonzero multiplicative complex [linear functional](../../../../../linear-functional.md) $\phi_I$ with kernel $I$.

Conversely let $\phi:A\to\mathbb C$ be a nonzero multiplicative complex linear functional, without assuming continuity. Nonzeroness and multiplicativity give $\phi(1)=1$, hence $\phi(\lambda1)=\lambda$ and surjectivity onto $\mathbb C$. Its kernel is a maximal ideal. If $a-\phi(a)1$ were invertible, applying $\phi$ to its product with an inverse would give $0=1$. Therefore $\phi(a)\in\sigma_A(a)$, so

$$
|\phi(a)|\le\|a\|.
$$

This proves [automatic continuity of characters](../../../../../automatic-continuity-of-characters.md); with normalized identity their [operator norm](../../../../../operator-norm.md) is one. Finally a kernel determines its character uniquely: for every $a$, its class in $A/I=\mathbb C1$ is a unique scalar multiple of the unit, and every character with kernel $I$ must take that scalar value. We have obtained the bijection

$$
\boxed{\{\text{maximal ideals of }A\}\longleftrightarrow\{\text{nonzero multiplicative complex linear functionals on }A\},\quad I\leftrightarrow\phi_I.}
$$

The commutativity in this correspondence cannot be dropped: $\operatorname{Mat}_2(\mathbb C)$ has the maximal two-sided ideal $0$, but has no scalar-valued character, since such a character would have zero kernel and give an impossible injective linear map into $\mathbb C$.

For use in the next question, the [spectrum equals character values in a commutative Banach algebra](../../../../../spectrum-equals-character-values-in-a-commutative-banach-algebra.md). We have proved one inclusion. For the other, if $a-\lambda1$ is noninvertible, its generated ideal is proper, hence lies in a maximal ideal. The corresponding character takes $a$ to $\lambda$. Thus

$$
\sigma_A(a)=\{\phi(a):\phi\in\mathcal M_A\}.
$$

Give $\mathcal M_A$ the [Gelfand topology](../../../../../gelfand-topology.md), namely the [weak-star topology](../../../../../weak-star-topology.md) of pointwise convergence on $A$ through these characters. It is Hausdorff and compact: the characters lie in the dual unit ball and form a weak-star closed subset, described by the closed equations $\phi(1)=1$ and $\phi(ab)=\phi(a)\phi(b)$. Apply the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md). The [Gelfand transform](../../../../../gelfand-representation.md) $a\mapsto\widehat a$, where $\widehat a(\phi)=\phi(a)$, is consequently a contractive unital algebra homomorphism into $C(\mathcal M_A)$; it separates distinct characters. This argument proves compactness and continuity, but does not assert injectivity or isometry for an arbitrary Banach algebra.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
