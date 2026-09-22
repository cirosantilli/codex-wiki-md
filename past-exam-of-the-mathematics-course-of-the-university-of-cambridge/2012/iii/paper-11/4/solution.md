<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The key is to widen the forbidden intersection while controlling a product of densities. We first derive the two ingredients, with constants explicit enough to yield the numerical base in the question.

For two nonempty [set families](../../../../../set-family.md) $\mathcal F,\mathcal G$ on $m$ coordinates, suppose every cross-intersection has size greater than an integer $w\geq0$. Their complements are separated from $\mathcal F$ by [Hamming distance](../../../../../hamming-distance.md) greater than $w$. Let $a$ be the least integer with $|\mathcal F|\leq S_m(a)$, where $S_m(a)=\sum_{j=0}^a\binom mj$. Iterating [Harper inequality](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md), and using $|\mathcal F|>S_m(a-1)$, shows that its radius-$w$ neighbourhood has at least $S_m(a+w-1)$ [vertices](../../../../../vertex-graph-theory.md). The complementary [set family](../../../../../set-family.md) is disjoint from that neighbourhood, so

$$
|\mathcal F||\mathcal G|\leq S_m(a)S_m(m-a-w).
$$

For $a=0$ the needed weaker neighbourhood bound follows simply by taking the ball around its single [vertex](../../../../../vertex-graph-theory.md); define $S_m(-1)=0$. If a displayed index forces a full neighbourhood, the other [set family](../../../../../set-family.md) would be empty, already excluded.

The provided [binary entropy function](../../../../../binary-entropy-function.md) bound gives

$$
S_m(t)\leq2^m\exp\left[-\frac{2}{m}(m/2-t)_+^2\right].
$$

Indeed, for $t\leq m/2$ this follows from $H_2(1/2-v)\leq1-2v^2/\log2$, obtained by integrating $H_2''\leq-4/\log2$; for larger $t$ use $S_m(t)\leq2^m$. The two nonnegative deficits in the preceding product have sum at least $w$. Their squared sum is at least $w^2/2$. Thus the [cross-intersection bound from cube separation](../../../../../cross-intersection-bound-from-cube-separation.md) is

$$
\boxed{\mu_m(\mathcal F)\mu_m(\mathcal G)\leq e^{-w^2/m}},
\qquad \mu_m(\mathcal F)=|\mathcal F|/2^m.
$$

Now suppose a pair of [set families](../../../../../set-family.md) forbids every cross-intersection in $[a,b]\subseteq[0,m]$. Put $\rho=\mu_m(\mathcal F)\mu_m(\mathcal G)$, and fix $\delta=1/50$. Split both [set families](../../../../../set-family.md) by the last coordinate. The following three replacements preserve the indicated forbidden intervals on $m-1$ coordinates:

$$
\begin{array}{c|c}
\text{new families}&\text{new forbidden interval}\\\hline
(\mathcal F_1,\mathcal G_1)&[a-1,b-1]\\
(\mathcal F_0,\mathcal G_0\cup\mathcal G_1)&[a,b]\\
(\mathcal F_1,\mathcal G_0\cap\mathcal G_1)&[a-1,b]
\end{array}
$$

For example, in the third row the same second set has witnesses in both sections of $\mathcal G$, so its intersection with a first-section member must avoid both shifted intervals; their union is $[a-1,b]$.

If the first replacement increases the density product by a factor at least $1+\delta$, use it. Otherwise interchange the names of the two [set families](../../../../../set-family.md) if needed so that

$$
x=\frac{\mu_{m-1}(\mathcal F_1)}{\mu_m(\mathcal F)}\leq\sqrt{1+\delta}.
$$

If the second replacement gives a factor at least $1+\delta$, use it. If neither does, use the third. To bound its loss, put

$$
z=\frac{\mu_{m-1}(\mathcal G_0\cup\mathcal G_1)}{\mu_m(\mathcal G)}.
$$

We have $z\geq1$, $(2-x)z<1+\delta$, and consequently $1-\delta<x\leq\sqrt{1+\delta}\leq1+\delta/2$. The third replacement's product factor is

$$
x(2-z)>h(x),\qquad h(x)=\frac{x(3-\delta-2x)}{2-x}.
$$

Since $h''(x)=-4(1+\delta)/(2-x)^3<0$, its minimum on $[1-\delta,1+\delta/2]$ is at an endpoint. There

$$
h(1-\delta)=1-\delta,
\qquad h(1+\delta/2)=1-\delta-\frac{\delta^2}{1-\delta/2}\geq1-\delta-2\delta^2.
$$

