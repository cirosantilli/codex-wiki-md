# String with a central point mass

↑ **Parent:** [Wave equation on a string](wave-equation-on-a-string.md)

A uniform string with fixed ends $x=\pm\ell$, [tension](tension.md) $T$, [linear mass density](linear-mass-density.md) $\rho$, and attached central [point mass](point-mass.md) $m>0$ obeys the [wave equation](wave-equation-split.md) away from zero, continuous displacement at zero, and $m y_{tt}(0,t)=T[y_x(0^+,t)-y_x(0^-,t)]$. The [normal modes](normal-mode.md) split into antisymmetric modes that leave the mass at rest and symmetric modes that move it.

To prove the spectral equations, use $X=A\sin(k(x+\ell))$ on the left and $X=B\sin(k(\ell-x))$ on the right, with $\omega^2=(T/\rho)k^2$. Continuity gives $(A-B)\sin(k\ell)=0$ and the force law gives $Tk(A+B)\cos(k\ell)=m\omega^2A\sin(k\ell)$. If $\sin(k\ell)=0$, then $k\ell=n\pi$, $n\geq1$, and $B=-A$. Otherwise $A=B$ and cancellation gives $\cot(k\ell)=mk/(2\rho)$. In dimensionless variables $z=k\ell$, $\alpha=m/(2\rho\ell)$, strict [monotonicity](monotonic-function.md) gives one symmetric root in each $(n\pi,n\pi+\pi/2)$, $n\geq0$. The apparent zero root of the sine equation has only the zero profile and is excluded.

For $m/(\rho\ell)\gg1$, the lowest root tends to zero. The [Taylor series](taylor-series.md) $\cot z=1/z-z/3+O(z^3)$ gives $z\sim\alpha^{-1/2}$ and hence $\omega\sim\sqrt{2T/(m\ell)}$. The two nearly straight half-strings supply a restoring [force](force-split.md) $-2TY/\ell$, explaining this [harmonic oscillator](simple-harmonic-motion.md) limit.

## ↑ Ancestors (7)

1. [Wave equation on a string](wave-equation-on-a-string.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2023/prelims/mathematics-v/6/b/solution.md)
