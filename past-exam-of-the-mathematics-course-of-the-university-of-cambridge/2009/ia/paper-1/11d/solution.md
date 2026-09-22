<h1 id="11d/solution">Solution</h1>

↑ **Parent:** [11D](../11d.md)

[Rolle's theorem](../../../../../rolle-theorem.md) states that a [continuous function](../../../../../continuous-function.md) $f:[a,b]\to\mathbb R$, differentiable on $(a,b)$ with $a<b$ and $f(a)=f(b)$, has $f'(c)=0$ for some $c\in(a,b)$. If $f$ is constant this is immediate. Otherwise the [extreme value theorem](../../../../../extreme-value-theorem.md) supplies a maximum or minimum with value different from the common endpoint value, so one such extremum occurs in $(a,b)$. At an interior maximum, the difference quotients for positive increments are nonpositive and those for negative increments are nonnegative. Their common limit, the [derivative](../../../../../derivative.md), must be zero. At a minimum the inequalities reverse, with the same conclusion. This proves [Rolle's theorem](../../../../../rolle-theorem.md).

For the two-function identity, write $\Delta f=f(b)-f(a)$ and $\Delta g=g(b)-g(a)$, and set $\phi(x)=g(x)\Delta f-f(x)\Delta g$. This is a [continuous function](../../../../../continuous-function.md) on the closed interval and is differentiable inside it. Its endpoint values agree:

$$
\phi(a)=\phi(b)=g(a)f(b)-f(a)g(b).
$$

They need not be zero, but [Rolle's theorem](../../../../../rolle-theorem.md) only requires equality. At the resulting point $c$,

$$
0=\phi'(c)=g'(c)\Delta f-f'(c)\Delta g,
$$

which proves the [Cauchy mean value theorem](../../../../../cauchy-mean-value-theorem.md) identity

$$
\boxed{f'(c)(g(b)-g(a))=g'(c)(f(b)-f(a)).}
$$

For the final endpoint limit, first state the denominator convention explicitly. In the usual zero-over-zero version of [L'Hopital rule](../../../../../l-hopital-s-rule.md), $g'(x)\ne0$ on some whole interval $(0,\delta)$; this is understood if the displayed derivative quotient is to be a function defined throughout a deleted right neighborhood of zero. Define $f(0)=g(0)=0$, making both functions continuous at zero. For $0<x<\delta$, [Rolle's theorem](../../../../../rolle-theorem.md) implies $g(x)\ne0$, since otherwise $g$ would have equal zero values at $0$ and $x$ and a zero [derivative](../../../../../derivative.md) between them. Apply the proved [Cauchy mean value theorem](../../../../../cauchy-mean-value-theorem.md) on $[0,x]$ to obtain $c_x\in(0,x)$ with

$$
f(x)g'(c_x)=f'(c_x)g(x),\qquad \frac{f(x)}{g(x)}=\frac{f'(c_x)}{g'(c_x)}.
$$

Given $\varepsilon>0$, the hypothesis on the derivative quotient supplies $\eta>0$ such that its distance from $\ell$ is less than $\varepsilon$ whenever $0<t<\eta$. If $0<x<\min(\eta,\delta)$ then $0<c_x<x<\eta$, so the same bound holds for $f(x)/g(x)$. Therefore

$$
\boxed{\lim_{x\to0^+}\frac{f(x)}{g(x)}=\ell.}
$$

No continuity of the [derivatives](../../../../../derivative.md) is needed.

The PDF does not explicitly state the nonvanishing condition on $g'$. If “the limit exists” permits a limit only along the natural domain where $g'\ne0$, the assertion is false, even with $g>0$ everywhere. The distinction concerns [derivative quotient limits on partial domains](../../../../../derivative-quotient-limits-on-partial-domains.md). Here is a concrete counterexample to that weaker reading. Put $x_n=2^{-n}$ and $h_n=4^{-n}$ for $n\ge0$. On each interval $[x_n/2,x_n]$, split off the plateau $[3x_n/4,x_n]$. On the plateau set

$$
g(x)=h_n,\qquad f(x)=h_nq\left(\frac{x-3x_n/4}{x_n/4}\right),\qquad q(u)=16u^2(1-u)^2.
$$

On the transition interval $[x_n/2,3x_n/4]$ set

$$
g(x)=h_{n+1}+(h_n-h_{n+1})S\left(\frac{x-x_n/2}{x_n/4}\right),\qquad f(x)=0,\qquad S(u)=3u^2-2u^3.
$$

Extend $g=1,f=0$ for $x\ge1$. The endpoints fit because $S(0)=0$, $S(1)=1$, while both $S'$ and $q'$ vanish at zero and one and $q$ also vanishes there. Thus $f,g$ are differentiable for all $x>0$ and tend to zero at zero. The [derivative](../../../../../derivative.md) $g'$ is nonzero exactly inside the transition intervals, where $f'=0$, so the derivative quotient has natural-domain limit zero. But $f(x_n)/g(x_n)=0$, whereas $f(7x_n/8)/g(7x_n/8)=1$. Hence $f/g$ has no limit. The preceding qualified proof is the intended valid form of [L'Hopital rule](../../../../../l-hopital-s-rule.md).

## ↑ Ancestors (10)

1. [11D](../11d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
