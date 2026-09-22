<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Gauss-Seidel method](../../../../gauss-seidel-method.md) updates coordinates successively using the newest available entries:

$$
\boxed{x_i^{(k+1)}=\frac{b_i-\sum_{j<i}a_{ij}x_j^{(k+1)}-\sum_{j>i}a_{ij}x_j^{(k)}}{a_{ii}}.}
$$

It is well-defined for every initial vector exactly when every $a_{ii}\ne0$, equivalently when the triangular matrix $D+L$ is invertible. Nonsingularity of $A$ alone does not ensure this. The matrix form is

$$
\boxed{(D+L)x^{(k+1)}=b-Ux^{(k)}.}
$$

If the iterates converge to $z$, passing to the limit gives $(D+L)z=b-Uz$, hence $Az=b$. Nonsingularity identifies $z$ as the unique solution $x$.

Now assume $A$ is a [symmetric positive-definite matrix](../../../../symmetric-positive-definite-matrix.md). Testing with the coordinate vector gives $a_{ii}=e_i^TAe_i>0$, so $D$ is positive definite. The form $\langle v,w\rangle_A=v^TAw$ is an [inner product](../../../../inner-product-split.md): bilinearity and symmetry are immediate and positivity is the hypothesis. Its [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) gives

$$
\|v+w\|_A^2\leq\|v\|_A^2+2\|v\|_A\|w\|_A+\|w\|_A^2,
$$

proving the triangle inequality; definiteness and absolute homogeneity are immediate. Thus $\|v\|_A=\sqrt{v^TAv}$ is the [energy norm](../../../../energy-norm.md).

Subtract the iteration from the exact equation to obtain $(D+L)e_{k+1}=-L^Te_k$. Hence

$$
Ae_k=(D+L)(e_k-e_{k+1}).
$$

Using the preceding iteration also gives $(D+L)e_k=-L^Te_{k-1}$ and therefore $Ae_k=L^T(e_k-e_{k-1})$ for $k\geq1$, as required.

Put $d=e_k-e_{k+1}$. Expanding the two quadratic forms and using the first identity gives the exact [Gauss-Seidel energy decrease identity](../../../../gauss-seidel-energy-decrease-identity.md):

$$
\boxed{\|e_k\|_A^2-\|e_{k+1}\|_A^2=2d^TAe_k-d^TAd=d^TDd.}
$$

Here $2d^TLd=d^T(L+L^T)d$. If $d=0$, then $Ae_k=0$, so $e_k=0$. Otherwise $d^TDd>0$. Thus $\boxed{\|e_k\|_A>\|e_{k+1}\|_A}$ unless the exact solution has already been reached.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
