<h1 id="6b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a finite [potential energy](../../../../../../potential-energy.md) discontinuity, the [stationary state](../../../../../../stationary-state.md) $\psi$ and its first [derivative](../../../../../../derivative.md) are [continuous](../../../../../../continuous-function.md) at $a$. Integrating the [Time-independent Schrödinger equation](../../../../../../time-independent-schrodinger-equation.md) across a shrinking interval about $a$ gives continuity of $\psi'$; a jump in $\psi$ would produce a [distributional derivative](../../../../../../distributional-derivative.md) incompatible with a finite [potential energy](../../../../../../potential-energy.md).

For $E>V_0$, put $k=\sqrt{2mE}/\hbar$, $q=\sqrt{2m(E-V_0)}/\hbar$ and use unit incident amplitude:

$$
\psi(x)=\begin{cases}e^{ik(x-a)}+r e^{-ik(x-a)},&x<a,\\t e^{iq(x-a)},&x>a.\end{cases}
$$

There is no wave incident from the right. The matching equations $1+r=t$, $k(1-r)=qt$ give $r=(k-q)/(k+q)$ and $t=2k/(k+q)$. Comparing reflected and incident [probability currents](../../../../../../probability-current.md) gives the [reflection coefficient](../../../../../../reflection-coefficient.md)

$$
\boxed{R(E)=\left(\frac{\sqrt E-\sqrt{E-V_0}}{\sqrt E+\sqrt{E-V_0}}\right)^2\quad(E>V_0)}.
$$

The transmitted fraction is $T=(q/k)|t|^2=4kq/(k+q)^2$, so $R+T=1$.

For $0<E<V_0$, write $\kappa=\sqrt{2m(V_0-E)}/\hbar$ and retain only the decaying right-hand solution $t e^{-\kappa(x-a)}$. Matching gives $r=(k-i\kappa)/(k+i\kappa)$, which has modulus one. The [evanescent wave](../../../../../../evanescent-wave.md) carries no transmitted [probability current](../../../../../../probability-current.md). At $E=V_0$, the bounded right-hand solution is constant and matching again gives $r=1$. Thus

$$
\boxed{R(E)=1\quad(0<E\leq V_0)}.
$$

Classically, a particle is wholly transmitted for $E>V_0$ and wholly reflected for $E<V_0$; there is no classical partial reflection above the step. At the threshold it has zero right-hand speed and no transmitted flux, a marginal case requiring a convention about motion exactly on the discontinuity. The quantum result approaches $R=0$ as $E/V_0\to\infty$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6B](../../6b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
