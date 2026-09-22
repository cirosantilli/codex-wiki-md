# Holomorphic logarithm

↑ **Parent:** [Complex analysis](complex-analysis-split.md)

A holomorphic logarithm of a nowhere-zero [holomorphic function](holomorphic-function.md) $f$ on a domain $U$ is a [holomorphic function](holomorphic-function.md) $g$ such that $e^{g(z)}=f(z)$ throughout $U$. Differentiating with the [chain rule](chain-rule.md) gives $g'=f'/f$. For $f(z)=z$, a [holomorphic logarithm](holomorphic-logarithm.md) is a [branch of the complex logarithm](branch-of-the-complex-logarithm.md), and its [derivative](derivative.md) is $1/z$.

The [principal logarithm](principal-complex-logarithm.md) is [holomorphic](holomorphic-function.md) on the slit [complex plane](complex-plane.md) $D=\mathbb C\setminus(-\infty,0]$, with

$$
\operatorname{Log}z=\log|z|+i\operatorname{Arg}z,\qquad -\pi<\operatorname{Arg}z<\pi,\qquad (\operatorname{Log}z)'=\frac1z.
$$

Here $\operatorname{Arg}$ is the chosen [complex argument](argument-complex-analysis.md), and $\operatorname{Im}\operatorname{Log}z\in(-\pi,\pi)$. One may conventionally assign a principal value on the negative real axis, but that axis is excluded from this [holomorphic](holomorphic-function.md) domain. [Romik, Complex Analysis Lecture Notes, section 13, items 109–110](https://www.math.ucdavis.edu/~romik/data/uploads/teaching/math205a-2018/complex-analysis-2018.pdf) For example, $1+i=\sqrt2e^{i\pi/4}$ gives $\operatorname{Log}(1+i)=\tfrac12\log2+i\pi/4$ and $(\operatorname{Log})'(1+i)=(1-i)/2$; all its other [complex logarithms](complex-logarithm.md) differ by $2\pi ik$, $k\in\mathbb Z$.

There is no [holomorphic logarithm](holomorphic-logarithm.md) of $z$ on the punctured [complex plane](complex-plane.md) $\mathbb C\setminus\{0\}$. Such a function would be a [holomorphic primitive](holomorphic-primitive.md) of $1/z$, so its [contour integral](contour-integral.md) around every closed path would vanish. On the counterclockwise [unit circle](complex-unit-circle.md), however,

$$
\oint_{|z|=1}\frac{dz}{z}=\int_0^{2\pi}\frac{ie^{it}}{e^{it}}\,dt=2\pi i\ne0.
$$

This is the [period obstruction to a holomorphic antiderivative](period-obstruction-to-a-holomorphic-antiderivative.md), and also exactly the logarithm change in the [monodromy](monodromy.md) diagram.

Every nowhere-zero [holomorphic function](holomorphic-function.md) $f$ on a [simply connected domain](simply-connected-domain.md) $U$ does admit a [holomorphic logarithm](holomorphic-logarithm.md). Choose $a\in U$ and $b\in\mathbb C$ with $e^b=f(a)$, and define

$$
g(z)=b+\int_a^z\frac{f'(\zeta)}{f(\zeta)}\,d\zeta.
$$

The [Cauchy integral theorem](cauchy-s-integral-theorem.md) makes this [contour integral](contour-integral.md) independent of the path in $U$. Then $g'=f'/f$ and $(fe^{-g})'=e^{-g}(f'-fg')=0$; its value at $a$ is $1$, proving $e^g=f$. Any two choices on a [connected](connected-space.md) domain differ by a constant $2\pi ik$, since their difference is [continuous](continuous-function.md) and takes values in the discrete set $2\pi i\mathbb Z$. [Romik, section 12, Corollary 108, and section 13, Exercise 114](https://www.math.ucdavis.edu/~romik/data/uploads/teaching/math205a-2018/complex-analysis-2018.pdf)

For a computed example, take $f(z)=1+z$ on the [unit disc](unit-disc.md), with $a=b=0$. Expanding $f'/f=1/(1+z)$ as a [geometric series](geometric-series.md) and integrating gives

$$
g(z)=\sum_{n=1}^{\infty}\frac{(-1)^{n-1}z^n}{n},\qquad g(1/2)=\log(3/2),\qquad e^{g(1/2)}=3/2.
$$

The construction also produces [holomorphic square roots](holomorphic-square-root.md): $h=e^{g/2}$ satisfies $h^2=f$, so here $h(1/2)=\sqrt{3/2}$. More generally, $e^{\alpha g}$ gives a consistent [branch of a multivalued function](branch-of-a-multivalued-function.md) for [complex exponentiation](complex-exponentiation.md) by $\alpha$. A [holomorphic logarithm](holomorphic-logarithm.md) converts multiplicative expressions into additive ones while making the domain restrictions explicit.

## ↑ Ancestors (5)

1. [Complex analysis](complex-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (40)

- [Boundary-adapted holomorphic zero factor](boundary-adapted-holomorphic-zero-factor.md)
- [Branch of a multivalued function](branch-of-a-multivalued-function.md)
- [Entire functions with the same zero divisor](entire-functions-with-the-same-zero-divisor.md)
- [Extremal derivative of a disc map into a symmetric annulus](extremal-derivative-of-a-disc-map-into-a-symmetric-annulus.md)
- [Holomorphic logarithm](holomorphic-logarithm.md)
- [Holomorphic square root](holomorphic-square-root.md)
- [Logarithm from a spectral slit in a Banach algebra](logarithm-from-a-spectral-slit-in-a-banach-algebra.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-7/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-9/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-9/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/4e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/4a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-2/23f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-10/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-11/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-11/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-12/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-32/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/14e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-11/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-26/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/5/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-8/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-17/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-8/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3/13g/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/13f/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-203/3/c/solution.md)
- [Prescribed zeros in a plane domain via Runge approximation](prescribed-zeros-in-a-plane-domain-via-runge-approximation.md)
- [Prime-character sum near one](prime-character-sum-near-one.md)
- [Schwarz integral on the unit disk](schwarz-integral-on-the-unit-disk.md)
- [Zero-free Schwarz lemma](zero-free-schwarz-lemma.md)
