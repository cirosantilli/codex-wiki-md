<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The relevant uniqueness is uniqueness of the node set, with $n\ge1$. Reordering the same nodes cannot change a constraint imposed at every node, so an unsorted “different sequence” obtained only by permutation would not give the claimed counterexample. Order the genuinely different nodes as $1\ge t_0>t_1>\cdots>t_n\ge-1$ and let $L_i$ be their [Lagrange cardinal polynomials](../../../../../lagrange-cardinal-polynomial.md):

$$
L_i(x)=\frac{\prod_{j\ne i}(x-t_j)}{\prod_{j\ne i}(t_i-t_j)}.
$$

The denominator has sign $(-1)^i$. For $1\le k\le n$, repeated differentiation of its numerator gives

$$
\left.\frac{d^k}{dx^k}\prod_{j\ne i}(x-t_j)\right|_{x=1}
=k!\sum_{\substack{S\subset\{0,\ldots,n\}\setminus\{i\}\\|S|=n-k}}\prod_{j\in S}(1-t_j).
$$

All products are nonnegative. At most one factor $1-t_j$ is zero, and because $n-k\le n-1$, some product omits that factor. The [derivative](../../../../../derivative.md) is consequently strictly positive, including when $k=n$, for which the product is empty and equals one. This proves the [endpoint derivative signs of Lagrange cardinal polynomials](../../../../../endpoint-derivative-signs-of-lagrange-cardinal-polynomials.md):

$$
\boxed{(-1)^iL_i^{(k)}(1)>0\qquad(1\le k\le n).}
$$

Choose a single [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) by prescribing $q(t_i)=(-1)^i$:

$$
q(x)=\sum_{i=0}^n(-1)^iL_i(x).
$$

It satisfies $|q(t_i)|=1$ at every prescribed node. Its [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) is $\sum_i1/|\prod_{j\ne i}(t_i-t_j)|>0$, so it has degree exactly $n$. The endpoint sign formula gives $q^{(k)}(1)=\sum_i|L_i^{(k)}(1)|$ simultaneously for all $k$.

Interpolate the [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) $T_n$ on the same nodes. Since $|T_n(t_i)|\le1$,

$$
q^{(k)}(1)-T_n^{(k)}(1)
=\sum_{i=0}^n|L_i^{(k)}(1)|\bigl(1-(-1)^iT_n(t_i)\bigr)\ge0.
$$

The only points at which $|T_n|=1$ are its $n+1$ extrema. A different set of $n+1$ distinct nodes includes at least one nonextremal point; at that point the bracket is strictly positive, and so is its [derivative](../../../../../derivative.md) weight for every $k$. Moreover $T_n^{(k)}(1)>0$: differentiating its differential equation gives $T_n^{(k+1)}(1)=(n^2-k^2)T_n^{(k)}(1)/(2k+1)$, beginning with $T_n(1)=1$ and ending at $k=n-1$. Thus

$$
\boxed{\|q^{(k)}\|_\infty\ge q^{(k)}(1)>T_n^{(k)}(1)=|T_n^{(k)}(1)|\quad(1\le k\le n).}
$$

The same $q$ violates every sharp [derivative](../../../../../derivative.md) bound, proving [uniqueness of Chebyshev derivative-norming nodes](../../../../../uniqueness-of-chebyshev-derivative-norming-nodes.md) for the given [Markov-Duffin-Schaeffer theorem](../../../../../duffin-schaeffer-polynomial-derivative-inequality.md). The result concerns node sets or consistently ordered sequences; a mere permutation is the literal ordering exception noted above.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
