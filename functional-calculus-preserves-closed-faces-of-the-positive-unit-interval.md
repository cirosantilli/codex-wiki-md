# Functional calculus preserves closed faces of the positive unit interval

↑ **Parent:** [Face of a convex set](face-of-a-convex-set.md)

Let $F$ be a nonempty [norm](norm.md)-closed [face of a convex set](face-of-a-convex-set.md) $[0,1_A]$ in a unital [C-star algebra](c-star-algebra.md), with $0\notin F$. Every $a\in F$ has [norm](norm.md) one: otherwise $a=\|a\|(a/\|a\|)+(1-\|a\|)0$ is a nontrivial [convex](convex-function.md) decomposition forcing zero into the face. If $g:[0,1]\to[0,1]$ is continuous and nondecreasing with $g(0)=0,g(1)=1$, then $g(a)\in F$.

To prove this, for $n\geq2$ replace $g$ near the endpoints by a function $g_n$ which is zero on $[0,1/(2n)]$, one on $[1-1/(2n),1]$, agrees with $g$ on $[1/n,1-1/n]$, and interpolates linearly in between. Monotonicity and endpoint continuity give $g_n\to g$ uniformly. With $\delta=1/(2n)$, the function $h_n(t)=(t-\delta g_n(t))/(1-\delta)$ takes values in $[0,1]$: check the two constant regions and use $\delta\leq t\leq1-\delta$ elsewhere. The [continuous functional calculus](continuous-functional-calculus.md) gives $a=\delta g_n(a)+(1-\delta)h_n(a)$ with both summands positive contractions. The face property gives $g_n(a)\in F$, and closedness gives $g(a)\in F$.

## ↑ Ancestors (6)

1. [Face of a convex set](face-of-a-convex-set.md)
2. [Convex set](convex-set-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
