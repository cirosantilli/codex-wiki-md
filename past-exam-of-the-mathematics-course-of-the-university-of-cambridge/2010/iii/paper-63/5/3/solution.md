<h1 id="5/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The $[1/1]$ [Padé approximant](../../../../../../pade-approximant.md) of the exponential is $r(z)=(1+z/2)/(1-z/2)$. Replacing each exponential in its original order gives the split [Crank-Nicolson method](../../../../../../crank-nicolson-method.md)

$$
u^{n+1}=C_A(\delta)C_B(\delta)u^n,
\qquad C_A(\delta)=(I-\delta A/2)^{-1}(I+\delta A/2),
$$

with the analogous definition for $B$. Operationally, first solve the $B$ substep and then the $A$ substep. The matrices $I-\delta A/2$, $I-\delta B/2$ are invertible for every $\delta\ge0$, since $A,B$ are symmetric negative definite.

An orthonormal eigenbasis of $A$ diagonalizes $C_A$. Its [eigenvalue](../../../../../../eigenvalue.md) for $\lambda\le0$ is

$$
r(\delta\lambda)=\frac{1+\delta\lambda/2}{1-\delta\lambda/2},\qquad
|r(\delta\lambda)|\le1.
$$

Therefore $\|C_A\|_h\le1$, and similarly $\|C_B\|_h\le1$. Submultiplicativity gives the [contractivity of split Crank-Nicolson diffusion](../../../../../../contractivity-of-split-crank-nicolson-diffusion.md):

$$
\boxed{\|u^{n+1}\|_h\le\|u^n\|_h\quad\text{for every }\mu=\Delta t/h^2\ge0.}
$$

No commutativity or simultaneous diagonalization is needed for this product bound. This proves unconditional discrete $L^2$ stability, not positivity of every stencil weight or unconditional maximum-norm monotonicity. Nor do the individually second-order rational substeps make the ordered splitting second order: when $[A,B]\ne0$, its leading splitting defect remains $\delta^2[A,B]/2$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [5](../../5.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
