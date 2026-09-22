<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a finite extension $E/K$ of [number fields](../../../../../number-field.md), the [inverse different](../../../../../inverse-different.md) is the [fractional ideal](../../../../../fractional-ideal.md)

$$
\mathfrak D_{E/K}^{-1}=\{x\in E:\operatorname{Tr}_{E/K}(x\mathcal O_E)\subseteq\mathcal O_K\}.
$$

The [different ideal](../../../../../different-ideal.md) is its inverse. The [trace pairing](../../../../../trace-pairing.md) is nondegenerate because extensions of [number fields](../../../../../number-field.md) are separable, so this definition gives a full [fractional ideal](../../../../../fractional-ideal.md). The inclusion $\mathcal O_E\subseteq\mathfrak D_{E/K}^{-1}$ shows that $\mathfrak D_{E/K}$ is integral.

Write its [prime ideal factorization](../../../../../prime-ideal-factorization.md) as $\mathfrak D_{E/K}=\prod_{\mathfrak P}\mathfrak P^{d_{\mathfrak P}}$. For $\mathfrak P$ above $\mathfrak p$, with [ramification index](../../../../../ramification-index.md) $e_{\mathfrak P}$ and residue characteristic $\ell$, the [different exponent and tame ramification](../../../../../different-exponent-and-tame-ramification.md) theorem says

$$
\boxed{d_{\mathfrak P}\geq e_{\mathfrak P}-1,\qquad d_{\mathfrak P}=e_{\mathfrak P}-1\ \Longleftrightarrow\ \ell\nmid e_{\mathfrak P}.}
$$

The equivalence uses the separability of finite residue-field extensions. In particular, $d_{\mathfrak P}=0$ precisely at unramified [prime ideals](../../../../../prime-ideal.md); in the wild case $d_{\mathfrak P}\geq e_{\mathfrak P}$. This theorem does not require a [Galois extension](../../../../../finite-galois-extension.md). The [relative discriminant](../../../../../relative-discriminant.md) is the [norm of the different ideal](../../../../../norm-of-the-different-ideal.md):

$$
\mathfrak d_{E/K}=N_{E/K}(\mathfrak D_{E/K}).
$$

For $K=\mathbb Q$, this gives $|D_E|=N(\mathfrak D_{E/\mathbb Q})$.

Now take $\alpha^3=m$ and $K=\mathbb Q(\alpha)$. For any [prime number](../../../../../prime-number.md) $q\mid m$, the [square-free integer](../../../../../square-free-integer.md) hypothesis makes $X^3-m$ an [Eisenstein polynomial](../../../../../eisenstein-polynomial.md) at $q$. It is therefore irreducible, and $K$ is a [pure cubic number field](../../../../../pure-cubic-number-field.md) of degree $3$. Since $\alpha$ is an [algebraic integer](../../../../../algebraic-integer.md), $A=\mathbb Z[\alpha]$ is an [order in a number field](../../../../../order-in-a-number-field.md). The [discriminant of elements of a number field](../../../../../discriminant-of-elements-of-a-number-field.md) for its basis $1,\alpha,\alpha^2$ is

$$
\operatorname{disc}(1,\alpha,\alpha^2)=\operatorname{disc}(X^3-m)=-27m^2.
$$

For example, the resultant of $X^3-m$ and $3X^2$ is $27m^2$, and the degree-three sign in the [polynomial discriminant](../../../../../polynomial-discriminant.md) is negative. If $I=[\mathcal O_K:A]$, the [discriminant-index formula for an integral lattice](../../../../../discriminant-index-formula-for-an-integral-lattice.md) gives

$$
-27m^2=I^2D_K.
$$

Only [prime numbers](../../../../../prime-number.md) dividing $3m$ can therefore divide $I$.

For $q\mid m$, the [Eisenstein polynomial](../../../../../eisenstein-polynomial.md) gives a [totally ramified extension](../../../../../totally-ramified-extension.md) of $\mathbb Q_q$ of degree $3$. Thus $K$ has a unique [prime ideal](../../../../../prime-ideal.md) $\mathfrak P$ above $q$, with [ramification index](../../../../../ramification-index.md) $3$ and [residue-field degree](../../../../../residue-field-degree.md) $1$. Since $q\ne3$, this is [tame ramification](../../../../../tamely-ramified-extension.md), and the [different exponent and tame ramification](../../../../../different-exponent-and-tame-ramification.md) theorem gives $d_{\mathfrak P}=2$. Hence $v_q(D_K)=2$. Comparing with $v_q(-27m^2)=2$ in the [discriminant-index formula for an integral lattice](../../../../../discriminant-index-formula-for-an-integral-lattice.md) yields $v_q(I)=0$.

At $3$, use the [shifted Eisenstein polynomial](../../../../../shifted-eisenstein-polynomial.md) of $\beta=\alpha-m$:

$$
(T+m)^3-m=T^3+3mT^2+3m^2T+(m^3-m).
$$

Because $3\nmid m$, the constant term is divisible by $3$. Moreover,

$$
9\mid m^3-m\ \Longleftrightarrow\ m\equiv\pm1\pmod9
$$

when $3\nmid m$: the factors $m-1$ and $m+1$ cannot both be divisible by $3$. The hypotheses therefore give $v_3(m^3-m)=1$, so the translated polynomial is an [Eisenstein polynomial](../../../../../eisenstein-polynomial.md) at $3$. The resulting completion is a [totally ramified extension](../../../../../totally-ramified-extension.md) of degree $3$, with [residue-field degree](../../../../../residue-field-degree.md) $1$, and its [ramification index](../../../../../ramification-index.md) is divisible by the residue characteristic. Thus its [different exponent](../../../../../different-exponent.md) is at least $3$.

It follows that $v_3(D_K)\geq3$. But $v_3(-27m^2)=3$, so

$$
3=2v_3(I)+v_3(D_K)
$$

forces $v_3(I)=0$ and $v_3(D_K)=3$. No [prime number](../../../../../prime-number.md) divides $I$. We have proved the [integral basis of a nonexceptional pure cubic field](../../../../../integral-basis-of-a-nonexceptional-pure-cubic-field.md):

$$
\boxed{\mathcal O_K=\mathbb Z[\alpha],\qquad \{1,\alpha,\alpha^2\}\text{ is an integral basis},\qquad D_K=-27m^2.}
$$

Using local [Eisenstein polynomials](../../../../../eisenstein-polynomial.md) here only establishes the local [ramification indices](../../../../../ramification-index.md); it does not assume that $\mathbb Z[\alpha]$ is already the full [ring of integers of a number field](../../../../../ring-of-integers.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
