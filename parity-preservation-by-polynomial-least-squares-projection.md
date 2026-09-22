# Parity preservation by polynomial least-squares projection

↑ **Parent:** [Polynomial least-squares approximation](polynomial-least-squares-approximation.md)

On a symmetric interval with an even positive weight, the best [least-squares polynomial](polynomial-least-squares-approximation.md) approximation to an [odd](odd-function.md) function is odd, and the approximation to an [even](even-function.md) function is even. Indeed, the even and odd [polynomial](polynomial-split.md) subspaces are [orthogonal](orthogonal-vectors.md). For odd $u$, write a candidate as $p=p_o+p_e$. Then

$$
\|u-p\|^2=\|u-p_o\|^2+\|p_e\|^2.
$$

Deleting a nonzero even component strictly reduces the error, so the minimizer has $p_e=0$. The same argument exchanges the parities for even $u$. This reduces the [normal equations](normal-equation.md) to the matching parity block and avoids computing coefficients known in advance to vanish.

## ↑ Ancestors (7)

1. [Polynomial least-squares approximation](polynomial-least-squares-approximation.md)
2. [Polynomial approximation](polynomial-approximation.md)
3. [Uniform approximation](uniform-approximation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/2/c/solution.md)
- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2014/2/d/solution.md)
