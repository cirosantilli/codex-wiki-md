<h1 id="10d/solution">Solution</h1>

↑ **Parent:** [10D](../10d.md)

Let $f:[a,b]\to\mathbb R$ be continuous. If it were unbounded, one could choose $x_n\in[a,b]$ with $|f(x_n)|>n$. The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) gives a subsequence $x_{n_j}\to x\in[a,b]$, but continuity would then give $f(x_{n_j})\to f(x)$, contradicting unboundedness.

Now let $M=\sup f([a,b])$. Choose $x_n$ with $f(x_n)>M-1/n$. A convergent subsequence and continuity give $f(x)=M$ at its limit. Applying the same argument to $-f$ shows that the infimum is attained. This proves the [extreme value theorem](../../../../../extreme-value-theorem.md) on a closed bounded interval.

The function

$$
\phi(x)=x\qquad(0<x<1)
$$

is continuous and bounded, but attains neither its infimum $0$ nor its supremum $1$. For the second example, enumerate the rationals in $[0,1]$ as $(q_n)$ and set

$$
\psi(x)=
\begin{cases}
n,&x=q_n,\\
0,&x\notin\mathbb Q.
\end{cases}
$$

Every [nondegenerate interval](../../../../../nondegenerate-interval.md) contains infinitely many [rational numbers](../../../../../rational-number.md), hence some $q_n$ with arbitrarily large $n$; therefore $\psi$ is [unbounded](../../../../../unbounded-function.md) on every such interval.

For the running extrema, compactness lets us write

$$
m(x)=\min_{a\leq\xi\leq x}f(\xi),\qquad
M(x)=\max_{a\leq\xi\leq x}f(\xi).
$$

The function $f$ is [uniformly continuous](../../../../../uniform-continuity.md) on $[a,b]$. Given $\varepsilon>0$, choose $\delta>0$ such that $|f(u)-f(v)|<\varepsilon$ whenever $|u-v|<\delta$. If $x<y$ and $y-x<\delta$, every new value $f(\xi)$ with $x\leq\xi\leq y$ is at most $f(x)+\varepsilon\leq M(x)+\varepsilon$. Since $M(y)\geq M(x)$,

$$
0\leq M(y)-M(x)\leq\varepsilon.
$$

Interchanging $x,y$ handles the other order. Applying this argument to $-f$ proves continuity of $m$ as well.

Finally fix $T>0$ and put $h(x)=g(x+T)-g(x)$. For each positive integer $n$, there must be some $x_n>n$ with $|h(x_n)|<1/n$. Otherwise, for some $n$ the continuous function $h$ would satisfy $|h(x)|\geq1/n$ on the interval $(n,\infty)$. By the [intermediate value theorem](../../../../../intermediate-value-theorem.md), $h$ would have a constant sign there. The values

$$
g(x),g(x+T),g(x+2T),\ldots
$$

would then increase or decrease by at least $1/n$ at every step, contradicting boundedness of $g$. Thus $x_n\to\infty$ and

$$
\boxed{g(x_n+T)-g(x_n)\to0}.
$$

## ↑ Ancestors (10)

1. [10D](../10d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
