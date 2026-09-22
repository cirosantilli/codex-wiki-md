# Step-function proof of the Riemann-Lebesgue lemma

↑ **Parent:** [Riemann-Lebesgue lemma](riemann-lebesgue-lemma.md)

For a continuous real [function](function-split.md) $f$ on $[a,b]$, [uniform step approximation on a compact interval](uniform-step-approximation-on-a-compact-interval.md) gives a finite [step function](step-function.md) $g=\sum_jc_j\mathbf1_{I_j}$ with small uniform error. Each cosine integral over an interval has absolute value at most $2/|\omega|$. Therefore

$$
\left|\int_a^bf(t)\cos(\omega t)\,dt\right|
\le(b-a)\|f-g\|_\infty+\frac2{|\omega|}\sum_j|c_j|.
$$

First choose $g$ to make the first term small, then let $|\omega|$ grow with $g$ fixed. This proves the cosine version of the [Riemann-Lebesgue lemma](riemann-lebesgue-lemma.md) without differentiating $f$; the sine and complex-exponential versions follow in the same way.

## ↑ Ancestors (6)

1. [Riemann-Lebesgue lemma](riemann-lebesgue-lemma.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/12f/solution.md)
