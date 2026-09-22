<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a finitely generated algebra over $k$, choose a finite-dimensional generating subspace $V$ containing one. Its [Gelfand–Kirillov dimension](../../../../../gelfand-kirillov-dimension.md) is

$$
\operatorname{GKdim}R=\limsup_{n\to\infty}\frac{\log(\dim_kV^n)}{\log n}.
$$

Changing generators bounds the two filtrations by constant rescalings of the index, so the value is independent of $V$.

For the [noncommutative Krull dimension](../../../../../noncommutative-krull-dimension.md), set the zero module's dimension to $-1$. A nonzero module has dimension zero exactly when it is an [Artinian module](../../../../../artinian-module.md). Recursively, dimension at most $d$ means that in every descending chain of submodules the successive factors eventually have dimension less than $d$; use the ordinal version of this definition if necessary. The left Krull dimension of $R$ is that of its left regular module. For commutative Noetherian rings this agrees with the usual prime-chain [Krull dimension](../../../../../krull-dimension.md), but prime-chain counting alone is not its definition for a noncommutative ring.

Write $U=U(\mathfrak{sl}_2(\mathbb C))$ with $[h,e]=2e$, $[h,f]=-2f$, $[e,f]=h$. By the [Poincaré-Birkhoff-Witt theorem](../../../../../poincare-birkhoff-witt-theorem.md), $f^ih^je^k$ form a basis. In the total-degree filtration there are $\binom{n+3}{3}$ such monomials of degree at most $n$, so

$$
\boxed{\operatorname{GKdim}U=3.}
$$

The commutators lower degree, giving $\operatorname{gr}U\cong\mathbb C[f,h,e]$, which also proves that $U$ is left and right Noetherian by finite leading-term cancellation.

To determine the module-theoretic Krull dimension, use the [generalized Weyl algebra](../../../../../generalized-weyl-algebra.md) description and verify the dimension criterion, rather than substituting the three-dimensional graded ring. Put

$$
z=4fe+h^2+2h.
$$

Commutation with $h$ is immediate; with $e$, the contributions are $4he-2(eh+he)-4e=0$, using $he-eh=2e$. The corresponding calculation with $f$ also vanishes. Thus $z$ is a [Casimir element](../../../../../casimir-element.md). The subalgebra $D=\mathbb C[h,z]$ is a polynomial ring in two variables: for a nonzero polynomial in $z$ with coefficients in $\mathbb C[h]$, its highest $z$ power contributes a nonzero PBW term with that many copies of both $f$ and $e$, and no lower power can cancel it.

Take $\sigma(h)=h-2$, $\sigma(z)=z$ and $t=(z-h^2-2h)/4$. The relations become

$$
ed=\sigma(d)e,\quad fd=\sigma^{-1}(d)f\ (d\in D),\qquad
fe=t,\quad ef=\sigma(t)=\frac{z-h^2+2h}{4}.
$$

They identify $U$ with $D(\sigma,t)$. Surjectivity follows from its generators; injectivity follows from PBW: the graded pieces $D$, $De^r$ and $Df^r$ for $r>0$ are linearly independent, using the difference between the $e$ and $f$ exponents and then the highest paired exponent. Every PBW monomial lies in one of these pieces by replacing paired $f,e$ powers with polynomials in $h,z$.

We use the following general [Krull dimension criterion for rank-one generalized Weyl algebras](../../../../../krull-dimension-criterion-for-rank-one-generalized-weyl-algebras.md): for a commutative Noetherian base $D$ of dimension $d$, the [generalized Weyl algebra](../../../../../generalized-weyl-algebra.md) has Krull dimension $d$ provided no height-$d$ maximal ideal is periodic under $\sigma$ and none contains infinitely many translates $\sigma^n(t)$. This is Theorem 5.3, specialized to the commutative base, in [Krull dimension of Generalized Weyl Algebras with non-commutative coefficients](https://webhomes.maths.ed.ac.uk/~tom/KdimGWA.pdf).

Here every maximal ideal is $\mathfrak m_{\lambda,\mu}=(h-\lambda,z-\mu)$ and has height two. Its translates have $h$ coordinate $\lambda+2n$, so no nonzero power of $\sigma$ fixes it. Further,

$$
\sigma^n(t)\bmod\mathfrak m_{\lambda,\mu}
=\frac{\mu-(\lambda-2n)^2-2(\lambda-2n)}4.
$$

This is a nonzero quadratic polynomial in $n$, so it vanishes for at most two integers. Both exceptional mechanisms are excluded for every maximal ideal, and the base has dimension two. The criterion consequently gives

$$
\boxed{\operatorname{Kdim}U=2.}
$$

The orbit and root calculations are needed for this upper bound on the entire left-ideal lattice; merely exhibiting a length-two chain of prime ideals would only prove a lower bound.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
