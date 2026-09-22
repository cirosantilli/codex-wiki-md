<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

A subset $U\subseteq\mathbb R^n$ is an [open set](../../../../../open-set.md) when every $x\in U$ has some radius $r>0$ for which $B(x,r)\subseteq U$. If a [continuous function](../../../../../continuous-function.md) takes only the values zero and one, continuity at $x$ with tolerance $1/2$ gives a neighborhood on which $|f(y)-f(x)|<1/2$. The two possible values differ by one, so $f(y)=f(x)$ throughout that neighborhood. Thus $f$ is [locally constant](../../../../../locally-constant-function.md), and the zero [linear map](../../../../../linear-map.md) is its [derivative](../../../../../derivative.md), since the difference $f(x+h)-f(x)$ is exactly zero for all sufficiently small $h$. Hence **$Df_x=0$ everywhere**.

For the bound on $g$, parametrize the segment by $\gamma(t)=b+t(a-b)$, $0\le t\le1$. The [chain rule](../../../../../chain-rule.md) gives

$$
(g\circ\gamma)'(t)=(Dg)_{\gamma(t)}(a-b),\qquad |(g\circ\gamma)'(t)|\le M\|a-b\|
$$

by the definition of [operator norm](../../../../../operator-norm.md). The [mean value theorem](../../../../../mean-value-theorem.md) applied to the real function $g\circ\gamma$ proves

$$
\boxed{|g(a)-g(b)|\le M\|a-b\|.}
$$

If the endpoints agree the estimate is immediate. No continuity of the [derivative](../../../../../derivative.md) is required.

For the finite-line complement, each removed line $\ell_i$ is closed, so $V$ is open. Because $a,b\notin\ell_i$, there is a unique affine plane $P_i$ containing $a$ and $\ell_i$, and a unique affine plane $Q_i$ containing $b$ and $\ell_i$. Choose $c$ outside the union of these finitely many planes, using the permitted fact about finite plane covers. In particular $c\in V$. If $[a,c]$ met $\ell_i$ at a point $d$, then $d\ne a$, and the line through $a,d$ lies in $P_i$. Since $c$ is on that same line, it would belong to $P_i$, a contradiction. The same argument using $Q_i$ applies to $[c,b]$. Thus **$a$ and $b$ can be joined in $V$ by these two segments**, proving [polygonal connectivity of a finite-line complement](../../../../../polygonal-connectivity-of-a-finite-line-complement.md).

Finally a continuous $f:V\to\{0,1\}$ has zero [derivative](../../../../../derivative.md) by the first argument. Apply the proved segment estimate with $M=0$ separately on $[a,c]$ and $[c,b]$. It gives $f(a)=f(c)=f(b)$. Since $a,b$ were arbitrary, **$f$ is constant on $V$**.

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
