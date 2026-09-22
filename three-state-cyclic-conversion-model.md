# Three-state cyclic conversion model

↑ **Parent:** [Linear system of differential equations](linear-system-of-differential-equations.md)

Three nonnegative amounts convert in the directed cycle $A\to B\to C\to A$ at positive first-order rates $a,b,c$. The [linear system of ordinary differential equations](linear-system-of-differential-equations.md) conserves $A+B+C=N$. Its [characteristic polynomial](characteristic-polynomial.md) is $\lambda[\lambda^2+(a+b+c)\lambda+ab+bc+ca]$. The two nonzero [eigenvalues](eigenvalue.md) have negative [real part](real-part.md), so every trajectory converges to the unique [steady state](steady-state.md) with that total:

$$
(A_\infty,B_\infty,C_\infty)=\frac{N}{ab+bc+ca}(bc,ca,ab).
$$

This is also a column-convention [continuous-time Markov chain](continuous-time-markov-chain-split.md) after normalizing by $N>0$: every component loses to one successor and receives from one predecessor. A complex-conjugate pair produces damped oscillations about equilibrium even though the amounts remain nonnegative. A repeated nonzero [eigenvalue](eigenvalue.md) is defective and requires a [Jordan chain](jordan-chain.md).

**Table of contents**

- [Defective repeated eigenvalue in a cyclic conversion model](defective-repeated-eigenvalue-in-a-cyclic-conversion-model.md)

## ↑ Ancestors (8)

1. [Linear system of differential equations](linear-system-of-differential-equations.md)
2. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Defective repeated eigenvalue in a cyclic conversion model](defective-repeated-eigenvalue-in-a-cyclic-conversion-model.md)
- [Solution](past-exam-of-the-mathematical-methods-i-course-of-the-university-of-oxford/2014/11/i/solution.md)
