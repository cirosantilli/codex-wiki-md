<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [abc conjecture](../../../../../../abc-conjecture.md) says that for every $\epsilon>0$ there is $C_\epsilon$ such that [coprime](../../../../../../coprime-integers.md) positive [integers](../../../../../../integer.md) $A+B=C$ satisfy $C\le C_\epsilon\operatorname{rad}(ABC)^{1+\epsilon}$, where the radical is the product of distinct prime [divisors](../../../../../../divisor.md).

The Catalan alternative yields finiteness of actual nontrivial solutions, with $x,y\ge2$ and $p,q\ge3$. Put $M=x^p$, so $y^q=M-1$ and $x,y$ are [coprime](../../../../../../coprime-integers.md). The triple $(y^q,1,x^p)$ has radical at most $xy<M^{2/3}$. Take $\epsilon=1/6$ to obtain

$$
M\le C_{1/6}M^{7/9},\qquad\boxed{M\le C_{1/6}^{9/2}}.
$$

Both bases are bounded, and $2^p\le M$, $2^q\le M-1$ also bound both exponents. Thus **only finitely many nontrivial Catalan solutions exist under abc**, the [Catalan power bound from abc](../../../../../../catalan-power-bound-from-abc.md).

For the Fermat alternative, the usual [arithmetic height](../../../../../../height-function.md) statement concerns primitive solutions, or equivalently solutions modulo common scaling. A primitive positive triple is pairwise [coprime](../../../../../../coprime-integers.md), and $x,y<z$. Applying abc to $(x^n,y^n,z^n)$ gives

$$
z^n\le C_{1/6}(xyz)^{7/6}<C_{1/6}z^{7/2},\qquad\boxed{z\le C_{1/6}^2\quad(n\ge4)}.
$$

This is uniform even in $n$. If $h=\max(x,y)<z$, then $z^n=x^n+y^n\le2h^n$, so $n\le\log2/\log(z/h)$ is bounded after $z$ is bounded. There are therefore finitely many primitive triples and exponents, the [primitive Fermat bound from abc](../../../../../../primitive-fermat-bound-from-abc.md). Without the primitive convention, any one nonzero homogeneous solution would produce infinitely many common multiples. The Catalan proof above supplies the requested literal finiteness alternative without that normalization issue.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
