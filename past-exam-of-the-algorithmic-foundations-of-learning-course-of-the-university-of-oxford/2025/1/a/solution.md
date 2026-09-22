<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\psi(s)=\log\mathbb E e^{sX}$ for the [cumulant-generating function](../../../../cumulant-generating-function.md), and let $D_+=\{s>0:\psi(s)<\infty\}$. This set is nonempty. In fact, finiteness of the [moment-generating function](../../../../moment-generating-function.md) at some $\eta>0$ and $-\eta$ gives

$$
\mathbb E e^{\eta|X|}\leq\mathbb E e^{\eta X}+\mathbb E e^{-\eta X}<\infty,
$$

so $X$ is an [integrable random variable](../../../../integrable-random-variable.md). Put $m=\mathbb EX$.

For the upper tail, use the following one-sided [convex conjugate](../../../../convex-conjugate.md) and its [strict generalized inverse of a nondecreasing function](../../../../strict-generalized-inverse-of-a-nondecreasing-function.md):

$$
I(x)=\sup_{s\in D_+\cup\{0\}}\{sx-\psi(s)\},\qquad
\psi_X^{*-1}(t):=\inf\{x\in\mathbb R:I(x)>t\},\quad t>0.
$$

Here $\psi(0)=0$, and $I$ is nondecreasing because every slope in its defining [supremum](../../../../supremum.md) is nonnegative. For $x\geq m$, negative $s$ cannot increase the conjugate: $\psi(s)\geq sm$ gives $sx-\psi(s)\leq s(x-m)\leq0$, and $s=0$ already gives zero. Thus $I$ agrees with the full [Legendre transform of a cumulant-generating function](../../../../legendre-transform-of-a-cumulant-generating-function.md) on its upper-tail branch. Using a [strict generalized inverse of a nondecreasing function](../../../../strict-generalized-inverse-of-a-nondecreasing-function.md) handles constant [random variables](../../../../random-variable-split.md) and bounded supports without assuming a strictly increasing, everywhere finite conjugate. Directly from the definition,

$$
\{x:I(x)>t\}
=\bigcup_{s\in D_+}\left(\frac{t+\psi(s)}s,\infty\right),
\qquad
\boxed{\psi_X^{*-1}(t)=\inf_{s\in D_+}\frac{t+\psi(s)}s.}
$$

This threshold is finite: any fixed $s\in D_+$ gives a finite upper bound, while $e^u\geq1+u$ gives $\mathbb E e^{s(X-m)}\geq1$ and hence $\psi(s)\geq sm$, providing the lower bound $m$.

We now derive the needed [Chernoff bound](../../../../chernoff-bound.md). For $s\in D_+$ and any real $x$, the pointwise inequality $e^{sX}\geq e^{sx}\mathbf1_{\{X>x\}}$ implies

$$
\mathbb P(X>x)\leq e^{\psi(s)-sx}.
$$

Let $q=\psi_X^{*-1}(t)$. For every $\varepsilon>0$, the [infimum](../../../../infimum.md) formula supplies an $s\in D_+$ such that $(t+\psi(s))/s<q+\varepsilon$. Thus $\mathbb P(X>q+\varepsilon)\leq e^{-t}$. As $\varepsilon\downarrow0$, these events increase to $\{X>q\}$; [continuity from below of a measure](../../../../continuity-from-below-of-a-measure.md) proves

$$
\boxed{\mathbb P\{X>\psi_X^{*-1}(t)\}\leq e^{-t}.}
$$

The strict event and the [strict generalized inverse of a nondecreasing function](../../../../strict-generalized-inverse-of-a-nondecreasing-function.md) avoid any assumption that the optimizing $s$ exists. For example, if $X=m$ almost surely, the threshold is $m$ for every $t>0$, and the probability is zero.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../split.md)
5. [Algorithmic foundations of learning course of the University of Oxford](../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
