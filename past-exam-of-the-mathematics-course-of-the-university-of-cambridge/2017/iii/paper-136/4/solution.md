<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Fix a non-Archimedean [local field](../../../../../local-field.md) $K$, its [valuation ring](../../../../../valuation-ring.md) $R=\mathcal O_K$, a [uniformizer](../../../../../uniformizer.md) $\pi$, and a [residue field](../../../../../residue-field.md) with cardinality $q$. The construction below applies both in mixed and equal characteristic. A one-dimensional commutative [formal group law](../../../../../formal-group-law.md) is $F(X,Y)\in R[[X,Y]]$ with identity, associativity and commutativity, and $F(X,Y)=X+Y+$ higher-degree terms. It has a unique [formal inverse](../../../../../formal-inverse.md). Its morphisms are series $h(T)\in TR[[T]]$ with $h(F(X,Y))=G(h(X),h(Y))$; a [unit](../../../../../unit-in-a-ring.md) linear coefficient makes such a morphism invertible by recursive coefficient comparison. Evaluating its integral series on the [maximal ideal](../../../../../maximal-ideal.md) of a finite extension of $K$ is legitimate because the series converge there.

Choose a [Lubin–Tate series](../../../../../lubin-tate-series.md) $f(T)$ satisfying

$$
f(T)=\pi T+O(T^2),\qquad f(T)\equiv T^q\pmod\pi.
$$

A useful choice is $f(T)=\pi T+T^q$. The [Lubin–Tate functional equation lemma](../../../../../lubin-tate-functional-equation-lemma.md) constructs a unique series with any prescribed linear form $\ell$ and satisfying

$$
f(H(X_1,\ldots,X_r))=H(f(X_1),\ldots,f(X_r)).
$$

Here is its coefficient argument. If terms below degree $d$ have been found, the unknown homogeneous degree-$d$ term appears with multiplier $\pi-\pi^d$. The already known error has every coefficient divisible by $\pi$: after reduction, the equation becomes $H(X)^q=H(X_1^q,\ldots,X_r^q)$, valid because the residue coefficients lie in $\mathbb F_q$. Since $\pi-\pi^d$ is $\pi$ times a [unit](../../../../../unit-in-a-ring.md) for $d\geq2$, the next term is uniquely determined and integral. Recursion proves existence and uniqueness.

Use $\ell=X+Y$ to construct $F_f$, and $\ell=aT$ to construct $[a]_f$ for every $a\in R$. Uniqueness gives $F_f(X,0)=X$ and $F_f(0,Y)=Y$. Comparing $[a]_f(F_f(X,Y))$ with $F_f([a]_f(X),[a]_f(Y))$, which satisfy the same functional equation and have the same linear form, proves that $[a]_f$ is an endomorphism of the law. The same uniqueness applied to three variables proves associativity: $F_f(F_f(X,Y),Z)$ and $F_f(X,F_f(Y,Z))$ have the same linear form and functional equation. It also proves commutativity and the identities

$$
[a+b]_f(T)=F_f([a]_f(T),[b]_f(T)),\qquad
[ab]_f=[a]_f\circ[b]_f,\qquad [1]_f(T)=T,\qquad [\pi]_f=f.
$$

Thus this [Lubin–Tate formal group](../../../../../lubin-tate-formal-group.md) is equipped with an action of the whole ring $R$, not only its integers. For a [unit](../../../../../unit-in-a-ring.md) $a$, the inverse of $[a]_f$ is $[a^{-1}]_f$. The same recursion, with two series for the fixed $\pi$, gives a unique strict [Lubin–Tate change of series](../../../../../lubin-tate-change-of-series.md). Its integral series and inverse converge on torsion points, so it identifies their torsion fields. We may compute with $f(T)=\pi T+T^q$ without losing the general construction for that uniformizer.

Write $f_0(T)=T$ and $f_n=f^{\circ n}$. The [Lubin–Tate torsion](../../../../../lubin-tate-torsion.md) of level $n$ is

$$
\Lambda_n=\{x\text{ algebraic over }K:|x|<1,\ f_n(x)=0\}.
$$

For $n\geq1$, its primitive points are the roots of

$$
\Phi_n(T)=\frac{f_n(T)}{f_{n-1}(T)}=\pi+f_{n-1}(T)^{q-1}.
$$

This is a [monic](../../../../../monic-polynomial.md) [polynomial](../../../../../polynomial-split.md) of degree $D_n=(q-1)q^{n-1}$. Modulo $\pi$ it is $T^{D_n}$, and its constant coefficient is exactly $\pi$. Thus the [Eisenstein layers of Lubin–Tate torsion](../../../../../eisenstein-layers-of-lubin-tate-torsion.md) are [Eisenstein polynomials](../../../../../eisenstein-polynomial.md). A root $\lambda_n$ generates a [totally ramified extension](../../../../../totally-ramified-extension.md) of degree $D_n$, and has $v_K(\lambda_n)=1/D_n$ in the uniquely extended [valuation](../../../../../valuation.md). Also $f_{n-1}(\lambda_n)^{q-1}=-\pi\ne0$, so it has exact level $n$.

