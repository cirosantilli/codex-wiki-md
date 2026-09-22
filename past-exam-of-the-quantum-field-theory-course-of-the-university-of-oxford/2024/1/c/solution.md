<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a small real time displacement $\epsilon$, the [unitary time evolution](../../../../unitary-time-evolution.md) operator is $T_t(\epsilon)=1-i\epsilon H+O(\epsilon^2)$. The corresponding [Heisenberg picture](../../../../heisenberg-picture.md) field transformation is conjugation by its inverse:

$$
\begin{aligned}
T_t(\epsilon)^\dagger\phi(t,\mathbf x)T_t(\epsilon)
&=\phi+i\epsilon[H,\phi]+O(\epsilon^2)\\
&=\phi+\epsilon\partial_t\phi+O(\epsilon^2)
=\boxed{\phi(t+\epsilon,\mathbf x)+O(\epsilon^2).}
\end{aligned}
$$

Here [a](../a.md) gives $[H,\phi]=-i\partial_t\phi$.

Likewise let $T_s(\mathbf a)=1+i\mathbf a\cdot\mathbf P+O(|\mathbf a|^2)$, with the paper's sign for its [spatial translation operator](../../../../spatial-translation-operator.md). From [b](../b.md),

$$
\begin{aligned}
T_s(\mathbf a)^\dagger\phi(t,\mathbf x)T_s(\mathbf a)
&=\phi+i\mathbf a\cdot[\phi,\mathbf P]+O(|\mathbf a|^2)\\
&=\phi+\mathbf a\cdot\nabla\phi+O(|\mathbf a|^2)
=\boxed{\phi(t,\mathbf x+\mathbf a)+O(|\mathbf a|^2).}
\end{aligned}
$$

These are precisely the first-order [Taylor expansions](../../../../taylor-expansion.md). Since $H$ and $\mathbf P$ commute in this translation-invariant theory, the finite result is

$$
\boxed{\phi(x)=e^{iP\cdot x}\phi(0)e^{-iP\cdot x},\qquad P\cdot x=Ht-\mathbf P\cdot\mathbf x.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
