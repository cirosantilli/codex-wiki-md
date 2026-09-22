<h1 id="sophomore-s-dream">Sophomore's dream</h1>

↑ **Parent:** [Integral](integral-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sophomore's_dream)

The two identities are

$$
\int_0^1x^{-x}\,dx=\sum_{n=1}^\infty n^{-n},\qquad
\int_0^1x^x\,dx=\sum_{n=1}^\infty(-1)^{n-1}n^{-n}.
$$

To prove them, expand $e^{\pm x\log x}$ in its [exponential series](exponential-series.md). Since $|x\log x|\leq1/e$ on $(0,1)$, the [Weierstrass M-test](weierstrass-m-test.md) justifies termwise integration. Substituting $x=e^{-t}$ gives $\int_0^1x^k(\log x)^k\,dx=(-1)^kk!/(k+1)^{k+1}$ through the [gamma function](gamma-function.md). Inserting these moments into the series and shifting $n=k+1$ proves both formulas. Each resulting numerical [series](series-mathematics.md) has [absolute convergence](absolute-convergence.md).

## ↑ Ancestors (7)

1. [Integral](integral-split.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-integration-course-of-the-university-of-oxford/2021/1/c/ii/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2011/d/d4/c/solution.md)
- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2011/d/d4/d/solution.md)
