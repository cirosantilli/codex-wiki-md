<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here $F$ is the usual one-dimensional commutative [formal group law](../../../../../../formal-group-law.md). Normalize the [valuation](../../../../../../valuation.md) $v$ by $v(\pi)=1$, and put $e=v(p)$. We show explicitly that for any [integer](../../../../../../integer.md) $m>e/(p-1)$,

$$
\boxed{F(\pi^m\mathcal O_K)\cong(\pi^m\mathcal O_K,+)\cong(\mathcal O_K,+).}
$$

This subgroup will have finite index in $F(\pi\mathcal O_K)$.

Set $a(T)=\partial_YF(T,0)$. Since $F(X,Y)=X+Y+$ terms of [total degree](../../../../../../total-degree-of-a-polynomial.md) at least two, $a(T)\in1+T\mathcal O_K[[T]]$. Its inverse has integral coefficients, say $a(T)^{-1}=\sum_{j\geq0}c_jT^j$ with $c_0=1$. Define the [formal logarithm](../../../../../../formal-logarithm.md) over $K$ by

$$
\ell(T)=\int_0^T\frac{dt}{a(t)}=\sum_{n\geq1}\frac{c_{n-1}}nT^n.
$$

Differentiate [associativity](../../../../../../associative-property.md) $F(F(X,Y),Z)=F(X,F(Y,Z))$ with respect to $Z$ at zero. This gives $a(F(X,Y))=\partial_YF(X,Y)a(Y)$, so

$$
\partial_Y\ell(F(X,Y))=\frac1{a(Y)}=\ell'(Y).
$$

Evaluating at $Y=0$ proves the formal identity $\ell(F(X,Y))=\ell(X)+\ell(Y)$.

The coefficients satisfy $v(c_{n-1}/n)\geq-e v_p(n)$. Thus the series converges on $\pi\mathcal O_K$, since for $v(T)\geq1$ the [valuations](../../../../../../valuation.md) of its terms are at least $n-e v_p(n)\to\infty$. More quantitatively,

$$
v_p(n)\leq\frac{n-1}{p-1}.
$$

Indeed, if $k=v_p(n)$ then $n\geq p^k\geq1+k(p-1)$. If $v(T)\geq m>e/(p-1)$, every nonlinear term has [valuation](../../../../../../valuation.md) strictly greater than $v(T)$. Write $h(T)=\ell(T)-T$. For $S,T\in\pi^m\mathcal O_K$, use $T^n-S^n=(T-S)\sum_{j=0}^{n-1}T^{n-1-j}S^j$ to obtain

$$
v(h(T)-h(S))\geq v(T-S)+1.
$$

The extra [valuation](../../../../../../valuation.md) is integral and positive because $(n-1)m-e v_p(n)>0$ for all $n\geq2$.

For any $b\in\pi^m\mathcal O_K$, solve $\ell(T)=b$ by iterating $T\mapsto b-h(T)$. This map preserves the complete ball $\pi^m\mathcal O_K$ and improves differences by at least one [valuation](../../../../../../valuation.md) step. The [contraction mapping theorem](../../../../../../contraction-mapping-theorem.md) gives a unique solution. Therefore $\ell$ is a bijection of this ball onto itself, and the formal identity, now evaluated in [convergent series](../../../../../../convergent-series.md), makes it a [group isomorphism](../../../../../../group-isomorphism.md). Multiplication by $\pi^{-m}$ then identifies the additive target with $\mathcal O_K$.

Integral coefficients in $F$ and its [formal inverse](../../../../../../formal-inverse.md) ensure that every $F(\pi^j\mathcal O_K)$ is a subgroup. Reduction modulo $\pi^m$ respects the group law; two parameters represent the same coset of $F(\pi^m\mathcal O_K)$ exactly when they are congruent modulo $\pi^m$. If the [residue field](../../../../../../residue-field.md) has $q_K$ elements, the quotient consequently has $q_K^{m-1}$ elements. This proves both the finite-index assertion and the claimed additive structure, with an explicit depth that also works in ramified extensions and when $p=2$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
