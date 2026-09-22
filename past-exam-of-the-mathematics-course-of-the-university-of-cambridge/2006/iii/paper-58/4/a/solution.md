<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The best classical strategy avoids previously failed inputs: inspect a uniformly random permutation. Assume $1\le m\le N$ and let $K$ be the first marked position. For $K=k$, the first $k-1$ guesses must all fail and the next must succeed. Thus

$$
\boxed{\mathbb P(K=k)=
\left[\prod_{r=0}^{k-2}\frac{N-m-r}{N-r}\right]\frac{m}{N-k+1}
=\frac{\binom{N-k}{m-1}}{\binom Nm}.}
$$

The empty product covers $k=1$. The binomial form follows by choosing the $m$ marked positions uniformly: put one at $k$ and the remaining $m-1$ after it. This is the [first marked item in a random permutation](../../../../../../first-marked-item-in-a-random-permutation.md) distribution.

The requested range is part of its support, but omits the last possible value $k=N-m+1$. All $N-m$ bad inputs can be encountered first, after which success is certain. The same formula includes that nonzero terminal probability; summing through this last value gives one. If $m=0$, the search never succeeds. If sampling were instead with replacement, its inferior repeated-guess strategy would have the geometric law $(1-m/N)^{k-1}m/N$ with no such finite endpoint.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
