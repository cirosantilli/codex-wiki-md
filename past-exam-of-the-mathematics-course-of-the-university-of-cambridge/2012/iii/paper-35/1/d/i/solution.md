<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Differentiate once less than might seem necessary: writing $v=h'$ turns the equation into

$$
\frac{v'(z)}{v(z)}=-\frac4\kappa\left(\frac1z+\frac1{z-1}\right).
$$

Uniqueness for this first-order linear equation also covers the solution $v\equiv0$. Thus every solution has $h'(z)=C[z(z-1)]^{-4/\kappa}$. Since $4/\kappa<1$, the derivative is integrable at $1$. The specified boundary value fixes the additive constant, giving

$$
\boxed{h(z)=C\,s_\kappa(z),\qquad
s_\kappa(z)=\int_1^z[v(v-1)]^{-4/\kappa}\,dv,\qquad C>0.}
$$

The strict positivity forces $C>0$; $C=0$ gives the zero function. These are all the positive solutions. The function $s_\kappa$ is the increasing [scale function of a one-dimensional diffusion](../../../../../../../scale-function-stochastic-processes.md) for the ratio process.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2012](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
