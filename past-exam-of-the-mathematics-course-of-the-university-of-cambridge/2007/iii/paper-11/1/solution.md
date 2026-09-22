<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The complement of $D$ is nonempty and closed. Take points $w_j$ in that complement with $|z_0-w_j|\to\delta(z_0)$. This sequence is bounded, so a subsequence converges to a point $w_0\notin D$. Continuity of distance gives $|z_0-w_0|=\delta(z_0)>0$.

Put $t=(z_0-w_0)/(z-w_0)$. On the indicated exterior region $|t|<1$, and $f=1-t$ lies in the right half-plane. Its principal [holomorphic logarithm](../../../../../holomorphic-logarithm.md) is therefore the [power series](../../../../../power-series.md)

$$
\log f(z)=-\sum_{k=1}^{\infty}\frac{t^k}{k}.
$$

On each compact subset of that region, $|t|\leq q<1$, so the series has [locally uniform convergence](../../../../../locally-uniform-convergence.md) by comparison with $\sum q^k/k$. It does **not converge uniformly on the whole region**: choose $z=w_0+(z_0-w_0)/s$ with $0<s<1$. Then $t=s$; as $s\uparrow1$, $\log(1-s)$ tends to minus infinity while each fixed partial sum stays bounded. In particular, the remainder after any fixed number of terms is unbounded.

The [boundary-adapted holomorphic zero factor](../../../../../boundary-adapted-holomorphic-zero-factor.md) $E_0$ is holomorphic throughout $D$, since its only possible denominator singularity is at $w_0\notin D$. The exponential never vanishes, so its only zero is $z_0$, and

$$
E_0'(z_0)=\frac{1}{z_0-w_0}\exp\left(\sum_{k=1}^K\frac1k\right)\ne0.
$$

On $|z-w_0|>2\delta(z_0)$, cancellation of the first $K$ logarithmic terms gives a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) of this zero-free restriction with

$$
\boxed{\left|\log E_0(z)\right|\leq\sum_{k>K}\frac{2^{-k}}k\leq\frac{2^{-K}}{K+1}.}
$$

Choose $K$ so that the final bound is smaller than the prescribed error. This logarithm is only asserted on the exterior region; a function with a zero cannot have a logarithm on all of $D$.

For each $z_n$, construct a [boundary-adapted holomorphic zero factor](../../../../../boundary-adapted-holomorphic-zero-factor.md) $E_n$ whose logarithmic error is smaller than $2^{-n}$. If $L\subset D$ is compact, write $d_L=\operatorname{dist}(L,\mathbb C\setminus D)>0$. For all sufficiently large $n$, $2\delta(z_n)<d_L\leq|z-w_n|$ for every $z\in L$. Hence $\sum\log E_n$ converges absolutely and uniformly on $L$ after discarding finitely many terms. Consequently

$$
\boxed{F(z)=\prod_{n=1}^{\infty}E_n(z)}
$$

is a [holomorphic function](../../../../../holomorphic-function.md). Its tail is the exponential of a convergent logarithmic sum and is nonzero. The finite initial product has precisely its prescribed [simple zeros](../../../../../simple-zero.md). Since $\delta(z_n)\to0$, only finitely many $z_n$ lie in any compact subset of $D$, and this proves that $F$ has exactly the desired [simple zeros](../../../../../simple-zero.md).

For the final [meromorphic function](../../../../../meromorphic-function.md) assertion, poles escaping to infinity need additional care: a locally finite pole sequence need not satisfy $\delta(z_n)\to0$. Here is the required extension of the product argument. Split the distinct poles $a$ into two sets according as

$$
\delta(a)\leq\frac{1}{1+|a|}\quad\hbox{or}\quad\delta(a)>\frac{1}{1+|a|}.
$$

In the first set, for each $\varepsilon>0$ the poles with $\delta(a)\geq\varepsilon$ are in a bounded closed subset lying at least $\varepsilon$ from the complement. Local finiteness makes this a finite set. Thus the boundary distances tend to zero. In the second set, poles in $|a|\leq R$ are at least $1/(1+R)$ from the complement, so there are finitely many of them. Thus their moduli tend to infinity.

Use the preceding factors for the first set. For the second set use the [Weierstrass elementary factors](../../../../../weierstrass-elementary-factor.md)

$$
P_K(z/a)=(1-z/a)\exp\left(\sum_{k=1}^K\frac{(z/a)^k}{k}\right).
$$

For $|z|<|a|/2$ these have the same logarithmic-tail bound as above. If a pole has order $m$, choose the factor's error smaller than $2^{-n}/m$ and raise it to the power $m$. A possible pole at zero is handled by a finite polynomial factor. On every compact subset the resulting logarithmic tails are uniformly summable, so their product $q$ is holomorphic with zeros of exactly the pole orders and no other zeros. If $M$ is the original [meromorphic function](../../../../../meromorphic-function.md), the product $Mq$ extends holomorphically across every pole. Writing that extension as $p$ gives the concise conclusion

$$
\boxed{M=p/q,\qquad p,q\text{ holomorphic on }D,\quad q\not\equiv0.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
