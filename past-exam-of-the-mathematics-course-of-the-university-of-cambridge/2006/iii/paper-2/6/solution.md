<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Fix a finite-dimensional nonnegative [filtration of a ring](../../../../../filtration-of-a-ring.md) giving $R$ its [almost commutative algebra](../../../../../almost-commutative-algebra.md) structure, and choose a [good filtration of a module](../../../../../good-filtration-of-a-module.md) on $M$. When $\operatorname{gr}R$ is a [standard graded algebra](../../../../../standard-graded-algebra.md), the [Hilbert-Serre theorem](../../../../../hilbert-serre-theorem.md) makes the cumulative Hilbert function $h_M(j)=\dim_k F_jM$ eventually a [polynomial](../../../../../polynomial-split.md). For $M\ne0$, define the [dimension of a filtered module](../../../../../dimension-of-a-filtered-module.md) and [multiplicity of a filtered module](../../../../../multiplicity-of-a-filtered-module.md) by

$$
\boxed{d(M)=\deg h_M,\qquad
m(M)=d(M)!\,[j^{d(M)}]h_M(j)}.
$$

Use $d(0)=-\infty$ and $m(0)=0$. With positive weighted generators instead of a standard grading, the cumulative Hilbert function is eventually a [quasipolynomial](../../../../../quasipolynomial.md) with a common positive leading coefficient across residue classes. Equivalently, $h_M(j)=c j^d+O(j^{d-1})$, and the definitions are $d(M)=d$ and $m(M)=d!\,c$. The common leading coefficient follows from monotonicity: interlacing consecutive residue classes forces their leading coefficients to agree. For a standard grading, multiplicity is a positive integer, since an integer-valued [polynomial](../../../../../polynomial-split.md) has an integral expansion in the binomial polynomials; weighted normalization can instead give a positive rational number.

Two [good filtrations of a module](../../../../../good-filtration-of-a-module.md) for this fixed algebra filtration bound each other after fixed index shifts. The corresponding Hilbert functions therefore satisfy $h_F(j-a)\leq h_G(j)\leq h_F(j+b)$ for fixed $a,b$. Comparing their leading growth shows that the degree and leading coefficient agree. Thus $d(M)$ and $m(M)$ are independent of the module filtration; the fixed algebra filtration is part of the multiplicity convention.

For a [submodule](../../../../../submodule.md) $N$, use its [subspace filtration](../../../../../subspace-filtration.md) and the [quotient filtration](../../../../../quotient-filtration.md) on $M/N$. These are good because $\operatorname{gr}R$ is [Noetherian](../../../../../noetherian-ring.md). The [short exact sequence](../../../../../short-exact-sequence.md) of filtered pieces gives

$$
h_M(j)=h_N(j)+h_{M/N}(j).
$$

Nonzero leading coefficients are positive, so

$$
\boxed{d(M)=\max\{d(N),d(M/N)\}}.
$$

If $d(N)=d(M/N)$, those leading coefficients add and

$$
\boxed{m(M)=m(N)+m(M/N)}.
$$

This is [dimension and multiplicity in a filtered exact sequence](../../../../../dimension-and-multiplicity-in-a-filtered-exact-sequence.md).

For the [Weyl algebra](../../../../../weyl-algebra.md) $A_n(k)$ in characteristic zero, [Bernstein inequality for Weyl algebra modules](../../../../../bernstein-inequality-for-weyl-algebra-modules.md) asserts $d(M)\geq n$ for every nonzero [finitely generated module](../../../../../finitely-generated-module.md) $M$. Write its generators as $x_i,D_i$, with $[D_i,x_j]=\delta_{ij}$ and all other generator commutators zero. The ordered monomials $x^\alpha D^\beta$ give the [Bernstein filtration](../../../../../bernstein-filtration.md)

$$
A_j=\operatorname{span}_k\{x^\alpha D^\beta:|\alpha|+|\beta|\leq j\},
\qquad\dim_k A_j=\binom{j+2n}{2n}.
$$

Take a finite-dimensional generating subspace $V\ne0$ of $M$ and put $M_j=A_jV$.

To prove [faithful finite-step action of a Weyl algebra](../../../../../faithful-finite-step-action-of-a-weyl-algebra.md), consider $0\ne a\in A_j$ and choose a nonzero coefficient $c_{\alpha\beta}$ of a monomial of maximal total degree $d\leq j$. Applying $\prod_i(\operatorname{ad}D_i)^{\alpha_i}(\operatorname{ad}x_i)^{\beta_i}$ to $a$ gives

$$
\lambda=c_{\alpha\beta}\alpha!\,\beta!\,(-1)^{|\beta|}\ne0.
$$

Indeed, these [commutators](../../../../../commutator.md) differentiate the ordered coefficients: lower-degree monomials vanish, and another degree-$d$ monomial can survive only if all its exponents dominate $(\alpha,\beta)$, which forces equality. This is [scalar extraction by iterated Weyl commutators](../../../../../scalar-extraction-by-iterated-weyl-commutators.md).

Expanding these iterated [commutators](../../../../../commutator.md) writes $\lambda=\sum_\ell u_\ell a v_\ell$ with $u_\ell,v_\ell\in A_j$. If $a$ annihilated $M_j$, every summand would annihilate $V$, contrary to $\lambda V\ne0$. Therefore the action map is [injective](../../../../../injective-function.md):

$$
A_j\hookrightarrow\operatorname{Hom}_k(M_j,M_{2j}).
$$

Taking dimensions and comparing polynomial degrees gives

$$
\binom{j+2n}{2n}\leq h_M(j)h_M(2j),
\qquad 2n\leq2d(M),
$$

which proves [Bernstein inequality for Weyl algebra modules](../../../../../bernstein-inequality-for-weyl-algebra-modules.md). The polynomial representation $k[x_1,\ldots,x_n]$ has dimension $n$, so the bound is sharp.

The [associated graded ring](../../../../../associated-graded-ring.md) of the [Weyl algebra](../../../../../weyl-algebra.md) is a polynomial ring, so [ascending filtered-graded transfer of Noetherianity](../../../../../ascending-filtered-graded-transfer-of-noetherianity.md) makes $A_n(k)$ a [left Noetherian ring](../../../../../left-noetherian-ring.md). Thus every [submodule](../../../../../submodule.md) of a [finitely generated module](../../../../../finitely-generated-module.md) is finitely generated. If $d(M)=n$, every nonzero subquotient has dimension at most $n$ by the exact-sequence formula, and at least $n$ by [Bernstein inequality for Weyl algebra modules](../../../../../bernstein-inequality-for-weyl-algebra-modules.md). Every such subquotient therefore has dimension $n$ and positive integral multiplicity.

In a strictly descending chain $M=M_0\supsetneq M_1\supsetneq\cdots$, each nonzero quotient $M_i/M_{i+1}$ consumes at least one unit of multiplicity, by [dimension and multiplicity in a filtered exact sequence](../../../../../dimension-and-multiplicity-in-a-filtered-exact-sequence.md). Hence there are at most $m(M)$ strict steps. This proves the [descending chain condition](../../../../../descending-chain-condition.md), so **$M$ is Artinian**. In fact this [holonomic Weyl algebra module](../../../../../holonomic-weyl-algebra-module.md) has [module length](../../../../../length-of-a-module.md) at most $m(M)$, as in [multiplicity bounds the length of a holonomic Weyl module](../../../../../multiplicity-bounds-the-length-of-a-holonomic-weyl-module.md).

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
