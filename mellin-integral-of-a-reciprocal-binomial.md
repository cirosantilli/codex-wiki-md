# Mellin integral of a reciprocal binomial

↑ **Parent:** [Mellin transform](mellin-transform.md)

For real $p>0$ and $0<s<p$, the displayed [improper integral](improper-integral.md) converges: its endpoint powers are $x^{s-1}$ near zero and $x^{s-p-1}$ near infinity. The [change of variables](change-of-variables-formula.md) $t=x^p$ gives

$$
\frac1p\int_0^\infty\frac{t^{s/p-1}}{1+t}dt=\frac1pB(s/p,1-s/p)=\frac{\Gamma(s/p)\Gamma(1-s/p)}p=\frac\pi{p\sin(\pi s/p)}.
$$

Here the [beta function](beta-function.md), the [beta-gamma identity](beta-gamma-identity.md), and the [Gamma reflection formula](gamma-reflection-formula.md) evaluate the integral. The same formula holds for complex $s$ in the [Mellin fundamental strip](fundamental-strip-of-a-mellin-transform.md) $0<\operatorname{Re}s<p$, by absolute convergence and analytic continuation within the strip. For integer $p$, a sector contour of angle $2\pi/p$ gives a direct [residue theorem](residue-theorem.md) proof, with a consistent branch of $z^{s-1}$.

## ↑ Ancestors (6)

1. [Mellin transform](mellin-transform.md)
2. [Integral transform](integral-transform-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2007/paper-2/4/solution.md)
