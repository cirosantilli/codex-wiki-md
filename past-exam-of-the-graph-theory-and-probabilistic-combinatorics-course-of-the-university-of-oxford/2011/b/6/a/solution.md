<h1 id="b/6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Galton-Watson process](../../../../../galton-watson-process-split.md) starts with one ancestor, $X_0=1$. Given generation size $X_r$, define

$$
X_{r+1}=\sum_{j=1}^{X_r}Z_{r,j},
$$

where all offspring variables are [independent](../../../../../independent-random-variables.md) with common distribution $Z$. The empty sum is zero, so zero is absorbing. Its [extinction](../../../../../extinction.md) [probability](../../../../../probability.md) is

$$
\eta=\mathbb P(\exists r:X_r=0)=\lim_{r\to\infty}\mathbb P(X_r=0).
$$

For the [probability generating function](../../../../../probability-generating-function.md) $f(s)=\mathbb E[s^Z]$, the allowed fixed-point characterization is

$$
\boxed{\eta\text{ is the smallest solution in }[0,1]\text{ of }f(s)=s.}
$$

For binomial offspring, $f(s)=(1-p+ps)^k$, with $f(1)=1$, $f'(1)=kp$, and $f$ [convex](../../../../../convex-function.md) on $[0,1]$.

First assume $0<p<1$. If $k=0$, [extinction](../../../../../extinction.md) occurs immediately. For $k=1$, $f(s)-s=(1-p)(1-s)>0$ for $s<1$, so the only [fixed point](../../../../../fixed-point.md) is one. For $k\geq2$, [strict convexity](../../../../../strictly-convex-function.md) gives

$$
f(s)>f(1)+f'(1)(s-1)=1+kp(s-1)\qquad(0\leq s<1).
$$

If $kp\leq1$, the right-hand side is at least $s$, so no [fixed point](../../../../../fixed-point.md) below one exists and $\eta=1$. If $kp>1$, $f(s)-s<0$ for $s$ just below one, whereas $f(0)>0$. [Continuity](../../../../../continuous-function.md) supplies a [fixed point](../../../../../fixed-point.md) in $(0,1)$; hence $\eta<1$. Thus in the nondegenerate parameter range,

$$
\boxed{0<p<1:\quad\eta<1\iff kp>1.}
$$

For completeness, if binomial endpoint parameters are allowed, $p=0$ or $k=0$ gives $\eta=1$, while $p=1$ and $k\geq1$ gives deterministic positive offspring and $\eta=0$. In particular $(k,p)=(1,1)$ survives forever despite [mean](../../../../../expected-value-split.md) one. Over $k\in\{0,1,\ldots\}$ and $p\in[0,1]$, the full condition is

$$
\boxed{\eta<1\iff kp>1\text{ or }(k,p)=(1,1).}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
