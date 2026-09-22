<h1 id="13g/solution">Solution</h1>

↑ **Parent:** [13G](../13g.md)

[Rouché's theorem](../../../../../rouche-s-theorem.md) states that if $g$ and $h$ are [holomorphic functions](../../../../../holomorphic-function.md) on a neighbourhood of the closure of a bounded domain and

$$
|h(z)|<|g(z)|
$$

on its positively oriented boundary, then $g$ and $g+h$ have the same number of zeros in the domain, counted with multiplicity.

The [Open mapping theorem](../../../../../open-mapping-theorem-complex-analysis.md) states that a nonconstant [holomorphic function](../../../../../holomorphic-function.md) on a domain maps every open subset to an open subset. To prove it, fix $z_0$ and put $w_0=f(z_0)$. By the [identity theorem](../../../../../identity-theorem.md), the zeros of $f-w_0$ are isolated. Choose $r>0$ so that the closed disc $\overline{D(z_0,r)}$ lies in the domain and $z_0$ is the only zero of $f-w_0$ in that disc. Then

$$
\delta=\min_{|z-z_0|=r}|f(z)-w_0|>0.
$$

Whenever $|w-w_0|<\delta$, the constant $w_0-w$ has [modulus](../../../../../modulus.md) smaller than $f-w_0$ on the circle. The Rouche theorem therefore says that

$$
f(z)-w=(f(z)-w_0)+(w_0-w)
$$

has the same positive number of zeros in the disc as $f-w_0$. Thus every $w\in D(w_0,\delta)$ lies in the image of $f$, proving that the image is open.

If $|f|$ had a local maximum at $z_0$, take a small [open disc](../../../../../open-disc.md) $D$ on which $|f(z)|\leq|f(z_0)|$. The restriction of $f$ to $D$ cannot be constant, since the identity theorem would then make $f$ constant on the whole domain. The complex open mapping theorem says that $f(D)$ is an open neighbourhood of $f(z_0)$, and such a neighbourhood contains points of [modulus](../../../../../modulus.md) greater than $|f(z_0)|$, a contradiction. This proves the [maximum modulus principle from the complex open mapping theorem](../../../../../maximum-modulus-principle-from-the-complex-open-mapping-theorem.md).

Now let $\Omega$ be bounded. Its closure is compact, so the [continuous](../../../../../continuous-function.md) [function](../../../../../function-split.md) $|f|$ attains a maximum there. If $f$ is nonconstant, the [maximum modulus principle](../../../../../maximum-modulus-principle.md) excludes an interior maximum; if $f$ is constant, the claimed bound is immediate. Hence

$$
\max_{z\in\overline\Omega}|f(z)|
=\max_{z\in\partial\Omega}|f(z)|\leq M,
$$

which is the [maximum modulus principle on a bounded domain](../../../../../maximum-modulus-principle-on-a-bounded-domain.md).

Finally let $\Omega=\{z:\operatorname{Re}z>1\}$ and suppose $|f|\leq K$ throughout $\overline\Omega$. Fix $z_0\in\Omega$. The principal [complex logarithm](../../../../../complex-logarithm.md) is holomorphic on the right half-plane, so for each positive integer $n$ the [function](../../../../../function-split.md)

$$
g_n(z)=f(z)z^{-1/n}
=f(z)\exp\left(-\frac1n\operatorname{Log}z\right)
$$

is holomorphic on $\Omega$ and continuous on its closure. Given $\varepsilon>0$, choose $R>|z_0|$ so large that

$$
K R^{-1/n}\leq M+\varepsilon.
$$

Apply the bounded-domain result to $g_n$ on $\Omega\cap D(0,R)$. On the vertical part of the boundary, $|z|\geq1$ and hence $|g_n(z)|\leq M$. On the circular part,

$$
|g_n(z)|\leq K R^{-1/n}\leq M+\varepsilon.
$$

It follows that

$$
|f(z_0)|\leq(M+\varepsilon)|z_0|^{1/n}.
$$

Letting $n\to\infty$ and then $\varepsilon\to0$ gives $|f(z_0)|\leq M$. Since $z_0$ was arbitrary, this proves the [bounded half-plane maximum principle](../../../../../bounded-half-plane-maximum-principle.md).

The boundedness assumption is necessary. The [function](../../../../../function-split.md)

$$
f(z)=e^z
$$

is holomorphic on $\Omega$ and continuous on its closure, and $|f(1+iy)|=e$ on the boundary, but $|f(x)|=e^x$ is unbounded for real $x>1$. Thus the boundary estimate does not control an unbounded [holomorphic function](../../../../../holomorphic-function.md) on this unbounded domain.

## ↑ Ancestors (10)

1. [13G](../13g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
