<h1 id="6e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At a positive equilibrium of the bounded Hill model, the [mutual repression stability criterion](../../../../../../mutual-repression-stability-criterion.md) becomes

$$
K=mn\frac{y^m}{1+y^m}\frac{x^n}{1+x^n}>1.
$$

Thus $mn>1$ is necessary. Because the same $\lambda$ is imposed in both synthesis functions, it is not sufficient for arbitrary unequal positive exponents. The additional equilibrium constraint is

$$
x(1+y^m)=y(1+x^n),\qquad \frac1y+y^{m-1}=\frac1x+x^{n-1}.
$$

Here is an exact criterion for all the printed exponent choices, including nonintegers. If $m>1$ and $n>1$, multistability is possible: for large $\lambda$ the intermediate equilibrium satisfies $x\sim\lambda^{(m-1)/(mn-1)}$, $y\sim\lambda^{(n-1)/(mn-1)}$, so both increase without bound and $K\to mn>1$. These asymptotics follow by balancing $xy^m\sim\lambda$ and $yx^n\sim\lambda$; the limiting two algebraic equations have a nonsingular log-Jacobian when $mn\ne1$, so a nearby exact equilibrium exists for large $\lambda$. If both exponents are at most one, $K<1$ everywhere and multistability is impossible.

For the remaining case, interchange $x,y$ if necessary so $0<m\le1<n$. For each $x>0$, let $Y(x)>0$ be the unique solution of

$$
Y^{-1}+Y^{m-1}=x^{-1}+x^{n-1},
$$

which exists because the left side is strictly decreasing; for $m=1$ the right side always exceeds one. Define

$$
K_{m,n}(x)=\frac{mn x^nY(x)^m}{(1+x^n)(1+Y(x)^m)}.
$$

Then the exact answer for this remaining range is

$$
\boxed{\text{multistability for some common }\lambda\ \Longleftrightarrow\ \max_{x>0}K_{m,n}(x)>1.}
$$

This is a one-variable test depending only on $m,n$, with no unknown $\lambda$. To prove it, parameterize all equilibria by $\lambda(x)=x(1+Y(x)^m)$. Implicit differentiation gives

$$
\lambda'(x)=\frac{(1+Y^m)(1-K_{m,n}(x))}{1-mY^m/(1+Y^m)}.
$$

The denominator is positive, and $\lambda(x)$ goes from zero to infinity as $x$ goes from zero to infinity. A negative-slope portion therefore forces two folds and an interval of three equilibria, with two attracting branches. If $K\le1$ everywhere, $\lambda$ is strictly increasing apart from possible isolated stationary points, so there is only one equilibrium for each $\lambda$. This is the [common-strength Hill repression criterion](../../../../../../common-strength-hill-repression-criterion.md).

For illustration and a closed test on the boundary $m=1$, $Y=x/(1+x^n-x)$ and

$$
\max K_{1,n}=\frac{(n-1)^2}{4n}\left(\frac{n+1}{n-1}\right)^{(n+1)/n},\qquad n>1,
$$

obtained at $x^n=(n+1)/(n-1)$. In particular $(m,n)=(1,2)$ has $mn>1$ but maximum $3\sqrt3/8<1$, so it cannot be multistable. For positive integer exponents the allowed choices simplify to **both exponents at least two, or one equal to one and the other at least four**. For arbitrary real exponents the preceding exact criterion is needed; replacing it by $mn>1$ would discard the common-strength constraint.

The unbounded power laws behave differently. Combining their equilibrium equations gives $x^{1-mn}=\lambda^{1-m}$. If $mn\ne1$, there is exactly one positive equilibrium,

$$
x=\lambda^{(1-m)/(1-mn)},\qquad y=\lambda^{(1-n)/(1-mn)}.
$$

Its slope product is exactly $mn$, so it is attracting if $mn<1$ and a saddle if $mn>1$, but there are never two isolated attracting equilibria. If $mn=1$, equilibria exist only when $\lambda^{1-m}=1$; when this holds there is a whole curve of equilibria, with a zero tangent [eigenvalue](../../../../../../eigenvalue.md) and transverse [eigenvalue](../../../../../../eigenvalue.md) $-2$. This includes $m=n=1$, $xy=\lambda$, for every $\lambda$. A neutrally degenerate continuum is not [bistability](../../../../../../bistability.md) between isolated attractors. Thus **these power laws do not generate ordinary multistability**; boundedness was essential to the outer-root argument in part (a).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6E](../../6e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
