<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [Nevanlinna proximity function](../../../../../nevanlinna-proximity-function.md) $m(r,f)=(2\pi)^{-1}\int\log^+|f(re^{i\theta})|\,d\theta$ and the [Nevanlinna integrated counting function](../../../../../nevanlinna-integrated-counting-function.md) $N(r,f)$ for [poles](../../../../../pole.md), counting [multiplicity](../../../../../multiplicity-mathematics.md). If the pole order at zero is $\nu_0$, then

$$
N(r,f)=\nu_0\log r+\sum_{0<|b|<r}\nu_b\log\frac r{|b|},\qquad T(r,f)=m(r,f)+N(r,f).
$$

Boundedness of the [Nevanlinna characteristic](../../../../../nevanlinna-characteristic.md) refers to $r\uparrow1$, equivalently to a uniform bound on $r_0\le r<1$ for any fixed $r_0>0$. This avoids the harmless origin normalization when $\nu_0>0$.

The [Nevanlinna first main theorem](../../../../../nevanlinna-first-main-theorem.md) states, for every fixed finite value $a$ and every nonconstant [meromorphic function](../../../../../meromorphic-function.md) on the disk,

$$
\boxed{N(r,1/(f-a))+m(r,1/(f-a))=T(r,f)+O(1).}
$$

For $a=\infty$, this is the definition of $T$. The error is bounded independently of $r$. Translation changes $T$ by $O(1)$, while [Jensen's formula](../../../../../jensen-s-formula.md) gives $T(r,h)-T(r,1/h)=\log|c|$ when $h(z)=cz^\nu(1+O(z))$ near zero; these observations explain the first theorem.

The [Nevanlinna second main theorem in the unit disc](../../../../../nevanlinna-second-main-theorem-in-the-unit-disc.md) states that for $q\ge3$ distinct values $a_j$ on the [Riemann sphere](../../../../../riemann-sphere.md),

$$
\boxed{(q-2)T(r,f)\le\sum_{j=1}^q\overline N(r;a_j)+O\left(\log^+T(r,f)+\log\frac1{1-r}\right)}
$$

as $r\uparrow1$ outside an exceptional set $E$ satisfying $\int_Edr/(1-r)<\infty$. The [truncated Nevanlinna counting function](../../../../../truncated-nevanlinna-counting-function.md) $\overline N$ counts each distinct preimage once. The boundary-distance error cannot simply be suppressed: on the disk it need not be $o(T)$. The disk error and exceptional-set estimates follow from the logarithmic-derivative estimates in [https://mathweb.tifr.res.in/Documents/Publications/Lectures/tifr17.pdf](https://mathweb.tifr.res.in/Documents/Publications/Lectures/tifr17.pdf) .

Suppose first that $T(r,f)$ is bounded. Since $m(r,f)\ge0$, its [poles](../../../../../pole.md) satisfy the [Blaschke condition](../../../../../blaschke-condition.md), counting their orders: let $r\uparrow1$ in their integrated count and use $1-|b|\le-\log|b|$. Let $B$ be their [Blaschke product](../../../../../blaschke-product.md), including the origin factor if necessary. Then $g=Bf$ extends to a [holomorphic function](../../../../../holomorphic-function.md) on the whole disk, and $|B|\le1$ gives

$$
\frac1{2\pi}\int_0^{2\pi}\log^+|g(re^{i\theta})|\,d\theta\le m(r,f)\le C.
$$

Here the last bound follows from bounded $T$ and the uniform lower bound $N(r,f)\ge\nu_0\log r_0$ on $r\ge r_0$.

The nonnegative [subharmonic function](../../../../../subharmonic-function.md) $\log^+|g|$ has a finite [harmonic majorant](../../../../../harmonic-majorant.md). Indeed its [Poisson integrals](../../../../../poisson-integral.md) $H_R$ on expanding disks dominate it by the [maximum principle for subharmonic functions](../../../../../maximum-principle-for-subharmonic-functions.md), increase with $R$, and have $H_R(0)\le C$. The [Harnack inequality for harmonic functions](../../../../../harnack-inequality-for-harmonic-functions.md) bounds them on every compact subdisk, so their increasing limit is a finite [harmonic function](../../../../../harmonic-function.md) $H\ge\log^+|g|$. Since the disk is simply connected, $H$ has a [harmonic conjugate](../../../../../harmonic-conjugate.md), giving a [holomorphic function](../../../../../holomorphic-function.md) $A$ with $\operatorname{Re}A=H$. Consequently

$$
u=ge^{-A},\qquad v=Be^{-A},\qquad |u|\le1,\quad |v|\le1,\quad v\not\equiv0,\quad f=u/v.
$$

This proves the constructive half of the [quotient characterization of bounded characteristic](../../../../../quotient-characterization-of-bounded-characteristic.md).

Conversely, if $f=u/v$ with $u,v$ bounded [holomorphic functions](../../../../../holomorphic-function.md) and $v\not\equiv0$, each [pole](../../../../../pole.md) of $f$ is a zero of $v$ of at least the same order. The elementary inequality $\log^+|u/v|\le\log^+|u|+\log^+|1/v|$ and the [Nevanlinna first main theorem](../../../../../nevanlinna-first-main-theorem.md) give

$$
T(r,f)\le m(r,u)+T(r,1/v)+O(1)\le\log^+\|u\|_\infty+T(r,v)+O(1)=O(1).
$$

Any cancellation at an origin zero contributes only a bounded multiple of $\log r$ on $r\ge r_0$, which is included in this $O(1)$. The zero function is immediate; constant nonzero $v$ is handled directly. Thus **bounded characteristic is exactly a quotient of two bounded analytic functions**.

An unbounded example with [bounded characteristic](../../../../../bounded-characteristic.md) is

$$
\boxed{g(z)=\frac1{1-z}.}
$$

It is a ratio of the bounded [holomorphic functions](../../../../../holomorphic-function.md) $1$ and $1-z$. More explicitly, [Jensen's formula](../../../../../jensen-s-formula.md) gives the mean of $\log|1-re^{i\theta}|$ as zero, so $m(r,1/(1-z))=m(r,1-z)\le\log2$, although $g(r)\to\infty$.

Finally, set $Y=(1+|g|^2)^{p/2}\ge1$. Pointwise $\log^+|g|\le p^{-1}\log Y$. [Jensen's inequality](../../../../../jensen-s-inequality.md) for the concave [logarithm](../../../../../logarithm.md) gives

$$
T(r,g)=m(r,g)\le\frac1p\int\log Y\,\frac{d\theta}{2\pi}\le\frac1p\log\int Y\,\frac{d\theta}{2\pi}<\frac{\log C}{p}.
$$

There is no pole term because $g$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md). Hence **the stated integral bound implies bounded characteristic**. This argument in fact works for every $p>0$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
