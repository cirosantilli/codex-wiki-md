# Half-line Green function for the first cylindrical harmonic

↑ **Parent:** [Green's function](green-s-function-split.md)

For $Ly=y''+y'/x-y/x^2$ on $x>0$, impose $y(0)=0$ by a continuous limit and $y(x)\to0$ at infinity. The adapted homogeneous solutions are $x$ at zero and $1/x$ at infinity, with [Wronskian](wronskian.md) $-2/x$. The displayed [Green function](green-s-function-split.md) is continuous and its first [derivative](derivative.md) has jump one at $x=s$, so $L_xG(x,s)=\delta(x-s)$ with ordinary source measure $ds$. For continuous $f$ with $\int_0^\infty(1+s^2)|f(s)|ds<\infty$,

$$
y(x)=\int_0^\infty G(x,s)f(s)ds=-\frac1{2x}\int_0^xs^2f(s)ds-\frac x2\int_x^\infty f(s)ds.
$$

This solves $Ly=f$ with the stated endpoint limits. No nonzero combination of $x,1/x$ meets both homogeneous endpoint conditions, proving [uniqueness](uniqueness.md). Multiplying $L$ by $x$ gives the self-adjoint expression $(xy')'-y/x$, explaining the weighted reciprocity $xG(x,s)=sG(s,x)$.

## ↑ Ancestors (5)

1. [Green's function](green-s-function-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/8/solution.md)
