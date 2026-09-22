<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

Let

$$
F(X)=a_nX^n+\cdots+a_1X+a_0\in\mathbb Z[X]
$$

be a [primitive polynomial](../../../../../primitive-polynomial.md). The [Eisenstein criterion](../../../../../eisenstein-criterion.md) states that if a [prime number](../../../../../prime-number.md) $p$ satisfies

$$
p\nmid a_n,\qquad p\mid a_j\ (0\leq j<n),\qquad p^2\nmid a_0,
$$

then $F$ is an [irreducible polynomial](../../../../../irreducible-polynomial.md) in $\mathbb Z[X]$, equivalently in $\mathbb Q[X]$ by [Gauss lemma for polynomials](../../../../../gauss-lemma-for-polynomials.md).

To prove it, suppose that $F=GH$ with $G,H\in\mathbb Z[X]$ of positive degree. Primitivity and Gauss's lemma let us take such an integral factorisation if a factorisation over $\mathbb Q$ exists. Reducing modulo $p$ gives

$$
\overline G\,\overline H=\overline{a_n}X^n.
$$

Because $p$ does not divide the leading coefficient of $F$, neither factor loses degree on reduction. The polynomial ring $\mathbb F_p[X]$ is a [unique factorization domain](../../../../../unique-factorization-domain.md), so both reductions are monomials of positive degree. In particular, $p$ divides both constant terms $G(0)$ and $H(0)$. It follows that $p^2$ divides

$$
F(0)=G(0)H(0)=a_0,
$$

a contradiction. This proves the criterion.

For a prime $p$, translate the geometric sum by one:

$$
f(X+1)=\frac{(X+1)^p-1}{X}
=\sum_{k=1}^{p}\binom pk X^{k-1}.
$$

Its leading coefficient is one, every other coefficient is divisible by $p$, and its constant coefficient is $p$, which is not divisible by $p^2$. It is therefore Eisenstein at $p$. Translation $X\mapsto X+1$ is an automorphism of $\mathbb Z[X]$, so

$$
\boxed{f(X)=1+X+\cdots+X^{p-1}\text{ is irreducible}.}
$$

This is the [geometric-sum irreducibility criterion](../../../../../geometric-sum-irreducibility-criterion.md).

The [evaluation homomorphism](../../../../../evaluation-homomorphism.md)

$$
\operatorname{ev}_\zeta:\mathbb Z[X]\longrightarrow\mathbb C,
\qquad G\longmapsto G(\zeta),
$$

has image $\mathbb Z[\zeta]$ and contains $(f)$ in its kernel. Since $f$ is monic, division by $f$ in $\mathbb Z[X]$ writes every $G$ as $G=Qf+R$ with $\deg R<\deg f$. If $G(\zeta)=0$, then $R(\zeta)=0$; the irreducibility of $f$ says that $f$ is the [minimal polynomial](../../../../../minimal-polynomial.md) of $\zeta$, so $R=0$. Thus $\ker(\operatorname{ev}_\zeta)=(f)$, and the [first isomorphism theorem for rings](../../../../../first-isomorphism-theorem-for-rings.md) gives

$$
\boxed{\mathbb Z[\zeta]\cong\mathbb Z[X]/(f)}.
$$

Now take $p=3$. Then $\zeta^2+\zeta+1=0$, and the [Eisenstein integers](../../../../../eisenstein-integer.md) are

$$
\mathbb Z[\zeta]=\{a+b\zeta:a,b\in\mathbb Z\}.
$$

Complex conjugation sends $\zeta$ to $\zeta^2$, so the [field norm](../../../../../field-norm.md) is

$$
N(a+b\zeta)=(a+b\zeta)(a+b\zeta^2)=a^2-ab+b^2=|a+b\zeta|^2.
$$

Given $z=x+y\zeta\in\mathbb C$, choose integers $m,n$ with $|x-m|,|y-n|\leq\tfrac12$. For $q=m+n\zeta$,

$$
|z-q|^2=(x-m)^2-(x-m)(y-n)+(y-n)^2\leq\frac34<1.
$$

For $\alpha,\beta\in\mathbb Z[\zeta]$ with $\beta\ne0$, apply this to $z=\alpha/\beta$ and put $r=\alpha-q\beta$. Then

$$
N(r)=N(\beta)|z-q|^2<N(\beta).
$$

Hence the norm is a [Euclidean function](../../../../../euclidean-function.md), proving that $\mathbb Z[\zeta]$ is a [Euclidean domain](../../../../../euclidean-domain.md). This is the [Euclidean norm on the Eisenstein integers](../../../../../euclidean-norm-on-the-eisenstein-integers.md).

Finally suppose $A\in\mathrm{GL}_n(\mathbb Z)$ satisfies $A^2+A+I=0$. Make the free abelian group $M=\mathbb Z^n$ into a $\mathbb Z[\zeta]$-module by defining

$$
\zeta v=Av.
$$

This is well-defined precisely because $A$ obeys the same polynomial relation as $\zeta$. The module is finitely generated. It is also [torsion-free module](../../../../../torsion-free-module.md): if $0\ne\alpha\in\mathbb Z[\zeta]$ and $\alpha v=0$, multiplication by the conjugate of $\alpha$ gives $N(\alpha)v=0$, and the additive group $\mathbb Z^n$ has no nonzero integer torsion.

A Euclidean domain is a [principal ideal domain](../../../../../principal-ideal-domain.md), and the [structure theorem for finitely generated modules over a principal ideal domain](../../../../../structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain.md) says that a finitely generated torsion-free module over one is free. Thus

$$
M\cong\mathbb Z[\zeta]^m
$$

for some $m$. Since $\mathbb Z[\zeta]$ has [free module](../../../../../free-module.md) basis $1,\zeta$ over $\mathbb Z$, comparison of abelian ranks gives $n=2m$. There can consequently be no such matrix when $n$ is odd.

If $n=2m$, choose a $\mathbb Z[\zeta]$-basis $v_1,\ldots,v_m$. Then

$$
v_1,Av_1,\ldots,v_m,Av_m
$$

is a $\mathbb Z$-basis, and $A^2v_i=-v_i-Av_i$. In this basis the matrix of $A$ is a direct sum of $m$ copies of

$$
C=\begin{pmatrix}0&-1\\1&-1\end{pmatrix}.
$$

Every admissible matrix is therefore conjugate in $\mathrm{GL}_n(\mathbb Z)$ to $C^{\oplus m}$. Hence there is exactly one conjugacy class for even $n$, and none for odd $n$. This is the [classification of integral matrices satisfying the third cyclotomic polynomial](../../../../../classification-of-integral-matrices-satisfying-the-third-cyclotomic-polynomial.md).

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
