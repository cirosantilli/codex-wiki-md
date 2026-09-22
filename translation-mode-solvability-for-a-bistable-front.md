# Translation-mode solvability for a bistable front

↑ **Parent:** [Fredholm solvability condition](fredholm-solvability-condition.md)

Suppose $u_t=Du_{xx}+f_0(u)+\varepsilon h(u)$ has a balanced stationary front $U_0(z)$, where $z=(x-q)/\sqrt D$ and $U_0''+f_0(U_0)=0$. Take $\dot q/\sqrt D=\varepsilon c_1+\cdots$ and $u=U_0+\varepsilon U_1+\cdots$. At first order, $LU_1=-c_1U_0'-h(U_0)$ with $L=d^2/dz^2+f_0'(U_0)$. Differentiating the front equation proves $LU_0'=0$. Integration by parts against the decaying [translation](translation-geometry.md) mode gives

$$
c_1=-\frac{\int_{-\infty}^\infty U_0'h(U_0)\,dz}{\int_{-\infty}^\infty(U_0')^2\,dz}.
$$

This is the [Fredholm solvability condition](fredholm-solvability-condition.md) determining the velocity, derived from the [self-adjoint differential operator](self-adjoint-differential-operator.md) rather than assumed. An orthogonality condition or a fixed midpoint removes the freedom to add a multiple of $U_0'$ to $U_1$. For the [bistable cubic reaction-diffusion equation](bistable-cubic-reaction-diffusion-equation.md), $h=-aU_0(1-U_0)$ gives $c_1=-\sqrt2a$, and its first-order forcing vanishes pointwise, so the phase-fixed shape correction is zero.

**Table of contents**

- [Moving-defect locking of a cubic-quintic front](moving-defect-locking-of-a-cubic-quintic-front.md)

## ↑ Ancestors (8)

1. [Fredholm solvability condition](fredholm-solvability-condition.md)
2. [Solvability condition at a Sturm-Liouville eigenvalue](solvability-condition-at-a-sturm-liouville-eigenvalue.md)
3. [Self-adjoint differential operator](self-adjoint-differential-operator.md)
4. [Sturm-Liouville theory](sturm-liouville-theory.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-75/2/solution.md)
