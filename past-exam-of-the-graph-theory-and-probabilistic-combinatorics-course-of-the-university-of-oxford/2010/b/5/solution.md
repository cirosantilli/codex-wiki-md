<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Start the [Galton-Watson process](../../../../galton-watson-process-split.md) with one ancestor, $Z_0=1$, and let every individual independently have a number of offspring distributed as $Z$. With independent copies $Z_{t,j}$,

$$
Z_{t+1}=\sum_{j=1}^{Z_t}Z_{t,j},
$$

where an empty sum is zero. Extinction is the event that some generation is empty; zero is then absorbing. Write $q$ for its [probability](../../../../probability.md) and $1-q$ for the survival [probability](../../../../probability.md).

Set $q_t=P(Z_t=0)$, with $q_0=0$. Conditional on the ancestor's number of children, extinction by generation $t+1$ requires independent extinction by generation $t$ in every child subtree. Thus

$$
q_{t+1}=f_Z(q_t),\qquad f_Z(s)=\mathbb E(s^Z).
$$

The events $\{Z_t=0\}$ increase, so $q_t\uparrow q$. The [probability generating function](../../../../probability-generating-function.md) is continuous on $[0,1]$, by domination of $s^Z$ by $1$, giving $q=f_Z(q)$. If $r\in[0,1]$ is any [fixed point](../../../../fixed-point.md), then $q_0=0\leq r$ and monotonicity of $f_Z$ inductively gives $q_t\leq r$. Taking limits proves the [Galton-Watson extinction fixed point](../../../../galton-watson-extinction-fixed-point.md) characterization:

$$
\boxed{q=\min\{s\in[0,1]:f_Z(s)=s\}.}
$$

In particular it is the smallest nonnegative [fixed point](../../../../fixed-point.md) wherever the generating series is defined, since it already lies in $[0,1]$.

Let $m=\mathbb EZ=f_Z'(1-)$, allowing $m=\infty$. The [probability generating function](../../../../probability-generating-function.md) is increasing and convex, with $f_Z(1)=1$. If $m<1$, its tangent inequality gives $f_Z(s)\geq1+m(s-1)>s$ for $s<1$, so $q=1$. If $m=1$ and $P(Z=1)\neq1$, there is positive mass at both zero and some integer at least two; strict convexity gives $f_Z(s)>s$ for $s<1$, again $q=1$. The exceptional case $Z=1$ almost surely has one individual forever, so $q=0$ despite $m=1$.

If $m>1$, the left [derivative](../../../../derivative.md) at $1$ gives $f_Z(s)-s<0$ for $s<1$ sufficiently close to $1$. Since $f_Z(0)\geq0$, [continuity](../../../../continuous-function.md) supplies a [fixed point](../../../../fixed-point.md) below $1$, possibly $0$. Thus **survival has positive [probability](../../../../probability.md) precisely when $m>1$, apart from deterministic one-child reproduction**.

For the random [bipartite graph](../../../../bipartite-graph-split.md), early exploration of a component alternates between the two [vertex](../../../../vertex-graph-theory.md) classes. Before many vertices are exposed, each discovered [vertex](../../../../vertex-graph-theory.md) has approximately $\operatorname{Poisson}(c)$ new neighbors in the other class, since $\operatorname{Bin}(n-O(1),c/n)$ tends to that distribution. The two-type mean offspring matrix is

$$
M=\begin{pmatrix}0&c\\c&0\end{pmatrix},
$$

with [spectral radius](../../../../spectral-radius.md) $c$; equivalently, the mean growth over two generations is $c^2$. The branching-process comparison therefore predicts a [giant component](../../../../giant-component.md) exactly when

$$
\boxed{c>1.}
$$

For $c\leq1$, the local process dies out almost surely, so no linear-sized component is expected; $c=1$ is the critical case, not a positive-survival exception. For $c>1$, the symmetric survival [probability](../../../../probability.md) is $1-q>0$, where $q=e^{c(q-1)}$, predicting approximately $2n(1-q)$ vertices in the giant. This last passage from local survival to a unique giant is the usual random-[graph](../../../../graph-split.md) exploration argument; the branching-process reasoning here supplies the requested threshold explanation rather than a proof of that global theorem.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../split.md)
5. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
