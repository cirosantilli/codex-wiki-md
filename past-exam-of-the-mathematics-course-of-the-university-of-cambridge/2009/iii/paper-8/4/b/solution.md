<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a bounded self-adjoint $T$, nonnegative spectrum is equivalent to $\langle Tx,x\rangle\geq0$. Here is a useful elementary justification of the nontrivial direction. Let $a=\inf_{\|x\|=1}\langle Tx,x\rangle$ and $S=T-aI$, so $S$ has nonnegative quadratic form. Cauchy-Schwarz for that positive form gives $\|Sx\|^2\leq\|S\|\langle Sx,x\rangle$. Taking unit vectors approaching the infimum makes $Sx_j\to0$, hence $a\in\sigma(T)$. Thus nonnegative spectrum forces $a\geq0$. The reverse direction follows from the lower bound and adjoint argument for $T-\lambda$ when $\lambda<0$, together with reality of the self-adjoint spectrum.

If $T=0$ its positive square root is zero. Otherwise set $M=\|T\|$ and $C=I-T/M$, so $0\leq C\leq I$ and $\|C\|\leq1$. Write the scalar binomial series

$$
\sqrt{1-z}=1-\sum_{n\geq1}a_nz^n,\qquad a_n>0,\quad\sum_{n\geq1}a_n=1.
$$

The last equality follows by taking $z\uparrow1$ in this positive-coefficient series. Consequently

$$
B=\sqrt M\left(I-\sum_{n\geq1}a_nC^n\right)
$$

converges absolutely in operator norm. Each partial sum is positive, because $0\leq C^n\leq I$ and the sum of its coefficients is at most one. The limit is positive and self-adjoint. Multiplying the absolutely convergent series gives $B^2=M(I-C)=T$.

For uniqueness let $R$ be another positive square root. It commutes with $T=R^2$, hence with the polynomial-norm-limit $B$. Thus $(R-B)(R+B)=0$. The kernel of $R+B$ is $\ker R\cap\ker B$: zero quadratic form for a positive operator implies it annihilates the vector, by positive-form Cauchy-Schwarz. The difference $R-B$ vanishes there and on $\operatorname{ran}(R+B)$; the latter is dense in the kernel complement because $R+B$ is self-adjoint. Therefore $R=B$. **The [positive square root of an operator](../../../../../../positive-square-root-of-an-operator.md) exists and is unique.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
