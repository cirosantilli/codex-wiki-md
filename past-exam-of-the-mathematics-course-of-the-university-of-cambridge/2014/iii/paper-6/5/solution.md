<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [character of an algebra](../../../../../character-of-an-algebra.md) is a nonzero complex linear multiplicative map $\phi:A\to\mathbb C$. It necessarily satisfies $\phi(1)=1$. If $\lambda=\phi(x)$, then $x-\lambda1$ cannot be invertible, since applying $\phi$ to an inverse identity would give $0=1$. Therefore $\phi(x)\in\sigma(x)$. The [Neumann series](../../../../../neumann-series.md) bound $\sigma(x)\subseteq\{z:|z|\leq\|x\|\}$ gives

$$
\boxed{|\phi(x)|\leq\|x\|,}
$$

proving [automatic continuity of characters](../../../../../automatic-continuity-of-characters.md). In particular every [algebra character](../../../../../character-of-an-algebra.md) belongs to the closed [unit ball](../../../../../unit-ball.md) of $A^*$; no prior [continuity](../../../../../continuous-function.md) was needed.

The [character space of an algebra](../../../../../character-space-of-an-algebra.md) is $\Phi_A$, the set of all [algebra characters](../../../../../character-of-an-algebra.md). Its [Gelfand topology](../../../../../gelfand-topology.md) is the weakest topology making every evaluation $\phi\mapsto\phi(x)$ continuous, equivalently the [weak-star topology](../../../../../weak-star-topology.md) inherited from $A^*$. Within the weak-star compact ball $B_{A^*}$, it is the closed set specified by

$$
\phi(1)=1,\qquad\phi(ab)=\phi(a)\phi(b)\quad(a,b\in A).
$$

These equations are closed conditions on finitely many evaluations at a time. By the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md), **$\Phi_A$ is compact**, and it is Hausdorff because distinct characters differ on an evaluation.

To obtain every spectral value from a [algebra character](../../../../../character-of-an-algebra.md), take $\lambda\in\sigma(x)$. Commutativity makes the ideal $(x-\lambda1)A$ proper, so it is contained in an algebraic maximal ideal $\mathfrak m$. Every such maximal ideal is [norm](../../../../../norm.md) closed: its closure is an ideal, and cannot be all of $A$, because an element of $\mathfrak m$ sufficiently close to $1$ would be invertible by the [Neumann series](../../../../../neumann-series.md). Maximality then makes its closure equal to itself.

The quotient $A/\mathfrak m$ is a complex Banach division algebra, hence is $\mathbb C$ by the [Gelfand-Mazur theorem](../../../../../gelfand-mazur-theorem.md). Composing the quotient map with this scalar identification gives a [algebra character](../../../../../character-of-an-algebra.md) with $\phi(x)=\lambda$. Together with the first inclusion,

$$
\boxed{\sigma(x)=\{\phi(x):\phi\in\Phi_A\}.}
$$

The same maximal-ideal argument shows that the [algebra character](../../../../../character-of-an-algebra.md) space of a nonzero algebra is nonempty.

Now suppose $A$ is a commutative [C-star algebra](../../../../../c-star-algebra.md). All its elements are normal. The [C-star identity](../../../../../c-star-identity.md) gives

$$
\|x^2\|^2=\|(x^*)^2x^2\|=\|(x^*x)^2\|=\|x^*x\|^2=\|x\|^4,
$$

since the self-adjoint element $h=x^*x$ satisfies $\|h^2\|=\|h\|^2$. Iterating yields $\|x^{2^n}\|=\|x\|^{2^n}$. The [spectral radius formula](../../../../../spectral-radius-formula.md) along this subsequence proves

$$
\boxed{r(x)=\|x\|.}
$$

This is [spectral radius norm equality for normal elements](../../../../../spectral-radius-norm-equality-for-normal-elements.md), applied to the commutative case.

For a self-adjoint $h$, the element $v_t=\exp(ith)$ is unitary for every real $t$, so $\|v_t\|=1$. [Algebra character](../../../../../character-of-an-algebra.md) [continuity](../../../../../continuous-function.md) and multiplicativity give

$$
\phi(v_t)=\exp(it\phi(h)),\qquad|\exp(it\phi(h))|\leq1\quad(t\in\mathbb R).
$$

Its modulus is $\exp(-t\operatorname{Im}\phi(h))$, forcing $\phi(h)\in\mathbb R$. Write $x=h+ik$ with $h,k$ self-adjoint. Then

$$
\boxed{\phi(x^*)=\phi(h)-i\phi(k)=\overline{\phi(x)}.}
$$

This proves that [characters of a C-star algebra respect the involution](../../../../../characters-of-a-c-star-algebra-respect-the-involution.md). The conjugation bar is present in the original PDF and must be retained; the TeX aid omits it.

The [Commutative Gelfand--Naimark theorem](../../../../../commutative-gelfand-naimark-theorem.md) states that a complex commutative unital [C-star algebra](../../../../../c-star-algebra.md) is isometrically star-isomorphic to $C(K)$ for a compact Hausdorff space, canonically $K=\Phi_A$. Its [Gelfand transform](../../../../../gelfand-representation.md) is

$$
\mathcal G:A\longrightarrow C(\Phi_A),\qquad\widehat x(\phi)=\phi(x).
$$

It is a unital [algebra homomorphism](../../../../../algebra-homomorphism-over-a-field.md); the conjugation identity just proved makes it preserve the involution. The [algebra character](../../../../../character-of-an-algebra.md) description of the spectrum and the spectral-radius equality give

$$
\boxed{\|\widehat x\|_\infty=\sup_{\phi\in\Phi_A}|\phi(x)|=r(x)=\|x\|.}
$$

Thus it is injective and isometric, and its range is closed because $A$ is complete. The range contains constants, is closed under complex conjugation, and separates points of $\Phi_A$: two distinct [algebra characters](../../../../../character-of-an-algebra.md) differ on some element of $A$.

The complex [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) says that a self-adjoint unital subalgebra of $C(K)$ separating points is uniformly dense. For completeness, its familiar lattice argument explains the last step. The real part of its uniform closure is closed under absolute value, by polynomial approximation of $|t|$ on bounded real intervals, and hence under finite maxima and minima. Constants and point separation permit a real function matching any given real continuous $g$ at any chosen pair of points. Fixing the first point, take a maximum of finitely many such functions to obtain a function above $g-\varepsilon$ everywhere and equal to $g$ at that first point. It is below $g+\varepsilon$ in a neighborhood of that point. A finite cover by these neighborhoods and the minimum of their associated functions then lies between $g-\varepsilon$ and $g+\varepsilon$ everywhere. Real and imaginary parts give density for complex functions.

Apply this to $\mathcal G(A)$. Its range is both dense and closed, so it is all of $C(\Phi_A)$. Therefore

$$
\boxed{A\cong C(\Phi_A)\quad\text{as unital C-star algebras, isometrically}.}
$$

This proves the commutative theorem in the setting of the question. For the zero algebra the corresponding compact space is empty and the representation is $C(\varnothing)=\{0\}$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
