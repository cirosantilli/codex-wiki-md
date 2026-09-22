<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

For an incident particle from the left, take $E>0$ and $E>V_0$, and define

$$
k=\frac{\sqrt{2mE}}\hbar,\qquad q=\frac{\sqrt{2m(E-V_0)}}\hbar.
$$

The [Time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) gives an incident plus reflected [plane wave](../../../../../plane-wave.md) on the left and an outgoing transmitted [plane wave](../../../../../plane-wave.md) on the right:

$$
\psi(x)=e^{ikx}+re^{-ikx}\quad(x<0),\qquad \psi(x)=te^{iqx}\quad(x>0).
$$

[Continuity](../../../../../continuous-function.md) of the [wavefunction](../../../../../wave-function.md) and its [derivative](../../../../../derivative.md) at a finite potential jump yields $1+r=t$ and $k(1-r)=qt$. Hence $r=(k-q)/(k+q)$ and $t=2k/(k+q)$. The incident and reflected [probability currents](../../../../../probability-current.md) have equal wave-number magnitude, so

$$
\boxed{P=|r|^2=\left(\frac{\sqrt E-\sqrt{E-V_0}}{\sqrt E+\sqrt{E-V_0}}\right)^2}.
$$

As a check, the transmitted current fraction is $(q/k)|t|^2=4kq/(k+q)^2$, and the two probabilities sum to one.

For a positive step, $E\downarrow V_0$ makes $q\downarrow0$, so **$P\to1$**. For a negative step with fixed positive incident energy, $V_0\to-\infty$ makes $q\to\infty$, so again **$P\to1$**. The latter is quantum reflection from an increasingly large wave-number mismatch, even though the step is downward.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
