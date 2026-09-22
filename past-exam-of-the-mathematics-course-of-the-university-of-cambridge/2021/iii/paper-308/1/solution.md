<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Differentiating the potential gives

$$
U'(\phi)=2(1-\phi^2)(\epsilon-\phi).
$$

Thus $\phi=\pm1$ are stationary points, and

$$
U''(1)=4(1-\epsilon)>0,
\qquad
U''(-1)=4(1+\epsilon)>0
$$

because $|\epsilon|<1$. Both are local minima. Their energies are

$$
U(1)=\frac{4\epsilon}{3},
\qquad
U(-1)=-\frac{4\epsilon}{3}.
$$

For $\epsilon=0$, the static energy can be completed to a square:

$$
E=\int dx\left\{\frac12[\phi'-(1-\phi^2)]^2
+\phi'(1-\phi^2)\right\}.
$$

The increasing [scalar-field kink](../../../../../scalar-field-kink.md) therefore obeys the first-order [Bogomolny equation](../../../../../bogomolny-equations.md)

$$
\boxed{\phi'=1-\phi^2}.
$$

With center $X$, its solution and energy are

$$
\boxed{\phi_K(x)=\tanh(x-X)},
\qquad
\boxed{E_K=\int_{-1}^{1}(1-\phi^2)\,d\phi=\frac43}.
$$

The antikink uses the opposite sign.

For small positive $\epsilon$, the true vacuum $\phi=-1$ lies below the false vacuum $\phi=1$ by

$$
\Delta U=U(1)-U(-1)=\frac{8\epsilon}{3}.
$$

This pressure exerts force $\Delta U$ on a kink with $-1$ on its left and $+1$ on its right. Dividing by its leading mass $4/3$ gives acceleration toward the false-vacuum side:

$$
\boxed{\ddot X=2\epsilon+O(\epsilon^2)}.
$$

An antikink followed by a kink encloses a region of the lower vacuum while approaching $\phi=1$ at both infinities. Vacuum pressure pushes the pair apart, whereas their attraction pulls them together. At a static separation $s$,

$$
\frac{8\epsilon}{3}=32e^{-2s},
$$

so

$$
\boxed{s\simeq\frac12\log\frac{12}{\epsilon}}.
$$

This estimate is self-consistent for $\epsilon\ll1$, when the two soliton cores are well separated.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
