<h1 id="18d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [symmetric double-delta potential](../../../../../../symmetric-double-delta-potential.md), take an odd state at $E=-\hbar^2\lambda^2/(2M)$, $\lambda>0$. On $0<x<a$ odd [parity](../../../../../../parity.md) selects $B\sinh(\lambda x)$. For $x>a$, decay and [continuity](../../../../../../continuous-function.md) give $B\sinh(\lambda a)e^{-\lambda(x-a)}$; extend to negative $x$ by oddness. At $x=a$ the jump condition is

$$
-\lambda B\sinh(\lambda a)-\lambda B\cosh(\lambda a)=-\frac{B\sinh(\lambda a)}{\Delta}.
$$

For a nonzero state this means $\lambda\Delta[1+\coth(\lambda a)]=1$, and therefore

$$
\boxed{E=-\frac{\hbar^2\lambda^2}{2M},\qquad\tanh(\lambda a)=\frac{\lambda\Delta}{1-\lambda\Delta}}.
$$

Oddness makes the jump at $-a$ follow automatically: both its derivative jump and its required [wavefunction](../../../../../../wave-function.md) value have the corresponding opposite signs.

There is a positive solution precisely when $\Delta<a$. To see this, rewrite the equation as

$$
\Delta=\frac{1-e^{-2a\lambda}}{2\lambda}.
$$

The right side decreases strictly from $a$ to zero as $\lambda$ increases from zero to infinity: its derivative has the sign of $(1+2a\lambda)e^{-2a\lambda}-1<0$. Hence for $0<\Delta<a$ there is exactly one positive solution, while $\Delta=a$ is a nonnormalizable zero-energy threshold and $\Delta>a$ gives no odd [bound state](../../../../../../bound-state.md). This verifies the stated sufficiently-small-$\Delta$ condition and identifies its exact boundary, consistent with the [odd bound state of a symmetric double-delta potential](../../../../../../odd-bound-state-of-a-symmetric-double-delta-potential.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18D](../../18d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
