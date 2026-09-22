<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [spectrum of a bounded operator](../../../../spectrum-of-a-bounded-operator.md) is $\sigma(T)=\{\lambda:\lambda I-T\text{ has no bounded two-sided inverse}\}$. Its [point spectrum](../../../../point-spectrum.md) is the set of eigenvalues, where $\lambda I-T$ is not [injective](../../../../injective-function.md).

Here $T$ is linear and takes [continuous](../../../../continuous-function.md) functions to continuously differentiable functions. Also $\|Tx\|_\infty\leq2\|x\|_\infty$; the constant function one attains this bound at $t=1$, so $\|T\|=2$. Its range is contained in $C^1([0,1])$, a proper subset of $C([0,1])$, so zero is in its spectrum. It is not an [eigenvalue](../../../../eigenvalue.md): $Tx=0$ gives $x(0)=0$ at zero and $x=0$ upon differentiation.

For a nonzero [eigenvalue](../../../../eigenvalue.md), $\lambda x=Tx$ implies $x'=x/\lambda$ and $(\lambda-1)x(0)=0$. A nonzero solution is therefore possible exactly at $\lambda=1$, with eigenfunctions $x(t)=ce^t$. Hence $p\sigma(T)=\{1\}$.

For the proposed [resolvent](../../../../resolvent-of-an-operator.md) put

$$
F(t)=e^{t/\lambda}\int_0^t y(s)e^{-s/\lambda}ds,\qquad F'=y+F/\lambda.
$$

The proposed $x$ is $y/\lambda+y(0)e^{t/\lambda}/[\lambda(\lambda-1)]+F/\lambda^2$. Consequently $x(0)=y(0)/(\lambda-1)$ and

$$
\int_0^tx(s)ds=\frac{F(t)}\lambda+\frac{y(0)}{\lambda-1}(e^{t/\lambda}-1).
$$

Adding $x(0)$ and subtracting from $\lambda x(t)$ gives exactly $y(t)$. Thus $\lambda I-T$ is onto for $\lambda\ne0,1$. It is also [injective](../../../../injective-function.md) by the [eigenvalue](../../../../eigenvalue.md) calculation. The displayed formula defines a bounded map in the [supremum norm](../../../../supremum-norm.md), since its exponential kernels are bounded on the [compact](../../../../compact-space.md) interval. It is therefore the [bounded inverse](../../../../bounded-inverse.md), and

$$
\boxed{\sigma(T)=\{0,1\},\qquad p\sigma(T)=\{1\}.}
$$

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
