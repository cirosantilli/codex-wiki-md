<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**The first assertion needs the [C-star identity](../../../../../c-star-identity.md); a Banach-algebra involution alone is insufficient.** For an explicit counterexample, take the [dual-number algebra](../../../../../dual-number.md)

$$
B=\mathbb C[\varepsilon]/(\varepsilon^2),\qquad
\|a+b\varepsilon\|=|a|+|b|,\qquad
(a+b\varepsilon)^*=\bar a+\bar b\varepsilon.
$$

This is a commutative unital [Banach algebra](../../../../../banach-algebra-split.md), since it is finite-dimensional and

$$
\|(a+b\varepsilon)(c+d\varepsilon)\|=|ac|+|ad+bc|
\le(|a|+|b|)(|c|+|d|).
$$

Its involution is conjugate-linear, multiplicative, involutive and isometric. Every [character of an algebra](../../../../../character-of-an-algebra.md) kills $\varepsilon$, because $\phi(\varepsilon)^2=0$. Thus there is just one character, $a+b\varepsilon\mapsto a$, and the [Gelfand transform](../../../../../gelfand-representation.md) sends the nonzero norm-one element $\varepsilon$ to zero. It is neither injective nor norm preserving. In particular $\|\varepsilon^*\varepsilon\|=0\ne\|\varepsilon\|^2$, identifying the missing norm axiom.

Even the claimed compatibility with the involution is not automatic. On $\mathbb C^2$ with the maximum norm and pointwise multiplication, define $(a,b)^*=(\bar b,\bar a)$. This is another isometric involution, but evaluation at the first coordinate takes $(1,0)^*$ to zero rather than to the conjugate of its value $1$ at $(1,0)$. These examples establish [involution alone does not imply an isometric Gelfand transform](../../../../../involution-alone-does-not-imply-an-isometric-gelfand-transform.md).

We now prove the intended assertion for a commutative complex unital [C-star algebra](../../../../../c-star-algebra.md). Let $\mathcal M$ be its [maximal ideal space](../../../../../maximal-ideal-space-of-a-commutative-banach-algebra.md), identified with the compact [character space of an algebra](../../../../../character-space-of-an-algebra.md) as in Question 3. The C-star identity and submultiplicativity give

$$
\|a\|^2=\|a^*a\|\le\|a^*\|\|a\|,
$$

and applying the same inequality to $a^*$ proves $\|a^*\|=\|a\|$. Thus the involution is continuous. For a self-adjoint element $h$, the exponential series defines $u_t=\exp(ith)$ in norm. Applying the involution term by term gives $u_t^*=\exp(-ith)$, and multiplying the absolutely convergent series shows $u_t^*u_t=1$. Hence $\|u_t\|=1$. Every [character of an algebra](../../../../../character-of-an-algebra.md) is contractive by Question 3, and so

$$
|e^{it\phi(h)}|=|\phi(u_t)|\le1\qquad(t\in\mathbb R).
$$

Taking both signs of $t$ forces $\phi(h)$ to be real. Writing

$$
a=h+ik,\qquad h=(a+a^*)/2,\qquad k=(a-a^*)/(2i),
$$

with $h,k$ self-adjoint, proves

$$
\boxed{\widehat{a^*}=\overline{\widehat a}.}
$$

This proves that [characters of a C-star algebra respect the involution](../../../../../characters-of-a-c-star-algebra-respect-the-involution.md).

To prove the norm assertion, we also justify the [spectral radius formula](../../../../../spectral-radius-formula.md) used here. Put $r(a)=\max_{\lambda\in\sigma(a)}|\lambda|$. By [spectrum equals character values in a commutative Banach algebra](../../../../../spectrum-equals-character-values-in-a-commutative-banach-algebra.md),

$$
r(a)^n=\sup_{\phi\in\mathcal M}|\phi(a^n)|\le\|a^n\|.
$$

For $R>\|a\|$, integrating the uniformly convergent Neumann series on $|z|=R$ gives

$$
a^n=\frac1{2\pi i}\int_{|z|=R}z^n(z1-a)^{-1}\,dz.
$$

Only the coefficient of $z^{-1}$ survives. The resolvent is holomorphic outside the spectrum by Question 3, so the [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) deforms this contour to any circle of radius $R>r(a)$. For algebra-valued integrals the same identity follows by applying every bounded linear functional and then using Hahn-Banach separation. Taking norms gives

