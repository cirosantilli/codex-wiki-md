# Essential range

↑ **Parent:** [Measurable function](measurable-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Essential_range)

The essential range of a real or complex [measurable function](measurable-function.md) $m$ consists of the values $z$ whose every [neighborhood](neighbourhood-mathematics.md) receives inputs of positive [measure](measure.md):

$$
\operatorname{essran}_\mu m=\{z:\mu(\{x:|m(x)-z|<\varepsilon\})>0\text{ for every }\varepsilon>0\}.
$$

It depends on the [measure](measure.md) as well as the [function](function-split.md). This definition concerns values arbitrarily near $z$, not necessarily inputs at which $m=z$ exactly. It therefore retains meaningful limiting values while ignoring values occurring only on [null sets](null-set.md). [Teschl, Mathematical Methods in Quantum Mechanics, §2.4, equation (2.77): essential range](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe2.pdf).

For $m(x)=x$ on $(0,1)$ with [Lebesgue measure](lebesgue-measure.md), **the ordinary [image of a function](image-of-a-function.md) is $(0,1)$, but the [essential range](essential-range.md) is $[0,1]$**. Neither endpoint is attained, yet inputs with $|m(x)|<\varepsilon$ or $|m(x)-1|<\varepsilon$ have positive [measure](measure.md) for every $\varepsilon>0$. Every interior value also belongs to the [essential range](essential-range.md), although its exact [fiber](fiber-of-a-function.md) is a [singleton](singleton-mathematics.md) of zero [measure](measure.md). Positive [measure](measure.md) of a fiber is sufficient, but is not necessary, for a value to belong to the [essential range](essential-range.md).

The two-sided example $g$ from [essential infimum and essential supremum](essential-infimum-and-essential-supremum.md) illustrates what disappears. It follows $g(x)=x$ on $[0,1]$, except $g(1/4)=-3$ and $g(3/4)=4$. Its ordinary [image of a function](image-of-a-function.md) is $([0,1]\setminus\{1/4,3/4\})\cup\{-3,4\}$, whereas its [essential range](essential-range.md) remains $[0,1]$. The missing ordinary values $1/4$ and $3/4$ still have arbitrarily close neighbors with positive [measure](measure.md); the exceptional values $-3$ and $4$ can each be isolated by a sufficiently small [neighborhood](neighbourhood-mathematics.md) whose [preimage](preimage.md) is a [null set](null-set.md).

<a id="image-the-essential-range-of-the-modified-identity-function-remains-0-1-while-its-ordinary-image-of-a-function-includes-two-isolated-outliers"></a>
![](essential-upper-lower-bound-exceptions.png)

**[Figure 2](#image-the-essential-range-of-the-modified-identity-function-remains-0-1-while-its-ordinary-image-of-a-function-includes-two-isolated-outliers). The essential range of the modified identity function remains $[0,1]$, while its ordinary image of a function includes two isolated outliers**. For [Lebesgue measure](lebesgue-measure.md), the filled outliers $-3$ and $4$ fail the criterion of positive [measure](measure.md) in every [neighborhood](neighbourhood-mathematics.md). The hollow values $1/4$ and $3/4$ still belong to the [essential range](essential-range.md) because nearby outputs occur on [intervals](interval-mathematics.md) of positive [measure](measure.md).

For the three-point example in [L-infinity norm](l-infinity-norm.md), the values are $1,3,10$. With weights $(0.5,0.5,0)$ the [essential range](essential-range.md) is $\{1,3\}$; with weights $(0.499,0.5,0.001)$ it is $\{1,3,10\}$. A small but positive [probability](probability.md) retains ten, so an [essential range](essential-range.md) does not discard a value merely because it is rare. For a real [function](function-split.md) on a space of positive total [measure](measure.md), the [essential infimum](essential-infimum.md) and [essential supremum](essential-supremum.md) are the lower and upper edges of its [essential range](essential-range.md), allowing infinite bounds. The [L-infinity norm](l-infinity-norm.md) instead takes the upper edge of the [essential range](essential-range.md) of $|m|$.

<a id="image-including-ten-in-the-essential-range-changes-the-limiting-lp-norm-even-when-its-probability-is-only-0-001"></a>
![](lp-norm-null-versus-rare-value.png)

**[Figure 3](#image-including-ten-in-the-essential-range-changes-the-limiting-lp-norm-even-when-its-probability-is-only-0-001). Including ten in the essential range changes the limiting Lp norm, even when its probability is only $0.001$**. The blue case has [essential range](essential-range.md) $\{1,3\}$, while the red case has [essential range](essential-range.md) $\{1,3,10\}$. These finite positive-valued examples make their largest essential values equal to their [L-infinity norms](l-infinity-norm.md).

A useful operator connection is the [spectrum of a real multiplication operator](spectrum-of-a-real-multiplication-operator.md): on a nonzero [L2 space](l2-space-is-a-hilbert-space.md) over a [sigma-finite measure](sigma-finite-measure.md), multiplication by a real [measurable function](measurable-function.md) $m$ has [spectrum](spectrum-functional-analysis.md) equal to its [essential range](essential-range.md), with the natural domain when $m$ is unbounded. Outside that range, $|m-z|$ has a positive lower bound [almost everywhere](almost-everywhere.md), so multiplication by $1/(m-z)$ gives an [inverse function](inverse-function.md) that is a [bounded linear operator](continuous-linear-operator.md). Near an essential value, this lower bound fails. Thus discarding [null sets](null-set.md) is precisely what makes the range match an operator acting on [almost everywhere](almost-everywhere.md) [equivalence classes](equivalence-class.md). [Teschl, Mathematical Methods in Quantum Mechanics, §2.4, equations (2.74)–(2.77): multiplication-operator spectrum](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe2.pdf).

## ↑ Ancestors (7)

1. [Measurable function](measurable-function.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Essential range](essential-range.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-7/1/solution.md)
- [Spectrum of a bounded operator](spectrum-of-a-bounded-operator.md)
- [Spectrum of a real multiplication operator](spectrum-of-a-real-multiplication-operator.md)
