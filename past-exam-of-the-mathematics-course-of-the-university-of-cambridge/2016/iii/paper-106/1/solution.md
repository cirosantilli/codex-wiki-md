<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**Invertibility is stable under sufficiently small perturbations, and inversion is continuous.** Let $1$ be the identity of the complex unital [Banach algebra](../../../../../banach-algebra-split.md) $A$, with its submultiplicative [algebra norm](../../../../../algebra-norm.md). For $\|h\|<1$, completeness makes the [Neumann series](../../../../../neumann-series.md)

$$
(1-h)^{-1}=\sum_{n=0}^{\infty}h^n
$$

converge in $A$. Multiplying either side of the partial sums by $1-h$ gives $1-h^{N+1}$, which tends to $1$, proving that the sum is a two-sided inverse.

Fix $a\in G(A)$, the [group of invertible elements of a Banach algebra](../../../../../group-of-invertible-elements-of-a-banach-algebra.md). If $\|b-a\|<\|a^{-1}\|^{-1}$, then

$$
b=a(1+a^{-1}(b-a)),\qquad \|a^{-1}(b-a)\|<1,
$$

so the [Neumann series](../../../../../neumann-series.md) makes $b$ invertible. This proves that $G(A)$ is open. It also gives a local bound

$$
\|b^{-1}\|\le\frac{\|1\|\,\|a^{-1}\|}{1-\|a^{-1}\|\|b-a\|}.
$$

We retain $\|1\|$ here so the estimate does not silently assume a normalized identity. The inverse identity

$$
b^{-1}-a^{-1}=b^{-1}(a-b)a^{-1}
$$

then implies

$$
\|b^{-1}-a^{-1}\|\le\|b^{-1}\|\|b-a\|\|a^{-1}\|\longrightarrow0\quad(b\to a).
$$

This proves [continuity of inversion in a Banach algebra](../../../../../continuity-of-inversion-in-a-banach-algebra.md).

For a unital [Banach algebra](../../../../../banach-algebra-split.md), the [spectrum of an element](../../../../../spectrum-of-an-element.md) is

$$
\sigma_A(x)=\{\lambda\in\mathbb C:\lambda1-x\notin G(A)\}.
$$

For a nonunital [Banach algebra](../../../../../banach-algebra-split.md), use its [unitization of an algebra](../../../../../unitization-of-an-algebra.md) $A^+=A\oplus\mathbb C$ with multiplication and norm

$$
(a,\lambda)(b,\mu)=(ab+\lambda b+\mu a,\lambda\mu),\qquad
\|(a,\lambda)\|=\|a\|+|\lambda|.
$$

It is a unital [Banach algebra](../../../../../banach-algebra-split.md), with identity $(0,1)$, and define $\sigma_A(x)=\sigma_{A^+}((x,0))$. In this nonunital convention, $0$ belongs to the [spectrum](../../../../../spectrum-functional-analysis.md): the scalar coordinate of $(x,0)$ is zero, so it cannot be invertible in $A^+$.

**The spectrum is nonempty and compact.** It suffices to work in a nonzero unital [Banach algebra](../../../../../banach-algebra-split.md), since [unitization](../../../../../unitization-of-an-algebra.md) reduces the other case to this one. The [group of invertible elements of a Banach algebra](../../../../../group-of-invertible-elements-of-a-banach-algebra.md) is open, so the complement of the [spectrum of an element](../../../../../spectrum-of-an-element.md) is open. For $|\lambda|>\|x\|$, the [Neumann series](../../../../../neumann-series.md) gives

$$
R(\lambda)=(\lambda1-x)^{-1}=\frac1\lambda\sum_{n=0}^{\infty}\left(\frac{x}{\lambda}\right)^n,
\qquad
\|R(\lambda)\|\le\frac{\|1\|}{|\lambda|-\|x\|}.
$$

Thus $\sigma_A(x)$ is closed and lies in $\{\lambda:|\lambda|\le\|x\|\}$, hence is compact.