$$
\|a^n\|\le R^{n+1}\max_{|z|=R}\|(z1-a)^{-1}\|.
$$

The maximum is finite by resolvent continuity on the circle. Taking $n$th roots and then $R\downarrow r(a)$ proves $\lim_n\|a^n\|^{1/n}=r(a)$.

Every element is normal because $B$ is commutative. For self-adjoint $h$, the C-star identity gives $\|h^2\|=\|h\|^2$. Therefore, for arbitrary $a$,

$$
\|a^2\|^2=\|(a^2)^*a^2\|=\|(a^*a)^2\|=\|a^*a\|^2=\|a\|^4.
$$

Iterating yields $\|a^{2^n}\|^{1/2^n}=\|a\|$, so the proved spectral radius formula gives

$$
\boxed{\|\widehat a\|_\infty=r(a)=\|a\|.}
$$

The Gelfand transform is thus isometric and injective. Its range is closed, since $B$ is complete and an isometry takes norm-Cauchy sequences back to norm-Cauchy sequences. It contains the constants, separates the characters, and is closed under complex conjugation by the proved involution identity. The [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) says that such a unital self-adjoint point-separating subalgebra of $C(\mathcal M)$ is uniformly dense: apply its real version to real and imaginary parts. Closedness then makes the range all of $C(\mathcal M)$. Hence **the Gelfand transform is an isometric star-isomorphism under the C-star hypothesis**, establishing the [Commutative Gelfand--Naimark theorem](../../../../../commutative-gelfand-naimark-theorem.md) in the form required.

For the finite-dimensional operator application, assume first $V\ne0$ and let $A$ be the unital algebra generated by $\alpha,\beta,\alpha^*,\beta^*$. Their pairwise commutation makes $A$ commutative; it is closed under the adjoint and norm closed because it is finite-dimensional. With the [operator norm](../../../../../operator-norm.md) it is a [C-star algebra](../../../../../c-star-algebra.md). Indeed [inner product](../../../../../inner-product.md) duality gives $\|T^*\|=\|T\|$, and

$$
\|T\|^2=\sup_{\|v\|=1}\langle T^*Tv,v\rangle
\le\|T^*T\|\le\|T^*\|\|T\|=\|T\|^2.
$$

Thus the missing hypothesis in the first paragraph really does hold for this algebra, independently of any spectral theorem.

The proved result identifies $A$ with $C(\mathcal M_A)$. This character space is finite. For if it had $N$ distinct points, point separation would give, for each pair, a continuous function taking values $1$ and $0$ at the chosen two points. Products of these functions give $N$ functions with Kronecker-delta values on the selected points, hence $N$ linearly independent functions. Taking $N>\dim A$ is impossible. Write $\mathcal M_A=\{\phi_1,\ldots,\phi_m\}$, a finite Hausdorff and therefore discrete space.

Let $p_j$ be the indicator of $\{\phi_j\}$ and let $\pi_j$ be its inverse Gelfand transform in $A$. Since $p_j^2=p_j$, $\bar p_j=p_j$, $p_jp_k=0$ for $j\ne k$, and $\sum_jp_j=1$, the injective star-isomorphism gives

$$
\pi_j^2=\pi_j=\pi_j^*,\qquad\pi_j\pi_k=0\ (j\ne k),\qquad\sum_j\pi_j=I_V.
$$

Thus the $\pi_j$ are mutually orthogonal [linear projections](../../../../../projection-linear-algebra.md), and in particular commute. Put $\lambda_j=\phi_j(\alpha)$ and $\mu_j=\phi_j(\beta)$. The pointwise identities $\widehat\alpha=\sum_j\lambda_jp_j$ and $\widehat\beta=\sum_j\mu_jp_j$ pull back to

$$
\boxed{\alpha=\sum_{j=1}^m\lambda_j\pi_j,\qquad
\beta=\sum_{j=1}^m\mu_j\pi_j.}
$$

The ranges are simultaneous eigenspaces: on $\pi_jV$, the two operators act as the scalars $\lambda_j,\mu_j$. This proves that [finite commuting normal operators have joint spectral projections](../../../../../finite-commuting-normal-operators-have-joint-spectral-projections.md). If $V=0$, the same conclusion holds with empty sums.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
