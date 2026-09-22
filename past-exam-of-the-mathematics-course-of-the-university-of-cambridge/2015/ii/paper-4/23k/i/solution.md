<h1 id="23k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $h(x)>0$, so the conditioning event has positive probability. For a continuous-time [Markov chain](../../../../../../markov-chain.md), write $\tau_y=\int_0^{T_A}\mathbf1_{\{X_s=y\}}\,ds$. At each time $s<T_A$, the [Markov property](../../../../../../markov-property.md) gives $\mathbb P(T_A<\infty\mid\mathcal F_s)=h(X_s)$. Using [Tonelli theorem](../../../../../../tonelli-theorem.md) for the nonnegative occupation integral,

$$
\mathbb E_x[\tau_y\mathbf1_{\{T_A<\infty\}}]
=\int_0^\infty\mathbb E_x[\mathbf1_{\{s<T_A,X_s=y\}}h(y)]\,ds
=h(y)\mathbb E_x\tau_y.
$$

Division by $h(x)$ yields $\boxed{\mathbb E_x[\tau_y\mid T_A<\infty]=[h(y)/h(x)]\mathbb E_x\tau_y}$. The discrete-time proof replaces the integral by a sum. Infinite expectations are allowed in the nonnegative sense; if $h(y)=0$, the numerator is zero directly, avoiding an ambiguous product of zero and infinity.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [23K](../../23k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
