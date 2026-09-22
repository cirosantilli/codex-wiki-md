<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work over $\mathbb C$ and take a nonzero commutative unital [Banach algebra](../../../../../banach-algebra-split.md) $A$, with $\|1\|=1$. A [character of an algebra](../../../../../character-of-an-algebra.md) is a nonzero multiplicative complex [linear functional](../../../../../linear-functional.md) $\chi:A\to\mathbb C$. It satisfies $\chi(1)=1$. Moreover $\chi(a)\in\sigma_A(a)$: otherwise $a-\chi(a)1$ would be invertible, although its image under $\chi$ is zero. The bound on the [spectrum of an element](../../../../../spectrum-of-an-element.md) therefore gives $|\chi(a)|\leq\|a\|$, proving [automatic continuity of characters](../../../../../automatic-continuity-of-characters.md) and $\|\chi\|=1$.

Every proper [maximal ideal](../../../../../maximal-ideal.md) $M$ of $A$ is closed. Indeed its closure is an [ideal](../../../../../ideal.md); if this closure were all of $A$, $M$ would contain an element within distance less than one of $1$. Such an element is invertible by the Neumann [series](../../../../../series-mathematics.md), forcing $1\in M$. Thus the closure is proper and maximality makes it equal to $M$. The [quotient Banach space](../../../../../quotient-banach-space.md) $A/M$, with its quotient [Banach algebra](../../../../../banach-algebra-split.md) structure, is a complex [normed division algebra](../../../../../normed-division-algebra.md). By the [Gelfand-Mazur theorem](../../../../../gelfand-mazur-theorem.md), it is $\mathbb C$, so the quotient map gives a [character of an algebra](../../../../../character-of-an-algebra.md) with kernel $M$. Conversely, the kernel of every [character of an algebra](../../../../../character-of-an-algebra.md) is a [maximal ideal](../../../../../maximal-ideal.md), since the character is onto $\mathbb C$. The [Zorn lemma](../../../../../zorn-s-lemma.md) supplies a [maximal ideal](../../../../../maximal-ideal.md) containing every proper [ideal](../../../../../ideal.md), so the [character space of an algebra](../../../../../character-space-of-an-algebra.md) $\Delta(A)$ is nonempty.

These facts give the exact relation between the [character space](../../../../../character-space-of-an-algebra.md) and the [spectrum of an element](../../../../../spectrum-of-an-element.md):

$$
\boxed{\sigma_A(a)=\{\chi(a):\chi\in\Delta(A)\}.}
$$

One inclusion was proved above. For the other, if $a-\lambda1$ is noninvertible, the principal [ideal](../../../../../ideal.md) it generates is proper because $A$ is commutative. Contain it in a [maximal ideal](../../../../../maximal-ideal.md) and use its corresponding [character of an algebra](../../../../../character-of-an-algebra.md) to obtain $\chi(a)=\lambda$.

Give $\Delta(A)$ the [Gelfand topology](../../../../../gelfand-topology.md), namely its [subspace topology](../../../../../subspace-topology.md) from the [weak-star topology](../../../../../weak-star-topology.md) on $A^*$. In the [closed unit ball](../../../../../closed-unit-ball.md) of $A^*$, it is the intersection of the closed conditions

$$
\chi(1)=1,\qquad \chi(ab)=\chi(a)\chi(b)\quad(a,b\in A).
$$

Consequently [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) makes $\Delta(A)$ a compact [Hausdorff space](../../../../../hausdorff-space.md). For every $a\in A$, define the [Gelfand transform](../../../../../gelfand-representation.md) $\widehat a(\chi)=\chi(a)$. This is a [continuous function](../../../../../continuous-function.md) on $\Delta(A)$ by definition of the [Gelfand topology](../../../../../gelfand-topology.md). The [Gelfand representation theorem](../../../../../gelfand-representation-theorem.md) gives a contractive unital [algebra homomorphism over a field](../../../../../algebra-homomorphism-over-a-field.md)

$$
\Gamma:A\longrightarrow C(\Delta(A)),\qquad a\longmapsto\widehat a,
\qquad
\boxed{\|\widehat a\|_\infty=r(a)\leq\|a\|.}
$$

Multiplicativity and linearity follow by evaluating at each [character of an algebra](../../../../../character-of-an-algebra.md); the [supremum norm](../../../../../supremum-norm.md) equality follows from the preceding [spectrum of an element](../../../../../spectrum-of-an-element.md) identity. Its kernel is

$$
\ker\Gamma=\bigcap_{\chi\in\Delta(A)}\ker\chi
=\bigcap_{M\text{ maximal}}M=\operatorname{rad}A,
$$

the [Jacobson radical](../../../../../jacobson-radical.md). Equivalently, its elements have [spectrum of an element](../../../../../spectrum-of-an-element.md) $\{0\}$. Thus $\Gamma$ is injective precisely when $A$ is a [semisimple commutative Banach algebra](../../../../../semisimple-commutative-banach-algebra.md), and it gives a faithful continuous representation of $A/\operatorname{rad}A$ as a function algebra. Its range contains the constants and separates points of $\Delta(A)$, because distinct [characters of an algebra](../../../../../character-of-an-algebra.md) differ on some $a$. An arbitrary [Banach algebra](../../../../../banach-algebra-split.md) need not have an isometric or surjective [Gelfand transform](../../../../../gelfand-representation.md), nor a uniformly dense range: those conclusions require further hypotheses.

