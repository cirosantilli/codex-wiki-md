<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Lefschetz fixed-point theorem](../../../../../lefschetz-fixed-point-theorem.md) says that a continuous self-map $f$ of a compact triangulable space has a fixed point whenever its [Lefschetz number](../../../../../lefschetz-number.md)

$$
L(f)=\sum_i(-1)^i\operatorname{tr}(f_*:H_i(X;\mathbb Q)\to H_i(X;\mathbb Q))
$$

is nonzero. In the smooth nondegenerate case, the [Lefschetz-Hopf fixed-point theorem](../../../../../lefschetz-hopf-fixed-point-theorem.md) expresses this number as the sum of the local fixed-point indices.

Identify $H_1(\mathbb R^2/\mathbb Z^2;\mathbb Z)$ with $\mathbb Z^2$ by sending $v\in\mathbb Z^2$ to the class of the loop $t\mapsto tv\bmod\mathbb Z^2$. The image of this loop under $f$ lifts from $0$ to the path $t\mapsto\widetilde f(tv)$, whose endpoint is $\widetilde f(v)=A(v)$. Its homology class is therefore $A(v)$. Thus $A=f_*$ under this identification, and in particular $A$ is a homomorphism represented by an integer matrix.

The expansion inequality implies, after taking a derivative, that

$$
|D\widetilde f_x(v)|\geq\mu|v|
$$

for every tangent vector. The supplied linear-algebra fact shows that every eigenvalue of $D\widetilde f_x$ has modulus at least $\mu>1$, so $1$ is not an eigenvalue. Every fixed point of $f$ is consequently nondegenerate and contributes local index $+1$ or $-1$.

On the [torus](../../../../../torus.md), the induced maps on $H_0,H_1,H_2$ have traces $1,\operatorname{tr}A,\det A$. Hence

$$
L(f)=1-\operatorname{tr}A+\det A=\det(I-A).
$$

The original expansion inequality applied to lattice vectors gives $|Av|\geq\mu|v|$ for $v\in\mathbb Z^2$, and homogeneity and density extend it to all $v\in\mathbb R^2$. If $\lambda_1,\lambda_2$ are the possibly complex eigenvalues of $A$, then $|\lambda_j|\geq\mu$, so

$$
|L(f)|=|1-\lambda_1|\,|1-\lambda_2|
\geq(\mu-1)^2.
$$

Since every fixed point contributes an index of absolute value one, the Lefschetz-Hopf formula gives

$$
\boxed{\#\operatorname{Fix}(f)\geq|L(f)|\geq(\mu-1)^2.}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
