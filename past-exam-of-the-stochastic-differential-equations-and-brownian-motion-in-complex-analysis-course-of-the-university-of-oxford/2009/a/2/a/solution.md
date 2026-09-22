<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [continuous semimartingale](../../../../../continuous-semimartingale.md) $X$ and a $C^{1,2}$ function $f$, [Itô's formula](../../../../../ito-s-lemma.md) is

$$
df(t,X_t)=f_t(t,X_t)\,dt+f_x(t,X_t)\,dX_t
+\tfrac12f_{xx}(t,X_t)\,d[X]_t.
$$

For [Brownian motion](../../../../../brownian-motion-split.md) $B$, $d[B]_t=dt$. With $f(t,x)=e^{-t/2}\cosh x$, the drift cancels:

$$
f_t+\tfrac12f_{xx}=-\tfrac12e^{-t/2}\cosh x+\tfrac12e^{-t/2}\cosh x=0.
$$

Consequently

$$
\boxed{d(e^{-t/2}\cosh B_t)=e^{-t/2}\sinh B_t\,dB_t.}
$$

The stochastic-integral representation makes this a [local martingale](../../../../../local-martingale.md); localization handles unbounded $B$. In fact it is the average of the two positive [exponential Brownian martingales](../../../../../exponential-brownian-martingale.md) $e^{B_t-t/2}$ and $e^{-B_t-t/2}$, so it is a true martingale on every finite time interval.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
