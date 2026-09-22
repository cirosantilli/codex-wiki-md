<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

The integral is finite and nonnegative because $|f|$ is [continuous](../../../../../continuous-function.md) on a compact interval. If it vanishes and $f(x_*)\ne0$, continuity gives a relative interval of positive length on which $|f|\geq|f(x_*)|/2$, a contradiction. Thus the integral is zero only for $f=0$. For a real scalar $a$, $\|af\|=|a|\|f\|$, and the pointwise [triangle inequality](../../../../../triangle-inequality.md) $|f+g|\leq|f|+|g|$ integrates to $\|f+g\|\leq\|f\|+\|g\|$. These are all the [norm](../../../../../norm.md) axioms.

The given sequence satisfies

$$
\boxed{\|f_n-0\|=\int_0^1e^{-nx}\,dx=\frac{1-e^{-n}}n\longrightarrow0.}
$$

Hence **it converges to the zero function in this integral [norm](../../../../../norm.md)**. Although $f_n(0)=1$ for all $n$, an isolated endpoint contributes no integral. The pointwise limit is discontinuous, and the sequence does not converge in the [uniform norm](../../../../../supremum-norm.md); neither fact obstructs convergence in the stated [norm](../../../../../norm.md).

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
