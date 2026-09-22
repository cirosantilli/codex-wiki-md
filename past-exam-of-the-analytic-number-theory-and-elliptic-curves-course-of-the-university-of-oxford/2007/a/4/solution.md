<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $x>0$, $(e^x-1)^{-1}=\sum_{n\ge1}e^{-nx}$. If $\sigma=\operatorname{Re}s>1$, the [integral](../../../../integral-split.md) of the sum of absolute values is $\Gamma(\sigma)\sum n^{-\sigma}<\infty$. Therefore interchange of sum and [integral](../../../../integral-split.md) is justified, and the substitution $u=nx$ gives

$$
J(s)=\sum_{n\ge1}\int_0^\infty x^{s-1}e^{-nx}dx
=\boxed{\Gamma(s)\zeta(s).}
$$

On the two unbounded rays of the specified [Hankel contour](../../../../hankel-contour.md), $x\ge\pi$ and $1/(e^x-1)$ decays exponentially, dominating every fixed power $x^{\sigma-1}$. The branch multiplier on the lower ray is a fixed factor $e^{2\pi i(s-1)}$. On the circular part, the chosen branch is continuous along the parametrized arc, and $e^z-1$ never vanishes because its nonzero zeros have modulus at least $2\pi$. Thus $I(s)$ exists for every $s$. The estimates are uniform when $s$ ranges over a [compact set](../../../../compact-space.md), including after differentiation in $s$, so $I$ is an [entire function](../../../../entire-function.md).

Let $C(s)=(e^{2\pi is}-1)\Gamma(s)$. The given identity shows that $I(s)/C(s)$ agrees with $\zeta(s)$ for $\operatorname{Re}s>1$ wherever the quotient is directly defined. It supplies the [meromorphic continuation](../../../../meromorphic-continuation.md) elsewhere wherever $C$ is finite and nonzero, with removable points filled by limits. At a nonpositive [integer](../../../../integer-split.md) $-k$, the simple zero of the exponential factor cancels the supplied gamma [pole](../../../../pole.md), giving

$$
C(-k)=\frac{2\pi i(-1)^k}{k!}.
$$

At $s=-k$, the [integrals](../../../../integral-split.md) on the two rays cancel because the integrand is single-valued. The remaining positively oriented circle has only the [pole](../../../../pole.md) at zero inside it, so

$$
I(-k)=2\pi i\operatorname{Res}_{z=0}\frac{z^{-k-1}}{e^z-1}
=2\pi i\,[z^{k+1}]\frac z{e^z-1}.
$$

The coefficient at $k=0$ is $-1/2$, hence $\boxed{\zeta(0)=-1/2}$. For positive even $k$, the relevant odd coefficient has degree at least three and is zero, giving $\boxed{\zeta(-2m)=0}$ for $m\ge1$. For $k=2m-1$, the given generating function gives the coefficient $(-1)^{m-1}B_m/(2m)!$. Division by $C(-(2m-1))=-2\pi i/(2m-1)!$ yields

$$
\boxed{\zeta(1-2m)=\frac{(-1)^mB_m}{2m}\qquad(m\ge1).}
$$

The symbols $B_m$ here follow the printed generating function: they are the positive magnitudes of the usual even-index [Bernoulli numbers](../../../../bernoulli-number-split.md), so $B_1=1/6$, $B_2=1/30$. This convention accounts for the alternating sign in the final expression.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