Thus each step either gains a factor $1+\delta$ without increasing interval width, or widens the interval by one and loses at most a factor $1-\delta-2\delta^2$. This is the [forbidden-intersection density increment](../../../../../forbidden-intersection-density-increment.md), with its loss proved rather than hidden in an asymptotic error.

Start with $\mathcal F=\mathcal G=\mathcal A$ and $a=b=\ell$. Stop when $a=0$ or $b=m$. Dimension drops at every step. The positive lower product factors ensure that a nonempty starting pair stays nonempty; it therefore cannot reach a forbidden interval containing all $0,\ldots,m$. Write $v$ for the number of widening steps, $u$ for the number of gain steps, and put

$$
g=\log(1.02),\quad h=-\log(0.9792),\quad D=g+h.
$$

The terminal density product $\rho_*$ satisfies $\rho_*\geq\rho_0e^{gu-hv}$. Always $v\leq\ell$, since a widening step lowers $a$ by one.

If the procedure stops at $a=0$, the terminal forbidden interval is $[0,v]$. Every cross-intersection is therefore greater than $v$, and the [cross-intersection bound from cube separation](../../../../../cross-intersection-bound-from-cube-separation.md) gives $\rho_*\leq e^{-v^2/m}$. At least $\ell$ steps were needed to lower $a$ to zero, so $u\geq\ell-v$. Since $m\leq n$,

$$
\log\rho_0\leq-g\ell+Dv-v^2/n
\leq\boxed{-g\ell+D^2n/4}.
$$

If instead the procedure stops at $b=m$, the number of steps is at least $n-\ell$, so $u\geq n-\ell-v$. Using $\rho_*\leq1$ and $v\leq\ell$ gives

$$
\log\rho_0\leq-g(n-\ell)+Dv
\leq\boxed{-gn+(2g+h)\ell}.
$$

These estimates hold for every nonempty pair forbidding the original intersection, with $\rho_0=(|\mathcal A|/2^n)^2$ in our application.

For $\ell=n/4$, the two positive exponential decay rates are, respectively,

$$
g/4-D^2/4>0.00453,
\qquad g-(2g+h)/4>0.00464.
$$

Both exceed $c=-2\log(1.999/2)<0.001001$. Hence $\rho_0\leq e^{-cn}$ and

$$
\boxed{|\mathcal A|\leq2^ne^{-cn/2}=1.999^n.}
$$

The empty [set family](../../../../../set-family.md) is immediate. This proves the numerical bound directly from [Harper inequality](../../../../../vertex-isoperimetric-inequality-in-the-discrete-cube.md) and the supplied [binary entropy function](../../../../../binary-entropy-function.md) estimate.

For $\ell=\lfloor n/8\rfloor$, the identical [forbidden-intersection density increment](../../../../../forbidden-intersection-density-increment.md) applies. For $n\geq17$, use $\ell\geq n/8-7/8$ in the first stopping estimate. Its decay rate is at least

$$
g/8-D^2/4-\frac{7g}{8n}
\geq g/8-D^2/4-7g/136>0.001039>c.
$$

For the second stopping estimate, $\ell\leq n/8$ gives the still stronger rate $g-(2g+h)/8>0.01222$. At $n=16$ the floor is exact and the first rate is $g/8-D^2/4>0.002058>c$.

It remains to handle $1\leq n\leq15$ without silently absorbing a constant into an exponential. Then $\ell$ is zero or one. Fix an $\ell$-set $T$. The $2^{n-\ell}$ sets containing $T$ are paired as $T\cup S$ and $T\cup([n]\setminus(T\cup S))$, and each pair intersects in exactly $T$. Since $n>\ell$, these are distinct pairs, and at most one member of each belongs to $\mathcal A$. Therefore

$$
|\mathcal A|\leq2^n-2^{n-\ell-1}\leq\tfrac34\,2^n<1.999^n.
$$

For $n=0$, the forbidden self-intersection is zero, so the [set family](../../../../../set-family.md) is empty. We have proved the claimed base for **all** dimensions in the second case as well.

Finally, **the same base is not forced by a forbidden intersection near $2n/3$.** Take $n=2000$ and every subset of size at most $1000$. Every intersection has size at most $1000$, below $\lfloor2n/3\rfloor=1333$, including self-intersections. By pairing complementary sets this [set family](../../../../../set-family.md) has more than $2^{1999}$ members, whereas

$$
1.999^{2000}=2^{2000}(0.9995)^{2000}<2^{1999},
$$

since $2000\log(0.9995)<-1<-\log2$. Thus it is a [large family avoiding a high intersection](../../../../../large-family-avoiding-a-high-intersection.md), and it contradicts the proposed bound.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
