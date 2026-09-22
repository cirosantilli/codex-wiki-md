<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) says that if a nonempty [complete metric space](../../../../../complete-metric-space.md) $(X,d)$ has a map $T:X\to X$ satisfying $d(Tx,Ty)\leq qd(x,y)$ for every $x,y$ and some fixed $0\leq q<1$, then $T$ has a unique fixed point $p$, and $T^n x\to p$ for every starting point. In particular $d(T^n x,p)\leq q^n d(x,p)$; an estimate using only consecutive iterates is $d(T^n x,p)\leq q^n d(x,Tx)/(1-q)$.

Let $s=\sqrt a$ and $T(x)=(x+a/x)/2$ for $x>0$. Direct subtraction gives

$$
T(x)-s=\frac{(x-s)^2}{2x}\geq0.
$$

Thus every iterate after the first lies in $[s,\infty)$. On this interval,

$$
0\leq T'(x)=\frac12\left(1-\frac a{x^2}\right)<\frac12.
$$

The [mean value theorem](../../../../../mean-value-theorem.md) gives a uniform Lipschitz constant $1/2$, and $T$ maps the interval into itself. The interval is closed in $\mathbb R$, hence complete. By the [contraction mapping theorem](../../../../../contraction-mapping-theorem.md), its iterates converge to its unique fixed point, which is $s$. Therefore **every positive initial guess converges to $\sqrt a$**.

The local error $e_n=x_n-s\geq0$ satisfies the sharper exact recursion

$$
\boxed{e_{n+1}=\frac{e_n^2}{2(s+e_n)}\sim\frac{e_n^2}{2s}.}
$$

In relative error $\delta_n=e_n/s$, this is $\delta_{n+1}=\delta_n^2/[2(1+\delta_n)]$. Thus when $\delta_n\approx10^{-d}$, the next relative error is approximately $\tfrac12 10^{-2d}$: one step roughly doubles the number of correct decimal digits. In particular **one further step suffices for one additional digit once the iteration is sufficiently close**. For absolute-error accuracy, the precise sufficient condition $e_n\leq s/5$ gives $e_{n+1}\leq e_n/10$; this states explicitly how close is sufficient when $a$ has an arbitrary scale.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
