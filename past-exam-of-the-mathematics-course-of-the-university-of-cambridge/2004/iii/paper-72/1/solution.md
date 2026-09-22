<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $B_{i\alpha}=\dot A_{i\alpha}$ and assume that the material constraint is regular, so $F_{,A}\ne0$. Differentiating the constraint shows that admissible rates of the [deformation gradient](../../../../../deformation-gradient.md) satisfy $F_{,A_{i\alpha}}B_{i\alpha}=0$. The given stress-power identity says that $W_{,A}-N^T$ annihilates this tangent hyperplane. Its orthogonal complement is the one-dimensional span of $F_{,A}$, so a [Lagrange multiplier](../../../../../lagrange-multiplier.md) gives the [constraint reaction in hyperelastic stress](../../../../../constraint-reaction-in-hyperelastic-stress.md):

$$
\boxed{N_{\alpha i}=W_{,A_{i\alpha}}+qF_{,A_{i\alpha}}.}
$$

The sign of $q$ is a convention; the [virtual work](../../../../../virtual-work.md) identity determines no constitutive value for this reaction. Regularity matters: a singular equation describing the same constraint need not have a nonzero gradient.

For [incompressibility](../../../../../incompressible-flow.md), take $F=\det A-1$. Differentiating the expression using the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) gives

$$
\frac{\partial\det A}{\partial A_{i\alpha}}=\frac12\epsilon_{\alpha\beta\gamma}\epsilon_{ijk}A_{j\beta}A_{k\gamma}=(\det A)(A^{-1})_{\alpha i}.
$$

The middle expression is the corresponding entry of the [cofactor matrix](../../../../../cofactor-matrix.md). Since $\det A=1$, the [nominal stress](../../../../../nominal-stress-tensor.md) is therefore

$$
\boxed{N_{\alpha i}=W_{,A_{i\alpha}}+q(A^{-1})_{\alpha i}.}
$$

For the [neo-Hookean solid](../../../../../neo-hookean-solid.md), $W_{,A_{i\alpha}}=\mu A_{i\alpha}$, so in the material-first convention $N=\mu A^T+qA^{-1}$. The [identity matrix](../../../../../identity-matrix.md) satisfies the prescribed [dead loading](../../../../../dead-loading.md) with $q=T-\mu$, proving that the undeformed cube is always an equilibrium.

To obtain the [homogeneous tensile bifurcation of a neo-Hookean cube](../../../../../homogeneous-tensile-bifurcation-of-a-neo-hookean-cube.md), first seek $A=\operatorname{diag}(\lambda,\lambda,\lambda^{-2})$, with $\lambda>0$. This has unit [determinant](../../../../../determinant.md). The two distinct diagonal stress equations are $\mu\lambda+q/\lambda=T$ and $\mu\lambda^{-2}+q\lambda^2=T$. Eliminating $q$ gives

$$
(\lambda^3-1)\left[\mu(\lambda+\lambda^{-2})-T\right]=0.
$$

Thus the nontrivial branch is

$$
\boxed{t=\lambda+\lambda^{-2},\qquad \lambda^3-t\lambda^2+1=0,\qquad q=\mu/\lambda,\quad t=T/\mu.}
$$

The function $h(\lambda)=\lambda+\lambda^{-2}$ decreases on $(0,2^{1/3})$ and increases on $(2^{1/3},\infty)$, because $h'=1-2\lambda^{-3}$. Its minimum is $h(2^{1/3})=3/2^{2/3}$. Above this threshold there are two positive roots $\lambda_-<2^{1/3}<\lambda_+$. For $t\ne2$, neither root is one, and the three choices of the exceptional coordinate for each root give six distinct diagonal [deformation gradients](../../../../../deformation-gradient.md), in addition to $I$.

At $t=2$, however, $\lambda_-=1$ and the three smaller-root matrices coincide with $I$: it would be incorrect to count those as three new deformations. The requested existence of seven distinct homogeneous deformations nevertheless holds even at this value. For any unit vector $n$, put

$$
A(n)=\lambda_+ I+(\lambda_+^{-2}-\lambda_+)n n^T.
$$

Its positive [eigenvalues](../../../../../eigenvalue.md) are $\lambda_+,\lambda_+,\lambda_+^{-2}$, and its [determinant](../../../../../determinant.md) is one. Since $A(n)$ is an orthogonal conjugate of the diagonal solution, the same $q=\mu/\lambda_+$ gives $\mu A(n)^T+qA(n)^{-1}=T I$. Choose the six directions

$$
e_1,\ e_2,\ e_3,\ \frac{e_1+e_2}{\sqrt2},\ \frac{e_1+e_3}{\sqrt2},\ \frac{e_2+e_3}{\sqrt2}.
$$

Their [outer products](../../../../../outer-product.md) are distinct, and $\lambda_+>2^{1/3}>1$, so the six $A(n)$ are distinct from one another and from $I$. Constant [nominal stress](../../../../../nominal-stress-tensor.md) satisfies equilibrium and the prescribed surface [tractions](../../../../../traction.md). Hence **seven distinct homogeneous equilibria exist whenever $T/\mu>3/2^{2/3}$**. This is an existence count, not an exhaustive classification: rotated principal axes actually give a continuous family. The conventional seven axis-aligned positive-stretch branches coalesce to four distinct matrices at $T/\mu=2$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
