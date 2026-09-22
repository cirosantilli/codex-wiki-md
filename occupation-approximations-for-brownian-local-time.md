# Occupation approximations for Brownian local time

↑ **Parent:** [Brownian local time](brownian-local-time.md)

For [Brownian motion](brownian-motion-split.md) started at zero, let $f_n$ equal $|x|$ outside $(-1/n,1/n)$ and $nx^2/2+1/(2n)$ inside. Its derivative is the clipped sign function $g_n(x)=\max\{-1,\min\{1,nx\}\}$. The [Itô integral](ito-integral.md) $M_t^{(n)}=\int_0^t g_n(B_s)dB_s$ converges uniformly on bounded time intervals in $L^2$ to a [continuous martingale](continuous-martingale.md) $M$, by the [Itô isometry](ito-isometry.md) and [Doob L2 maximal inequality](doob-l2-maximal-inequality.md): the squared maximal error is at most $8\sqrt{2T/\pi}/n$. The [Itô formula](ito-s-lemma.md) gives $\frac n2\int_0^t\mathbf1_{\{|B_s|<1/n\}}ds=f_n(B_t)-f_n(0)-M_t^{(n)}$. Along $n=k^2$, the maximal errors are summable, so [First Borel-Cantelli lemma](borel-cantelli-first-lemma.md) gives uniform almost-sure convergence. The [ratio-one interpolation for shrinking-window occupation integrals](ratio-one-interpolation-for-shrinking-window-occupation-integrals.md) extends it to every integer $n$. The limit is $|B_t|-M_t=L_t^0$, the [local time of a semimartingale](local-time-of-a-semimartingale.md) in the [Tanaka formula](tanaka-s-formula.md) convention. The unnormalized factor $n$ gives twice this limit.

**Table of contents**

- [Ratio-one interpolation for shrinking-window occupation integrals](ratio-one-interpolation-for-shrinking-window-occupation-integrals.md)

## ↑ Ancestors (10)

1. [Brownian local time](brownian-local-time.md)
2. [Local time of a semimartingale](local-time-of-a-semimartingale.md)
3. [Local time (mathematics)](local-time-mathematics.md)
4. [Stochastic calculus](stochastic-calculus-split.md)
5. [Stochastic process](stochastic-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Brownian local time](brownian-local-time.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31/4/solution.md)
