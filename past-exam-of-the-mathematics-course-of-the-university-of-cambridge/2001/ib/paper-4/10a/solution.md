<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

Set $e_n(x)=|f_n(x)-f(x)|$. The functions $e_n$ are [continuous](../../../../../continuous-function.md), converge pointwise to zero, and decrease with $n$. This remains true even if the direction of monotonicity of $f_n(x)$ differs between points: at each fixed point a monotone convergent real sequence approaches its limit from one side.

Given $\varepsilon>0$, the sets $U_n=\{x:e_n(x)<\varepsilon\}$ are relatively open in $[a,b]$, increase with $n$, and cover the interval. [Compactness](../../../../../compact-space.md) gives a finite subcover; choosing the largest index in it gives $U_N=[a,b]$. For every $n\ge N$ and every $x$, $e_n(x)\le e_N(x)<\varepsilon$. Hence **$f_n\to f$ uniformly**. This proves the required version of [Dini's theorem](../../../../../dini-s-theorem.md), rather than assuming a common direction of monotonicity everywhere.

On $[0,1)$, take $f_n(x)=x^n$. Each function and its pointwise limit $f=0$ are [continuous](../../../../../continuous-function.md), and the sequence decreases at every point. Nevertheless

$$
\boxed{\sup_{0\le x<1}|f_n(x)-0|=1\quad\text{for every }n.}
$$

Thus [uniform convergence](../../../../../uniform-convergence.md) fails on the noncompact interval although all the other conditions hold.

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
