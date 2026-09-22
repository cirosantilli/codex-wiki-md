<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $t>0$, use the continuous logarithm of the [characteristic function](../../../../../../characteristic-function.md), normalized to zero at $u=0$, to write

$$
\frac1t\log\phi_{X_t}(u)
=a(\cos(bu)-1)+c(e^{iu}-1)+icu.
$$

Thus the deterministic drift is **$+c$**. In particular the last contribution is not the negative drift of a compensated unit-jump process.

Take a [Poisson random measure](../../../../../../poisson-random-measure.md) $N$ on $(0,\infty)\times\{+,-,p\}$ with intensity

$$
ds\left(\frac a2\delta_++\frac a2\delta_-+c\delta_p\right).
$$

Define the jump marks $j(+)=b$, $j(-)=-b$, and $j(p)=1$. A realization with the required process law is the [Poisson stochastic integral with finite intensity](../../../../../../poisson-stochastic-integral-with-finite-intensity.md)

$$
\boxed{X_t=ct+\int_{(0,t]\times\{+,-,p\}}j(z)\,N(ds,dz)
=ct+bN_t^+-bN_t^-+N_t^p,}
$$

where the three counts are independent [Poisson processes](../../../../../../poisson-process.md) of rates $a/2,a/2,c$. Their [characteristic functions](../../../../../../characteristic-function.md) multiply to

$$
\exp\left\{t\left[icu+\frac a2(e^{ibu}-1)+\frac a2(e^{-ibu}-1)+c(e^{iu}-1)\right]\right\},
$$

which is exactly the given expression. The constructed process is a [Lévy process](../../../../../../levy-process.md), and stationary independent increments make its entire finite-dimensional law determined by these one-time characteristic functions. This gives a representation in law of the specified process.

Equivalently, using its nonzero-jump measure, the [Lévy measure](../../../../../../levy-measure.md) is

$$
\nu=\frac a2\mathbf1_{\{b>0\}}(\delta_b+\delta_{-b})+c\delta_1,
$$

and the unmarked representation is $X_t=ct+\int_{(0,t]\times(\mathbb R\setminus\{0\})}z\,N(ds,dz)$ with intensity $ds\,\nu(dz)$. The finite-jump case of the [Lévy–Itô decomposition](../../../../../../levy-ito-decomposition.md) realizes this pathwise using the jump measure of a version of $X$; the integral is an uncompensated finite sum.

The [atomic compound Poisson process with drift](../../../../../../atomic-compound-poisson-process-with-drift.md) has [càdlàg](../../../../../../cadlag.md) paths with finitely many nonzero jumps on every bounded time interval, linear slope $c$ between jumps, and no Brownian component. When $b>0$, jumps of sizes $b,-b,1$ occur at the stated rates; when $b=1$, positive unit-jump rates combine to $a/2+c$. When $b=0$, the two symmetric marks have zero effect and are omitted from the [Lévy measure](../../../../../../levy-measure.md); the process reduces to $ct+N_t^p$, so $a$ has no effect. If $c=0$ the paths are piecewise constant, and if also $ab=0$ they are identically zero. All paths have finite variation on bounded intervals. As a check on the drift sign,

$$
\mathbb EX_t=2ct,\qquad\operatorname{Var}(X_t)=t(ab^2+c).
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