For the [Banach algebra](../../../../../banach-algebra-split.md) $C(K)$ on a nonempty compact [Hausdorff space](../../../../../hausdorff-space.md) $K$, all [characters of an algebra](../../../../../character-of-an-algebra.md) are [evaluation characters](../../../../../evaluation-character.md). To see this, let $M$ be a [maximal ideal](../../../../../maximal-ideal.md). If its elements had no common zero, compactness would supply $f_1,\ldots,f_n\in M$ with no common zero. The [continuous function](../../../../../continuous-function.md) $h=\sum_i\overline{f_i}f_i$ belongs to $M$, is strictly positive on $K$, and has a continuous reciprocal. It is therefore invertible, a contradiction. Hence all elements of $M$ vanish at some $x\in K$, so $M\subseteq\ker\delta_x$ and maximality gives equality. The associated [character of an algebra](../../../../../character-of-an-algebra.md) must be $\delta_x$: since $f-f(x)1\in M$, its value on $f$ is $f(x)$.

The map $x\mapsto\delta_x$ is a continuous bijection $K\to\Delta(C(K))$, using separation of points by [continuous functions](../../../../../continuous-function.md). Compactness and the Hausdorff property make it a [homeomorphism](../../../../../homeomorphism.md). Under this identification the [Gelfand transform](../../../../../gelfand-representation.md) is **$\boxed{\widehat f(\delta_x)=f(x)}$**, so it is the identity representation of $C(K)$, in particular an isometric onto map. The empty $K$ gives the zero algebra, whose empty [character space](../../../../../character-space-of-an-algebra.md) represents the zero function space; it was excluded by the nonzero unital convention above.

Now let $A$ be a commutative unital [C-star algebra](../../../../../c-star-algebra.md). The stronger conclusion is the [Commutative Gelfand--Naimark theorem](../../../../../commutative-gelfand-naimark-theorem.md): **the [Gelfand transform](../../../../../gelfand-representation.md) is an isometric onto [C-star homomorphism](../../../../../c-star-homomorphism.md) $A\cong C(\Delta(A))$**. We prove the additional assertions without assuming this conclusion.

First every [character of an algebra](../../../../../character-of-an-algebra.md) respects the [C-star algebra](../../../../../c-star-algebra.md) involution. If $h=h^*$, the elements $e^{ith}$, $t\in\mathbb R$, are [unitary elements of a C-star algebra](../../../../../unitary-element-of-a-c-star-algebra.md), and their [norm](../../../../../norm.md) is one by the [C-star identity](../../../../../c-star-identity.md). Continuity and multiplicativity give $\chi(e^{ith})=e^{it\chi(h)}$. Thus $|e^{it\chi(h)}|\leq1$ for every real $t$, forcing $\chi(h)$ to be real. Writing $a=h+ik$ with $h=(a+a^*)/2$ and $k=(a-a^*)/(2i)$ self-adjoint gives $\chi(a^*)=\overline{\chi(a)}$. Therefore the range of $\Gamma$ is closed under [complex conjugation](../../../../../complex-conjugation.md).

Every element of commutative $A$ is a [Normal element of a C-star algebra](../../../../../normal-element-of-a-c-star-algebra.md). For a normal $b$, use the [C-star identity](../../../../../c-star-identity.md), and then the same identity for the self-adjoint element $b^*b$, to obtain

$$
\|b^2\|^2=\|(b^2)^*b^2\|=\|(b^*b)^2\|
=\|b^*b\|^2=\|b\|^4.
$$

Its powers are also normal, so $\|a^{2^n}\|=\|a\|^{2^n}$. The [spectral radius formula](../../../../../spectral-radius-formula.md) gives $r(a)=\|a\|$, hence $\|\widehat a\|_\infty=\|a\|$. The [Gelfand transform](../../../../../gelfand-representation.md) is therefore an [isometry](../../../../../isometry.md), and its range is complete and closed in the [supremum norm](../../../../../supremum-norm.md). It contains constants, separates points and is closed under [complex conjugation](../../../../../complex-conjugation.md). The complex [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) makes that range dense, hence all of $C(\Delta(A))$.

The approximation step in [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md) can also be seen directly here. For a unital conjugation-closed point-separating subalgebra $B\subseteq C(K)$, the real-valued part of its uniform closure is closed under absolute values, by polynomial approximation to $|t|$ on bounded intervals, hence under pointwise maxima and minima. Its real-valued functions separate points. Given real $f\in C(K)$ and $\varepsilon>0$, for each $x,y$ an affine rescaling of a separating function produces $b_{x,y}$ agreeing with $f$ at $x,y$; take a constant when $x=y$. For fixed $x$, finitely many neighbourhoods of $y$ where $b_{x,y}>f-\varepsilon$ cover $K$. Their maximum $b_x$ exceeds $f-\varepsilon$ everywhere and agrees with $f$ at $x$, hence is less than $f+\varepsilon$ near $x$. Finitely many of these latter neighbourhoods cover $K$; the minimum of their $b_x$ lies between $f-\varepsilon$ and $f+\varepsilon$ everywhere. Approximate real and imaginary parts separately. This proves the density used above and completes the [C-star algebra](../../../../../c-star-algebra.md) conclusion.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