The map

$$
R/\pi^nR\longrightarrow\Lambda_n,\qquad a\longmapsto[a]_f(\lambda_n)
$$

is well-defined and injective. If $a=\pi^r u$ with $r<n$ and $u$ a [unit](../../../../../unit-in-a-ring.md), then $[a]\lambda_n=[u]f_r(\lambda_n)\ne0$, because $[u]$ is invertible and $\lambda_n$ is primitive. Conversely every multiple of $\pi^n$ kills it. The image therefore contains $q^n$ distinct roots of the degree-$q^n$ [polynomial](../../../../../polynomial-split.md) $f_n$, so it is all of $\Lambda_n$. This proves, without merely assuming the torsion cardinality,

$$
\boxed{\Lambda_n\cong R/\pi^nR\quad\text{as an }R\text{-module}.}
$$

Its primitive generators are exactly $[a]\lambda_n$ with $a\in(R/\pi^nR)^{\times}$.

Define the [Lubin–Tate extension](../../../../../lubin-tate-extension.md) $K_{\pi,n}=K(\Lambda_n)$. Every integral endomorphism series evaluated at $\lambda_n$ converges in the complete field $K(\lambda_n)$, so all torsion points already lie there. Hence

$$
K_{\pi,n}=K(\lambda_n),\qquad [K_{\pi,n}:K]=D_n.
$$

It is the splitting field of $f_n$, which has $q^n$ distinct roots by the [module](../../../../../module-mathematics.md) calculation. Thus it is Galois. Every K-automorphism preserves the uniquely extended [absolute value on a field](../../../../../absolute-value-algebra.md), hence is continuous and commutes with limits of the integral endomorphism series. Its automorphisms therefore commute with the endomorphism action and send a primitive generator to a primitive generator. There is a unique [unit](../../../../../unit-in-a-ring.md) class $a_\sigma$ such that $\sigma(\lambda_n)=[a_\sigma]\lambda_n$. The [Lubin–Tate Galois action on primitive torsion](../../../../../lubin-tate-galois-action-on-primitive-torsion.md) gives an injective homomorphism

$$
\operatorname{Gal}(K_{\pi,n}/K)\longrightarrow(R/\pi^nR)^{\times}.
$$

Both sides have order $D_n=(q-1)q^{n-1}$, so it is an isomorphism. In particular every finite layer is abelian and totally ramified.

For an example, take $K=\mathbb Q_p$, $\pi=p$, and the equally admissible series $f(T)=(1+T)^p-1$. Its [formal group law](../../../../../formal-group-law.md) is the [formal multiplicative group](../../../../../formal-multiplicative-group.md) $F(X,Y)=X+Y+XY$, with $[a](T)=(1+T)^a-1$ for $a\in\mathbb Z_p$. The [binomial polynomials](../../../../../binomial-polynomial.md) make its coefficients integral. Its level-$n$ torsion points are $\zeta-1$ with $\zeta^{p^n}=1$. Thus the [Lubin–Tate cyclotomic example](../../../../../lubin-tate-cyclotomic-example.md) gives $K_{p,n}=\mathbb Q_p(\mu_{p^n})$ and Galois action $\zeta\mapsto\zeta^a$. The order formula includes $p=2,n=1$, when the first field and its [Galois group](../../../../../galois-group.md) are trivial over $\mathbb Q_2$.

Finally choose primitive points compatibly, $[\pi]\lambda_{n+1}=\lambda_n$. They exist by taking a root of $f(T)-\lambda_n$ in the algebraic closure; its roots have positive [valuation](../../../../../valuation.md) and exact level $n+1$. Then $K_{\pi,n}\subseteq K_{\pi,n+1}$, and restriction of Galois automorphisms corresponds to reduction of [unit](../../../../../unit-in-a-ring.md) classes. The [Lubin–Tate tower](../../../../../lubin-tate-tower.md) $K_\pi=\bigcup_nK_{\pi,n}$ consequently has the topological [Galois group](../../../../../galois-group.md)

$$
\boxed{\operatorname{Gal}(K_\pi/K)\cong\varprojlim_n(R/\pi^nR)^{\times}\cong R^{\times}.}
$$

The final isomorphism uses completeness of the [discrete valuation ring](../../../../../discrete-valuation-ring.md) $R$. This computes the finite-layer and infinite-tower Galois groups directly from the formal action and the primitive Eisenstein [polynomials](../../../../../polynomial-split.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 136](../../paper-136-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
