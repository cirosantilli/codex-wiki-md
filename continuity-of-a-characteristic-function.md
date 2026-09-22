# Continuity of a characteristic function

↑ **Parent:** [Characteristic function](characteristic-function-split.md)

Every characteristic function is uniformly continuous and satisfies $\varphi(0)=1$ and $|\varphi(t)|\leq1$. Continuity follows from the [dominated convergence theorem](dominated-convergence-theorem.md) applied to $e^{itX}$.

More explicitly, if $t_n\to t$, then $e^{it_nX}\to e^{itX}$ pointwise and $|e^{it_nX}|=1$. Apply the [dominated convergence theorem](dominated-convergence-theorem.md) to the [real part](real-part.md) and [imaginary part](imaginary-part.md) separately. There is no finite [moment](moment.md) hypothesis. For [uniform continuity](uniform-continuity.md), the stronger estimate

$$
\sup_{t\in\mathbb R}|\varphi_X(t+h)-\varphi_X(t)|
\leq\mathbb E[|e^{ihX}-1|]\longrightarrow0
\qquad(h\to0)
$$

follows by factoring out $e^{itX}$, whose absolute value is one. The integrand tends pointwise to zero and is bounded by two, so the [dominated convergence theorem](dominated-convergence-theorem.md) applies again. The bound is independent of $t$, which supplies [uniform continuity](uniform-continuity.md) on the entire real line.[Theorem 3.3.1(d) and proof, printed p. 126](probability-theory-and-examples-fifth-edition-by-rick-durrett.md)

If the first [absolute moment](absolute-moment.md) is finite, $|e^{iu}-1|\leq|u|$ additionally gives $|\varphi_X(t+h)-\varphi_X(t)|\leq|h|\mathbb E[|X|]$, a [Lipschitz continuity](lipschitz-continuity.md) estimate. The earlier argument matters because [continuity](continuous-function.md) survives even when this [expected value](expected-value-split.md) is infinite. For [convergence in distribution](convergence-in-distribution.md), the separate [Lévy continuity theorem](levy-continuity-theorem.md) concerns limits of whole sequences of [characteristic functions](characteristic-function-split.md); the argument here establishes [continuity](continuous-function.md) of one [characteristic function](characteristic-function-split.md).

## ↑ Ancestors (6)

1. [Characteristic function](characteristic-function-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Characteristic-function derivatives from finite absolute moments](characteristic-function-derivatives-from-finite-absolute-moments.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/27k/b/i/solution.md)
