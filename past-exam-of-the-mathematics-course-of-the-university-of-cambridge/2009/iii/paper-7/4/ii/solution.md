<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $S_n(t)=\sum_{r=-n}^na_re^{irt}$. First we prove [decay of coefficients of an almost-everywhere convergent trigonometric series](../../../../../../decay-of-coefficients-of-an-almost-everywhere-convergent-trigonometric-series.md) rather than assuming the series can be integrated term by term. For $n\ge1$, $T_n(t)=S_n(t)-S_{n-1}(t)=a_ne^{int}+a_{-n}e^{-int}$ tends to zero outside the finite set $E$. Suppose $M_n=|a_n|+|a_{-n}|$ does not tend to zero, and choose a subsequence with $M_n\ge\varepsilon>0$. Then $|T_n/M_n|\le1$ and $T_n/M_n\to0$ almost everywhere. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives

$$
\frac1{2\pi}\int_0^{2\pi}\left|\frac{T_n(t)}{M_n}\right|^2dt\to0.
$$

[orthogonality](../../../../../../orthogonal-vectors.md) of the two distinct [Fourier modes](../../../../../../fourier-mode.md) instead makes the integral $(|a_n|^2+|a_{-n}|^2)/M_n^2\ge1/2$, a contradiction. Thus $\boxed{a_n,a_{-n}\to0}$.

Define on the real line the twice-integrated [continuous function](../../../../../../continuous-function.md)

$$
F(t)=\frac{a_0t^2}{2}-\sum_{r\ne0}\frac{a_r}{r^2}e^{irt}.
$$

The series has both [absolute convergence](../../../../../../absolute-convergence.md) and [uniform convergence](../../../../../../uniform-convergence.md) because its coefficients are bounded. Its symmetric second quotient is therefore, for nonzero $h$,

$$
\frac{F(t+h)-2F(t)+F(t-h)}{h^2}=a_0+\sum_{r\ne0}a_re^{irt}w(rh/2).
$$

We next prove that this tends to zero whenever $t\notin E$, lifted periodically to the line. Let $b_0=a_0$ and $b_n=a_ne^{int}+a_{-n}e^{-int}$ for $n\ge1$, so the partial sums of the $b_n$ are exactly $S_n(t)\to0$. Put $k=|h|/2$ and $w_n=w(nk)$. [Summation by parts](../../../../../../abel-s-summation-formula.md) gives

$$
\sum_{n=0}^\infty b_nw_n=\sum_{n=0}^\infty S_n(t)(w_n-w_{n+1}).
$$

The boundary term vanishes because $S_n(t)$ is bounded and $w_n\to0$ for fixed nonzero $k$. Moreover

$$
\sum_{n\ge0}|w_n-w_{n+1}|\le\int_0^\infty|w'(x)|dx=C<\infty.
$$

Indeed $w'(x)=O(x)$ near zero and $|w'(x)|\le2/x^2+2/x^3$ for $x\ge1$. Each fixed weight difference tends to zero as $k\to0$. Splitting the last series at an index beyond which $|S_n(t)|<\eta$ therefore bounds its upper limit by $C\eta$. Letting $\eta\to0$ proves the claimed zero second quotient. This explicitly proves the needed [Riemann summation of a convergent trigonometric series](../../../../../../riemann-summation-of-a-convergent-trigonometric-series.md), despite the oscillations in its weights.

We also need the elementary fact that a [continuous function](../../../../../../continuous-function.md) with zero [symmetric second derivative](../../../../../../symmetric-second-derivative.md) at every interior point of an interval is affine. For a real-valued function, subtract its endpoint chord on any compact subinterval $[a,b]$. If the difference were positive somewhere, adding $\varepsilon(t-a)(t-b)$ for sufficiently small $\varepsilon>0$ would retain a positive maximum at an interior point. At that maximum each symmetric second difference is nonpositive, while its quotient tends to $2\varepsilon>0$, a contradiction. Thus the function lies below its chord. Apply the argument to its negative to get the reverse inequality. Applying this to real and imaginary parts proves the complex-valued case as well. This establishes that [vanishing symmetric second derivative forces an affine function](../../../../../../vanishing-symmetric-second-derivative-forces-an-affine-function.md). Hence $F$ is an [affine function](../../../../../../affine-function.md) on each open interval between the finitely many exceptional points in any period.

It remains to exclude corners at those points. Multiplying the formula for the second quotient by $h$, and using $h=2k$ and the evenness of $w$, gives

$$
\frac{F(t+h)-2F(t)+F(t-h)}h=a_0h+h\sum_{n\ge1}(a_ne^{int}+a_{-n}e^{-int})w(nh/2)\longrightarrow0
$$

for every $t$, by the infinite-series version of part (i), since $a_n,a_{-n}\to0$. [continuity](../../../../../../continuous-function.md) extends the adjacent affine pieces to each exceptional point, and the fact that [symmetric second differences detect an affine corner](../../../../../../symmetric-second-differences-detect-an-affine-corner.md) makes their slopes and intercepts agree. Thus $F$ is globally an [affine function](../../../../../../affine-function.md) on the real line.

The periodic part of its definition gives $F(t+2\pi)-F(t)=2\pi a_0t+2\pi^2a_0$. An [affine function](../../../../../../affine-function.md) has constant increments, so $a_0=0$. The resulting $F$ is both an [affine function](../../../../../../affine-function.md) and a [periodic function](../../../../../../periodic-function.md), hence constant. Finally, absolute [uniform convergence](../../../../../../uniform-convergence.md) justifies integrating its defining series against $e^{-irt}$, and for $r\ne0$ the resulting [Fourier coefficient](../../../../../../fourier-coefficient.md) is $-a_r/r^2$. A constant has all these coefficients zero. Therefore $\boxed{a_r=0\text{ for every }r\in\mathbb Z}$, proving [uniqueness of a trigonometric series outside a finite set](../../../../../../uniqueness-of-a-trigonometric-series-outside-a-finite-set.md) with all exceptional points accounted for.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
