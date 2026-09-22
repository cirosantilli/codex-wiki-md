<h1 id="b/6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The [Jacobian matrix](../../../../../jacobian-matrix.md) of $F_\mu$ in $(x,y)$ is

$$
J(v)=\begin{pmatrix}H(x,y)&-A(x)^T\\Y A(x)&C(x)\end{pmatrix}.
$$

The top-left block is the [Hessian matrix](../../../../../hessian-matrix.md) of $f-y^Tc$ with $y$ held fixed. In the second block, differentiating $C(x)y$ in $x$ gives $YA$ and in $y$ gives $C$. The explicit derivative with respect to $\mu$ is $(0,-e)^T$. Differentiate $F_\mu(v(\mu))=0$ by the [chain rule](../../../../../chain-rule.md):

$$
\boxed{\begin{pmatrix}H&-A^T\\YA&C\end{pmatrix}\begin{pmatrix}x'(\mu)\\y'(\mu)\end{pmatrix}=\begin{pmatrix}0\\e\end{pmatrix}.}
$$

All blocks are evaluated on the current [central path](../../../../../central-path.md) point.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