For [nonemptiness of the Banach-algebra spectrum](../../../../../nonemptiness-of-the-banach-algebra-spectrum.md), suppose that $R$ were defined on all of $\mathbb C$. At any $\lambda_0$, factoring $\lambda1-x=(\lambda_01-x)(1+(\lambda-\lambda_0)R(\lambda_0))$ gives a locally convergent power series

$$
R(\lambda)=\sum_{n=0}^{\infty}(-1)^n(\lambda-\lambda_0)^nR(\lambda_0)^{n+1}.
$$

For every [bounded linear functional](../../../../../continuous-linear-functional.md) $\ell\in A^*$, the scalar function $\ell(R(\lambda))$ is therefore [entire](../../../../../entire-function.md). The bound at infinity makes it bounded outside a disk, while continuity makes it bounded on the disk. By the [Liouville theorem](../../../../../liouville-theorem.md), it is constant; since it tends to zero at infinity, it is identically zero. The version of the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) used here says that [bounded linear functionals](../../../../../continuous-linear-functional.md) separate points of a [normed vector space](../../../../../normed-vector-space.md): if $z\ne0$, there is $\ell$ with $\ell(z)\ne0$. Consequently $R(\lambda)=0$ for every $\lambda$, contradicting $(\lambda1-x)R(\lambda)=1$. This proves the assertion.

**Every nonzero complex unital normed division algebra is algebraically and topologically isomorphic to $\mathbb C$.** This is the [Gelfand-Mazur theorem](../../../../../gelfand-mazur-theorem.md); completeness is not needed in its statement. Let $D$ be a [normed division algebra](../../../../../normed-division-algebra.md), and take its [completion of a normed space](../../../../../completion-of-a-normed-space.md) using the [algebra norm](../../../../../algebra-norm.md) to obtain a unital [Banach algebra](../../../../../banach-algebra-split.md) $\widehat D$. Submultiplicativity extends multiplication continuously to the completion, and the original identity remains its identity.

For $x\in D$, the [spectrum of an element](../../../../../spectrum-of-an-element.md) of $x$ in $\widehat D$ contains some $\lambda$. If $x-\lambda1\ne0$ in $D$, the division-algebra assumption supplies an inverse in $D$, which is still an inverse in $\widehat D$. This contradicts $\lambda\in\sigma_{\widehat D}(x)$. Therefore $x=\lambda1$. The map $\lambda\mapsto\lambda1$ is a bijective complex algebra homomorphism, and

$$
\|\lambda1\|=|\lambda|\|1\|.
$$

It and its inverse are continuous; when $\|1\|=1$, it is an [isometry](../../../../../isometry.md).

**A complete algebra norm on a function algebra dominates the supremum norm, even before continuity of point evaluations is known.** Let $A$ be the given algebra of functions. Form the same artificial [unitization](../../../../../unitization-of-an-algebra.md) $A^+$ even if $A$ already has an identity. For each $t\in K$, the algebraic map

$$
\chi_t:A^+\to\mathbb C,\qquad\chi_t(f,\lambda)=f(t)+\lambda
$$

is a unital multiplicative complex [linear functional](../../../../../linear-functional.md). No continuity has been assumed. Since $\chi_t(f-f(t)1)=0$, the element $f-f(t)1$ cannot be invertible: applying $\chi_t$ to an inverse equation would give $0=1$. Hence $f(t)\in\sigma_{A^+}(f)$, and the [spectrum](../../../../../spectrum-functional-analysis.md) bound already proved yields

$$
|f(t)|\le\|f\|\quad(t\in K).
$$

Taking the supremum proves the [supremum bound for a complete function-algebra norm](../../../../../supremum-bound-for-a-complete-function-algebra-norm.md):

$$
\boxed{\sup_{t\in K}|f(t)|\le\|f\|.}
$$

In particular every $f$ is bounded, and every point evaluation is a [bounded linear functional](../../../../../continuous-linear-functional.md) of norm at most $1$. This is an instance of [automatic continuity of characters](../../../../../automatic-continuity-of-characters.md): a [character of an algebra](../../../../../character-of-an-algebra.md) on a [Banach algebra](../../../../../banach-algebra-split.md) is bounded because its value at any element belongs to that element's [spectrum](../../../../../spectrum-functional-analysis.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
