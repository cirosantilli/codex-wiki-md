<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $c=e^{-\gamma}$, where $\gamma$ is the [Euler--Mascheroni constant](../../../../../../euler-s-constant.md), and let $f(u)=w(u)-c$. The [Buchstab function](../../../../../../buchstab-function.md) equation becomes

$$
\frac{d}{du}(u f(u))=f(u-1)\qquad(u>2).
$$

The given [Gamma function](../../../../../../gamma-function.md) bound implies $u f(u)\to0$. Indeed,

$$
\Gamma(u+1)=\int_0^\infty e^{-x}x^u\,dx\ge\int_u^{u+1}e^{-x}x^u\,dx\ge e^{-u-1}u^u,
$$

so $u/\Gamma(u+1)\to0$.

Suppose first that $f\ge0$ throughout an interval $[u,u+1]$, with $u\ge1$. The [delay differential equation](../../../../../../delay-differential-equation.md) and integration successively on $[u+1,u+2]$, $[u+2,u+3]$, and so on propagate nonnegativity to the entire tail $[u,\infty)$. In particular, $v f(v)$ is nonnegative and nondecreasing for $v\ge u+1$. Its limit is zero, so it is identically zero there. Thus $f=0$ on that tail.

The [delay differential equation](../../../../../../delay-differential-equation.md) then propagates this equality backwards: if $f=0$ for $v\ge a$, then $f(v-1)=0$ for $v>\max(a,2)$. Repeating finitely many times would give $f=0$ on $(1,2)$, contradicting $f(v)=1/v-c$ there. Hence every interval $[u,u+1]$ contains a point where $f<0$.

If instead $f\le0$ on $[u,u+1]$, the same propagation makes $v f(v)$ nonpositive and nonincreasing on the tail. Its limit zero again forces it to vanish, giving the same contradiction. Thus every such interval also contains a point where $f>0$. **The oscillation of the Buchstab function is therefore strict on every unit interval**:

$$
\boxed{\exists u^+,u^-\in[u,u+1]:\quad w(u^+)>e^{-\gamma},\quad w(u^-)<e^{-\gamma}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
