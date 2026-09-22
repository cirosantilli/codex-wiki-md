<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A suitable version of the [Hensel lemma](../../../../../hensel-s-lemma.md) is this: if $R$ is a [complete discrete valuation ring](../../../../../complete-discrete-valuation-ring.md), $h\in R[X]$, and $\overline a$ is a root of $\overline h$ with $\overline h'(\overline a)\ne0$, there is a unique $a\in R$ reducing to $\overline a$ with $h(a)=0$. Starting with any lift, [Newton iteration over a valued field](../../../../../newton-iteration-over-a-valued-field.md) $a_{j+1}=a_j-h(a_j)/h'(a_j)$ keeps the derivative a [unit](../../../../../unit-in-a-ring.md) and doubles the error [valuation](../../../../../valuation.md), giving convergence. Uniqueness follows by factoring $h(u)-h(v)$ when two roots have the same residue.

The field in the rest of this question is not assumed complete, so that version cannot simply be applied to it. Instead use the stated uniqueness of the [extension of an absolute value](../../../../../extension-of-an-absolute-value.md). Let $\alpha_i,\alpha_j$ be any two [roots of a polynomial](../../../../../root-of-a-polynomial.md) $f$, which is irreducible. The [field embedding](../../../../../field-embedding.md) sending $\alpha_i$ to $\alpha_j$ identifies $K(\alpha_i)$ with $K(\alpha_j)$. Pulling the latter field's absolute value back gives an extension on $K(\alpha_i)$, which must coincide with the given one. More generally, for every $h\in K[X]$,

$$
|h(\alpha_i)|=|h(\alpha_j)|.
$$

This proves [equal absolute values of algebraic conjugates](../../../../../equal-absolute-values-of-algebraic-conjugates.md) without assuming separability or a transitive action of a [Galois group](../../../../../galois-group.md); repeated roots cause no difficulty.

Every root of the [monic](../../../../../monic-polynomial.md) $f\in\mathcal O_K[X]$ has absolute value at most one. Indeed, if $|\alpha|>1$, then each lower term satisfies $|c_j\alpha^j|\leq|\alpha|^j<|\alpha|^n$. The [ultrametric inequality](../../../../../ultrametric-inequality.md) makes the leading term dominate their sum, contradicting $f(\alpha)=0$. Thus

$$
\boxed{|\alpha_i|=|\alpha_1|\leq1\quad\text{for all }i.}
$$

All roots lie in the [valuation ring](../../../../../valuation-ring.md) $\mathcal O_M$, so their residues are defined in the [residue field](../../../../../residue-field.md) $k_M$. Let $\varphi\in k_K[X]$ be the [monic](../../../../../monic-polynomial.md) [minimal polynomial of an algebraic element](../../../../../minimal-polynomial-of-an-algebraic-element.md) of $\overline\alpha_1$; this residue is algebraic because it satisfies the [monic](../../../../../monic-polynomial.md) $\overline f$. Choose a coefficientwise lift $\Phi\in\mathcal O_K[X]$. Then $|\Phi(\alpha_1)|<1$, and the conjugacy argument gives $|\Phi(\alpha_i)|<1$ for every $i$. Hence every $\overline\alpha_i$ is a root of $\varphi$.

Reduction of the splitting-field factorization, with multiplicities, gives

$$
\overline f(X)=\prod_{i=1}^n(X-\overline\alpha_i)\qquad\text{in }k_M[X].
$$

Every [monic](../../../../../monic-polynomial.md) irreducible factor of $\overline f$ over $k_K$ has a root among these residues. That root also satisfies $\varphi$, so its minimal [polynomial](../../../../../polynomial-split.md) is $\varphi$. Unique factorization therefore proves the [pure-power reduction of a monic irreducible polynomial](../../../../../pure-power-reduction-of-a-monic-irreducible-polynomial.md):

$$
\boxed{\overline f=\varphi^m\quad\text{for some }m\geq1.}
$$

This does not assert that $\varphi$ is separable or that the reduction is square-free.

Finally, factor the [monic](../../../../../monic-polynomial.md) $g$ over $K$ as $g=\prod_j h_j^{e_j}$ with distinct [monic](../../../../../monic-polynomial.md) [irreducible polynomials](../../../../../irreducible-polynomial.md) $h_j$. The same leading-term argument bounds every root of $g$ by one. Coefficients of any $h_j$ are [elementary symmetric polynomials](../../../../../elementary-symmetric-polynomial.md) in some of these roots, so they lie in $\mathcal O_K$. By the preceding result each $\overline h_j$ is a power of a single [monic](../../../../../monic-polynomial.md) irreducible residue [polynomial](../../../../../polynomial-split.md) $\varphi_j$.

Since the prescribed $\overline g_1,\overline g_2$ are [coprime](../../../../../coprime-integers.md), every $\varphi_j$ occurs on exactly one side. Assign the entire factor $h_j^{e_j}$ to that side and form the two products. Comparing irreducible-factor multiplicities in the reduction proves the [coprime factor lifting from valuation-extension uniqueness](../../../../../coprime-factor-lifting-from-valuation-extension-uniqueness.md):

$$
\boxed{g=g_1g_2,\qquad g_i\in\mathcal O_K[X]\text{ monic},\qquad\overline{g_i}=\overline g_i.}
$$

Empty products are one, covering constant prescribed factors. The construction proves the required factor-lifting form of the [Hensel lemma](../../../../../hensel-s-lemma.md) directly from extension uniqueness, without adding completeness as an unstated hypothesis.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 136](../../paper-136-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
