<h1 id="11g/solution">Solution</h1>

↑ **Parent:** [11G](../11g.md)

A [Euclidean domain](../../../../../euclidean-domain.md) is an [integral domain](../../../../../integral-domain.md) $R$ with a function $\nu:R\setminus\{0\}\to\mathbb N$ such that, for any $a,b\in R$ with $b\ne0$, there are $q,r\in R$ satisfying $a=bq+r$ and either $r=0$ or $\nu(r)<\nu(b)$. To prove that every [ideal](../../../../../ideal.md) is principal, take a nonzero ideal $J$ and choose a nonzero $b\in J$ of minimal Euclidean value. Divide any $a\in J$ by $b$. The remainder belongs to $J$, so minimality forces it to be zero. Thus $J=(b)$; the zero ideal is also principal. Hence **every Euclidean domain is a [principal ideal domain](../../../../../principal-ideal-domain.md)**.

In $R=\mathbb Z[\sqrt{-7}]$, consider $J=(2,1+\sqrt{-7})$. It is proper: the map $R\to\mathbb F_2$ sending $\sqrt{-7}$ to one is a well-defined surjective ring map, and annihilates both generators. Suppose $J=(\eta)$. The positive integer [field norm](../../../../../field-norm.md) $N(a+b\sqrt{-7})=a^2+7b^2$ is multiplicative, and $\eta$ divides two. Therefore $N(\eta)$ divides four. A proper ideal cannot have a unit generator, so $N(\eta)\ne1$. There is no element of norm two. The elements of norm four are only $\pm2$, but neither divides $1+\sqrt{-7}$ in this ring. This is a contradiction. Thus

$$
\boxed{\mathbb Z[\sqrt{-7}]\text{ is not a principal ideal domain, hence not Euclidean for any Euclidean function}.}
$$

The argument does not merely show failure of one proposed norm.

Now put $\omega=(1+\sqrt{-7})/2$ and $R'=\mathbb Z[\omega]$. Its algebraic [field norm](../../../../../field-norm.md) is

$$
N(a+b\omega)=a^2+ab+2b^2\in\mathbb N,
$$

since $\omega\overline\omega=2$ and $\omega+\overline\omega=1$. To construct Euclidean division, let $z\in\mathbb C$. Choose an integer $b$ so that $|\operatorname{Im}z-b\sqrt7/2|\le\sqrt7/4$, then choose an integer $a$ so that $|\operatorname{Re}z-b/2-a|\le1/2$. The lattice point $q=a+b\omega$ satisfies

$$
|z-q|^2\le\frac14+\frac7{16}=\frac{11}{16}<1.
$$

For $A,B\in R'$ with $B\ne0$, apply this construction to $z=A/B$, and set $r=A-Bq\in R'$. Multiplicativity gives $N(r)=N(B)|z-q|^2<N(B)$ unless $r=0$. Therefore

$$
\boxed{\mathbb Z[(1+\sqrt{-7})/2]\text{ is Euclidean for }N(z)=z\overline z.}
$$

This is the geometric division argument for the [norm-Euclidean integers of discriminant minus seven](../../../../../norm-euclidean-integers-of-discriminant-minus-seven.md).

## ↑ Ancestors (10)

1. [11G](../11g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
