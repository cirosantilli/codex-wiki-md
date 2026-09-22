<h1 id="38c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One form of the [Householder-John theorem](../../../../../../householder-john-theorem.md) is as follows. Suppose $A=A^*$ and $A=M-N$, with $M$ invertible and $W=M+M^*-A$ positive definite. Then the stationary iteration $Mx^{(k+1)}=Nx^{(k)}+b$ converges for every initial vector exactly when $A$ is positive definite; its iteration matrix is $B=M^{-1}N$ and convergence means [spectral radius](../../../../../../spectral-radius.md) below one.

For a known positive definite system, design a splitting with $M$ easy to solve, such as diagonal or triangular, and arrange $M+M^*-A>0$. The theorem then guarantees convergence. For example $M=sI$ has $W=2sI-A>0$ when $2s$ exceeds the largest [eigenvalue](../../../../../../eigenvalue.md) of $A$. In the converse direction, the discrete energy identity $A-B^*AB=(I-B)^*W(I-B)$ explains the criterion: stable $B$ gives $A$ as a convergent sum of positive matrices, while positive $A,W$ force every iteration [eigenvalue](../../../../../../eigenvalue.md) inside the unit disk.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38C](../../38c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
