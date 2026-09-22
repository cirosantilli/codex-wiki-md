<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In this setting a [formal group law](../../../../../formal-group-law.md) means a one-dimensional commutative series $F(X,Y)\in R[[X,Y]]$ with identity zero and

$$
F(X,0)=X,\quad F(0,Y)=Y,\quad F(X,Y)=F(Y,X),\quad F(F(X,Y),Z)=F(X,F(Y,Z)).
$$

It starts with $X+Y$; there is a unique inverse series $\iota(T)=-T+\cdots$ satisfying $F(T,\iota(T))=0$. For coefficients in $\mathbb Z$, the series and its inverse converge on $p\mathbb Z_p$, making this ideal a topological [abelian group](../../../../../abelian-group.md) under $F$.

Set $a(T)=\partial_YF(T,0)\in1+T\mathbb Z[[T]]$, and write $a(T)^{-1}=\sum_{j\ge0}b_jT^j$. The [formal logarithm](../../../../../formal-logarithm.md) is

$$
L(T)=\int_0^T\frac{dU}{a(U)}=T+\sum_{j\ge1}\frac{b_j}{j+1}T^{j+1}\in\mathbb Q[[T]].
$$

Differentiate associativity in the third variable at zero. It gives $a(F(X,Y))=\partial_YF(X,Y)a(Y)$, so $\partial_YL(F(X,Y))=L'(Y)$. Subtracting $L(Y)$ leaves a series independent of $Y$, whose value at zero is $L(X)$. Thus **$L(F(X,Y))=L(X)+L(Y)$**.

For odd $p$, the logarithm converges on $I=p\mathbb Z_p$: the valuation of its degree-$n$ term is at least $n-v_p(n)$, which tends to infinity. Put $u(T)=L(T)-T$. For $x,y\in I$, factor $x^n-y^n$ to obtain

$$
v_p\left(\frac{b_{n-1}}n(x^n-y^n)\right)\ge v_p(x-y)+n-1-v_p(n)\ge v_p(x-y)+1
$$

for every $n\ge2$ and odd $p$. Hence $u$ is a contraction with constant at most $1/p$ and maps $I$ into $pI$. The equation $L(x)=z$ is equivalent to $x=z-u(x)$; the [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) gives a unique solution in $I$ for every $z\in I$. The same estimate shows $|L(x)-L(y)|_p=|x-y|_p$, so the logarithm is a topological group isomorphism. Dividing its values by $p$ gives

$$
\boxed{F(p\mathbb Z_p)\cong(p\mathbb Z_p,+)\cong(\mathbb Z_p,+)\qquad(p\text{ odd}).}
$$

This is the [deep logarithm subgroup of a formal group](../../../../../deep-logarithm-subgroup-of-a-formal-group.md) argument, here with depth one.

For $p=2$, the degree-two estimate at depth one need not be strict. At depth two, however,

$$
2(n-1)-v_2(n)\ge1\qquad(n\ge2),
$$

so the same proof gives **$F(4\mathbb Z_2)\cong(4\mathbb Z_2,+)\cong\mathbb Z_2$**. This subgroup has index two in $F(2\mathbb Z_2)$, because $F(x,y)\equiv x+y\pmod4$ when $x,y\in2\mathbb Z_2$.

Indeed the [topological structure of a formal group on twice the 2-adic integers](../../../../../topological-structure-of-a-formal-group-on-twice-the-2-adic-integers.md) has just two possibilities. Let $G=F(2\mathbb Z_2)$, let its index-two subgroup $H$ have topological generator $h$, and choose $v\notin H$. Write $2v=c h$, with $c\in\mathbb Z_2$, using group notation. If $c$ is odd, $2v$ generates $H$ and $v$ generates $G$, giving $G\cong\mathbb Z_2$. If $c$ is even, $v-(c/2)h$ has order two and lies outside $H$, giving $G\cong H\times\mathbb Z/2\mathbb Z$. The $\mathbb Z_2$ multiples are defined by continuity in this compact pro-two group.

For explicit contrasting examples, the [formal additive group](../../../../../formal-additive-group.md) $F_a(X,Y)=X+Y$ gives $F_a(2\mathbb Z_2)\cong\mathbb Z_2$, which is a [torsion-free group](../../../../../torsion-free-group.md). The [formal multiplicative group](../../../../../formal-multiplicative-group.md) $F_m(X,Y)=X+Y+XY$ is identified by $x\mapsto1+x$ with $1+2\mathbb Z_2$. Its element $x=-2$ corresponds to $-1$ and has order two. Moreover

$$
1+2\mathbb Z_2=\{\pm1\}\times(1+4\mathbb Z_2),
$$

and the logarithm identifies the second factor with $4\mathbb Z_2$. **The two resulting groups are $\mathbb Z_2$ and $\mathbb Z/2\mathbb Z\times\mathbb Z_2$, so they are not isomorphic.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
