# Finite Hilbert transform inversion

↑ **Parent:** [Finite Hilbert transform](finite-hilbert-transform.md)

For $G\in C^1([0,1])$, the displayed expression solves $Tf=G$, where $T=H_{(0,1)}/i$ and $H_{(0,1)}$ is the [finite Hilbert transform](finite-hilbert-transform.md) with denominator $t-x$. To derive it, put $S(z)=\sqrt{z(z-1)}\sim z$ at [infinity](infinity.md), take $h$ to be the [Cauchy transform](cauchy-transform.md) of $i\rho G$, and set $w=h/S$. The [Sokhotski–Plemelj formula](sokhotski-plemelj-theorem.md) gives $w_++w_-=G$ and the displayed jump $f=w_+-w_-$. The endpoint behavior is at most inverse [square root](square-root.md), and $w=O(z^{-2})$ at [infinity](infinity.md). [Cauchy reconstruction from a jump across a finite interval](cauchy-reconstruction-from-a-jump-across-a-finite-interval.md) then gives $w=C[f]$ and hence $Tf=G$. Adding any constant multiple of $1/\rho$ gives another solution in the integrable endpoint class.

Multiplying an auxiliary sign-changing factor by a growing analytic factor can invalidate this reconstruction. For example, using $S$ instead of $1/S$ with $G=1$ produces the constant [function](function-split.md) $w=1/2$ and zero jump. The [boundary](boundary-of-a-set.md) sum alone is not enough: the entire remainder in reconstructing $w$ from its jump must also be controlled.

## ↑ Ancestors (7)

1. [Finite Hilbert transform](finite-hilbert-transform.md)
2. [Hilbert transform](hilbert-transform.md)
3. [Fourier transform](fourier-transform-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-applied-complex-variables-course-of-the-university-of-oxford/2011/2/b/solution.md)
