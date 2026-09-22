<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $E_0=\hbar\omega/2$. Repeated application of the [annihilation operator](../../../../../annihilation-operator.md) lowers the [energy eigenvalue](../../../../../energy-eigenvalue-split.md) in steps of $\hbar\omega$. The lower bound from part (ii) forces this process to stop. To see why it also quantizes the starting energy, write

$$
\frac{E-E_0}{\hbar\omega}=n+\delta,\qquad n\in\{0,1,2,\ldots\},\quad 0\leq\delta<1.
$$

The first $n$ lowering steps have positive squared [norms](../../../../../norm.md). If $\delta>0$, the next step is also nonzero by part (ii), and its energy would be $E_0+(\delta-1)\hbar\omega<E_0$, contradicting the bound. Thus $\delta=0$, and

$$
\boxed{E_n=\left(n+\frac12\right)\hbar\omega,\qquad n=0,1,2,\ldots.}
$$

Existence of the [ground state](../../../../../ground-state.md) can also be checked directly in the position representation. The equation $a_-\psi_0=0$ is

$$
-i\hbar\psi_0'-im\omega x\psi_0=0,
$$

whose solution is proportional to $e^{-m\omega x^2/(2\hbar)}$. This [Gaussian function](../../../../../gaussian-function.md) is [square-integrable](../../../../../square-integrable-function.md), so it gives an actual [ground state](../../../../../ground-state.md). Its normalization can be chosen using the [Gaussian integral](../../../../../gaussian-integral.md).

All the displayed levels occur: for a nonzero state at $E_n$,

$$
\|a_+\psi_n\|^2=\langle\psi_n,a_-a_+\psi_n\rangle=2m\hbar\omega(n+1)\|\psi_n\|^2>0.
$$

Thus repeated raising creates a nonzero [energy eigenstate](../../../../../energy-eigenstate.md) at every $E_n$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
