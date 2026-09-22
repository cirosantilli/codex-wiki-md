<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $\alpha^2+\beta^2=1$ and label the first vector of each measurement basis by outcome $0$. Assign the [Pauli measurement](../../../../../../measurement-of-a-pauli-observable.md) value $+1$ to outcome $0$ and $-1$ to outcome $1$. The four observables are

$$
A_1=Z,\qquad A_2=X,\qquad
B_1=\frac{\sqrt3}{2}X+\frac12 Z,\qquad
B_2=\frac{\sqrt3}{2}X-\frac12 Z.
$$

Here $X$ and $Z$ are the [Pauli X gate](../../../../../../pauli-x-gate.md) and [Pauli Z gate](../../../../../../pauli-z-gate.md) matrices. These follow by subtracting the two rank-one basis projectors; a real basis rotated through $\gamma$ has observable $\sin(2\gamma)X+\cos(2\gamma)Z$.

The [Schmidt-basis Pauli correlation tensor](../../../../../../schmidt-basis-pauli-correlation-tensor.md) of the state gives

$$
\langle Z\otimes Z\rangle=1,\quad \langle X\otimes X\rangle=2\alpha\beta,\quad
\langle X\otimes Z\rangle=\langle Z\otimes X\rangle=0.
$$

Consequently $E_{11}=1/2$, $E_{21}=E_{22}=\sqrt3\alpha\beta$ and $E_{12}=-1/2$, where $E_{jk}=\langle A_j\otimes B_k\rangle$. For binary outcomes, $\mathbb E\big([A-B]_2\big)=P(A\ne B)=(1-E_{AB})/2$, whereas the final offset term has $\mathbb E\big([B-A-1]_2\big)=P(A=B)=(1+E_{AB})/2$. The [chained modular Bell inequality](../../../../../../chained-modular-bell-inequality.md) left side is therefore

$$
I=\frac{1-E_{11}}2+\frac{1-E_{21}}2+\frac{1-E_{22}}2+\frac{1+E_{12}}2
=\boxed{\frac32-\sqrt3\alpha\beta}.
$$

The local bound is $I\geq1$, so the exact violation condition is

$$
\boxed{\alpha\beta>\frac1{2\sqrt3},\qquad \alpha^2+\beta^2=1}.
$$

Equality saturates the bound. The maximal violation for these fixed measurements occurs at $\alpha=\beta=1/\sqrt2$ or their common negative, giving $I=(3-\sqrt3)/2$. Opposite signs do not violate this particular inequality with these fixed bases, although other measurement choices can reveal the state's [entanglement](../../../../../../entangled-state.md). If unnormalized real amplitudes are used, replace $\alpha\beta$ throughout by $\alpha\beta/(\alpha^2+\beta^2)$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
