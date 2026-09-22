# Van der Corput inequality for finite scalar sequences

↑ **Parent:** [Van der Corput lemma (Hilbert space sequences)](van-der-corput-lemma-hilbert-space-sequences.md)

For complex numbers $|u_n|\leq1$, $0\leq n<N$, and $1\leq H\leq N$, put $C_h=\sum_{n=0}^{N-h-1}u_{n+h}\overline{u_n}$. Then

$$
\left|\frac1N\sum_{n=0}^{N-1}u_n\right|^2
\leq\frac{N+H-1}{NH}\left(1+2\sum_{h=1}^{H-1}\left(1-\frac hH\right)\frac{|C_h|}{N}\right).
$$

Extend the sequence by zero, count each summand in $H$ consecutive windows, and apply the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) to their sum. Expansion of the squared window sums gives the stated coefficients. Fixing $H$ and making each normalized correlation tend to zero bounds the limiting squared average by $1/H$; then let $H$ tend to infinity. This is the scalar finite form underlying the [Van der Corput lemma](van-der-corput-lemma-hilbert-space-sequences.md).

## ↑ Ancestors (8)

1. [Van der Corput lemma (Hilbert space sequences)](van-der-corput-lemma-hilbert-space-sequences.md)
2. [Ergodic theory](ergodic-theory.md)
3. [Measure theory](measure-theory-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Differencing obstruction to equidistribution](differencing-obstruction-to-equidistribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-76/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-13/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-11/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-79/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-108/3/solution.md)
- [Quadratic exponential sum](quadratic-exponential-sum.md)
- [Quantitative quadratic recurrence](quantitative-quadratic-recurrence.md)
- [Uniform equidistribution of an irrational skew shift](uniform-equidistribution-of-an-irrational-skew-shift.md)
