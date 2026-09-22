# McShane extension theorem

↑ **Parent:** [Lipschitz continuity](lipschitz-continuity.md)

Let $A$ be a nonempty [subset](subset.md) of a [metric space](metric-space.md) $X$, and let $f:A\to\mathbb R$ satisfy a [Lipschitz bound](lipschitz-bound.md) $L$. Then

$$
F(x)=\inf_{a\in A}\{f(a)+Ld(x,a)\},\qquad
G(x)=\sup_{a\in A}\{f(a)-Ld(x,a)\}
$$

are real-valued [Lipschitz functions](lipschitz-continuity.md) on all of $X$, agree with $f$ on $A$, and obey the same bound $L$. Every other extension $H$ satisfying that bound lies between them, $G\leq H\leq F$. Despite the [infimum](infimum.md) in its formula, $F$ is the largest such extension: every given sample supplies an upper constraint $H(x)\leq f(a)+Ld(x,a)$.

Take three real samples $f(0)=0$, $f(1)=1/2$, $f(2)=0$, and allow the bound $L=1$. Their least [Lipschitz constant](lipschitz-constant.md) is only $1/2$, so this is deliberately a looser permitted bound. The two extensions are

$$
F(x)=\min\{|x|,\tfrac12+|x-1|,|x-2|\},\qquad
G(x)=\max\{-|x|,\tfrac12-|x-1|,-|x-2|\}.
$$

At $x=1/2$, the allowable [interval](interval-mathematics.md) is $0=G(1/2)\leq H(1/2)\leq F(1/2)=1/2$. The [interpolant](interpolant.md) obtained by [linear interpolation](linear-interpolation.md) is a [piecewise linear function](piecewise-linear-function.md) and has value $1/4$ there. Extending it constantly outside $[0,2]$ obeys the same bound on the entire [real line](real-line.md). At $x=5/2$, the allowable [interval](interval-mathematics.md) is $[-1/2,1/2]$. Thus the data and the bound control possible values without selecting a unique curve.

<a id="image-each-sample-constrains-a-lipschitz-function-the-upper-and-lower-envelopes-bound-every-allowed-extension"></a>
![](lipschitz-extension-envelopes.png)

**[Figure 13](#image-each-sample-constrains-a-lipschitz-function-the-upper-and-lower-envelopes-bound-every-allowed-extension). Each sample constrains a Lipschitz function; the upper and lower envelopes bound every allowed extension**.

The construction is useful when data are known only on a [subset](subset.md): it extends them without increasing an allowed [Lipschitz bound](lipschitz-bound.md). A short justification explains why the envelopes work. Fix $a_0\in A$. The [triangle inequality](triangle-inequality.md) and the bound on $f$ imply

$$
f(a_0)-Ld(x,a_0)\leq f(a)+Ld(x,a)
\qquad(a\in A),
$$

so the [infimum](infimum.md) is finite below; the term $a=a_0$ makes it finite above. At a sample $x=a_0$, all upper terms are at least $f(a_0)$, while that term gives equality. Finally, $d(x,a)\leq d(y,a)+d(x,y)$ gives $F(x)\leq F(y)+Ld(x,y)$ after taking an [infimum](infimum.md); exchanging $x,y$ proves the bound. The lower envelope follows by applying the same argument to $-f$.

E. J. McShane's paper _Extension of range of functions_ appeared in the _Bulletin of the American Mathematical Society_, volume 40, in 1934, pp. 837–842. [AMS bibliography: E. J. McShane, Extension of range of functions](https://www.ams.org/books/surv/012/surv012-endmatter.pdf) [McShane's original publication](https://doi.org/10.1090/S0002-9904-1934-05978-0)

## ↑ Ancestors (6)

1. [Lipschitz continuity](lipschitz-continuity.md)
2. [Real analysis](real-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Interpolant](interpolant.md)
- [Interpolation](interpolation-split.md)
- [Lipschitz continuity](lipschitz-continuity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-2/12f/a/solution.md)
