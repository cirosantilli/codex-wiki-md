<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [matrix splitting](../../../../../matrix-splitting.md) produces $Mx^{(k+1)}=Nx^{(k)}+b$. If the iterates converge to $z$, passing to the limit yields $Mz=Nz+b$, hence $Az=b$. Thus any finite limit solves the system; when $A$ is nonsingular it is the unique solution.

The [iteration matrix](../../../../../iteration-matrix.md) is $G=M^{-1}N=I-M^{-1}A$. For $M$ symmetric positive definite, its positive-definite square root gives

$$
\boxed{M^{1/2}GM^{-1/2}=I-M^{-1/2}AM^{-1/2},}
$$

which is symmetric when $A$ is symmetric. Let $\theta_i$ be the [eigenvalues](../../../../../eigenvalue.md) of $\widetilde A=M^{-1/2}AM^{-1/2}$. In its orthonormal eigenbasis the transformed error is multiplied by $1-\theta_i$ at each step. Therefore convergence to the unique solution for every starting vector is equivalent to

$$
\boxed{|1-\theta_i|<1\text{ for all }i\quad\Longleftrightarrow\quad0<\theta_i<2\text{ for all }i.}
$$

Sufficiency follows because each scalar mode tends to zero. Necessity follows by starting with a nonzero error in any mode whose multiplier has modulus at least one. Equivalently the condition says $\boxed{A\text{ and }2M-A\text{ are positive definite}}$, by congruence of their quadratic forms.

Under the usual nonsingularity assumption, a symmetric $A$ that is not positive definite has a negative quadratic direction. Its congruent $\widetilde A$ then has a negative [eigenvalue](../../../../../eigenvalue.md), making an error multiplier $1-\theta_i>1$. A starting error in that mode diverges, proving the final claim in that setting.

If singular matrices are permitted, the last claim needs qualification. A zero [eigenvalue](../../../../../eigenvalue.md) gives a persistent error mode, but the iterates may still converge to another solution of a compatible singular system. For example $A=0$, $M=I$, $b=0$ makes every iterate constant and already a solution, despite $A$ not being positive definite. Thus literal nonconvergence cannot be deduced from a zero eigenvalue alone.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
