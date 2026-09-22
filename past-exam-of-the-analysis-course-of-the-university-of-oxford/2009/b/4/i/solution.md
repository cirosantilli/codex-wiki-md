<h1 id="b/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A complete [orthonormal sequence](../../../../../orthonormal-sequence.md) $(e_n)$ has $\langle e_n,e_m\rangle=\delta_{nm}$ and dense [linear span](../../../../../linear-span.md); equivalently, the only vector orthogonal to every $e_n$ is zero. The [Parseval identity](../../../../../parseval-identity.md) says $\|x\|^2=\sum_n|\langle x,e_n\rangle|^2$, with expansion $x=\sum_n\langle x,e_n\rangle e_n$ in the Hilbert [norm](../../../../../norm.md).

Put $G(t,z)=(1-2zt+z^2)^{-1/2}$ and $D=1-2zt+z^2$. Direct differentiation gives

$$
G_t=zD^{-3/2},\quad G_{tt}=3z^2D^{-5/2},\quad G_z=(t-z)D^{-3/2},\quad G_{zz}=-D^{-3/2}+3(t-z)^2D^{-5/2}.
$$

Substitution yields $(1-t^2)G_{tt}-2tG_t+z^2G_{zz}+2zG_z=0$. Extracting the coefficient of $z^n$ in the [generating function](../../../../../generating-function.md) gives

$$
\boxed{(1-t^2)P_n''-2tP_n'+n(n+1)P_n=0,}
$$

the [Legendre differential equation](../../../../../legendre-differential-equation.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
