<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a nonzero [separable solution](../../../../../../separable-solution.md) $u=XT$, [separation of variables](../../../../../../separation-of-variables.md) gives

$$
\frac{T'}{DT}=\frac{X''}{X}=-\kappa,
\qquad
\boxed{X''+\kappa X=0,\qquad X(0)=X(L)=0.}
$$

These [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) follow because $T$ is not identically zero. If $\kappa=0$, the [affine function](../../../../../../affine-function.md) $X=A+Bx$ obeys both conditions only when $A=B=0$. If $\kappa=-\rho^2<0$, $X=A\cosh(\rho x)+B\sinh(\rho x)$ also has only the zero solution under both conditions.

For $\kappa=\omega^2>0$, $X=A\cos(\omega x)+B\sin(\omega x)$. The first [boundary condition](../../../../../../boundary-condition.md) forces $A=0$, and the second forces $\omega L=n\pi$ for a nonzero solution. Hence all nonzero spatial modes are

$$
\boxed{\kappa_n=\left(\frac{n\pi}{L}\right)^2,\qquad
X_n(x)=B_n\sin\frac{n\pi x}{L},\quad n=1,2,\ldots,\quad B_n\ne0.}
$$

The identically zero [function](../../../../../../function-split.md) is also a solution. Allowing $B_n=0$ includes it in the displayed family. Here $L>0$ is the interval length and $n$ labels the [eigenvalues](../../../../../../eigenvalue.md) of the operator $-d^2/dx^2$ with these [boundary conditions](../../../../../../boundary-condition.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
