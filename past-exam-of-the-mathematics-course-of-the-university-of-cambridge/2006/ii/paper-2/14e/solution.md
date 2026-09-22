<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

A [horseshoe for an interval map](../../../../../horseshoe-for-an-interval-map.md) consists of an [open interval](../../../../../open-interval.md) $J$ containing two disjoint open subintervals each mapped onto $J$. [Glendinning chaos](../../../../../glendinning-chaos.md) means that some positive iterate has a horseshoe.

Solving on the appropriate branches of the [tent map](../../../../../tent-map.md) gives

$$
\boxed{x_0=\frac{\mu}{\mu+1},\quad x_{-1}=\frac1{\mu+1},\quad x_{-2}=1-\frac1{\mu(\mu+1)}.}
$$

Here $F(x_{-2})=x_{-1}$ and $F(x_{-1})=x_0$. On $J=[x_{-1},x_0]$ the second iterate is

$$
G(x)=\begin{cases}\mu-\mu^2x,&x\le1/2,\\\mu-\mu^2+\mu^2x,&x\ge1/2.\end{cases}
$$

Both endpoints map to $x_0$, and the minimum is $v=\mu-\mu^2/2$. Both monotone branches cover $J$ when $v\le x_{-1}$, equivalently $(\mu-1)(\mu^2-2)\ge0$. Restricting them to preimages of the interior proves **a horseshoe for $F^2$ when $\mu\ge\sqrt2$**.

<a id="14e/image-the-tent-map-and-its-second-iterate-with-the-fixed-point-and-its-indicated-preimages"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2-tent-iterates.png)

**[Figure 2](#14e/image-the-tent-map-and-its-second-iterate-with-the-fixed-point-and-its-indicated-preimages). The tent map and its second iterate with the fixed point and its indicated preimages**.

For $1<\mu\le\sqrt2$, $G(J)\subseteq J$. Set $d=(\mu-1)/(\mu+1)$ and $h(x)=(x_0-x)/d$. This maps $J$ onto $[0,1]$; substitution in each linear piece gives $hGh^{-1}=F_{\mu^2}$. The [renormalization of the tent map near its fixed point](../../../../../renormalization-of-the-tent-map-near-its-fixed-point.md) therefore makes $F^4$ conjugate on $J$ to $F_{\mu^2}^2$. Applying the preceding threshold proves its horseshoe when $2^{1/4}\le\mu<\sqrt2$.

For $\mu\ge\sqrt2$, the inverse branch of $G$ fixing $x_0$ contracts distance to $x_0$ by $\mu^{-2}$. Compose $m$ copies of it with the other inverse branch. This contraction has a [fixed point](../../../../../fixed-point.md) with a periodic itinerary, distinct from $x_0$ and at distance $O(\mu^{-2m})$. Hence nontrivial periodic points accumulate at $x_0$.

For $\mu<\sqrt2$, the conjugate tent parameter $\nu=\mu^2<2$ has every nonzero periodic point in $[\nu-\nu^2/2,\nu/2]$. This interval is forward invariant; below it, a nonzero point increases until entering it. The positive lower bound separates those periodic points from zero, which corresponds to $x_0$. Thus no nontrivial periodic points are sufficiently close to $x_0$ from the left. A point sufficiently close on the right maps to such a left-hand point; periodicity would pass to its image and is impossible. Thus **$x_0$ is isolated among periodic points**, even though a fourth-iterate horseshoe exists elsewhere.

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
