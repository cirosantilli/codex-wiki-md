<h1 id="fieller-s-theorem">Fieller's theorem</h1>

↑ **Parent:** [Confidence interval](confidence-interval.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fieller's_theorem)

For jointly approximately [normal](normal-distribution.md) estimates $(\widehat C,\widehat E)$ with estimated [variances](variance-split.md) $v_C,v_E$ and [covariance](covariance.md) $v_{CE}$, a [confidence interval](confidence-interval.md) for the ratio $C/E$, where $E\ne0$, can be obtained by inverting tests of $C-rE=0$. For each proposed ratio $r$, the contrast has estimate $\widehat C-r\widehat E$ and [variance](variance-split.md) $v_C-2rv_{CE}+r^2v_E$. Retain $r$ when its absolute standardized contrast is at most the chosen critical value $q$. This gives the displayed quadratic inequality, with coefficients $A=\widehat E^2-q^2v_E$, $B=-2(\widehat C\widehat E-q^2v_{CE})$, $D=\widehat C^2-q^2v_C$. When $A>0$ and the discriminant is positive, retain the interval between the roots. When $A<0$, a confidence set can instead be two unbounded rays or the entire real line. Degenerate linear cases are interpreted directly from the inequality. A bounded interval must not be forced when the denominator is poorly separated from zero. Known [covariance matrix](covariance-matrix.md) and a joint [normal distribution](normal-distribution.md) give exact normal critical values; estimated covariance usually gives approximate coverage, unless an appropriate exact common-scale pivot exists.

## ↑ Ancestors (6)

1. [Confidence interval](confidence-interval.md)
2. [Statistical inference](statistical-inference-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-41/5/ii/solution.md)
