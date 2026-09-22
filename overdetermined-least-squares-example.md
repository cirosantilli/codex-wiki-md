# Overdetermined least-squares example

↑ **Parent:** [Moore-Penrose inverse](moore-penrose-inverse.md)

Suppose three measurements constrain two unknowns:

$$
A=\begin{pmatrix}1&0\\0&1\\1&1\end{pmatrix},
\qquad
b=\begin{pmatrix}1\\2\\6\end{pmatrix}.
$$

The [linear system](system-of-linear-equations.md) asks for $x_1=1$, $x_2=2$, and $x_1+x_2=6$, which are incompatible. A [least-squares solution](least-squares-solution-of-a-linear-inverse-problem.md) makes a balanced compromise. The [matrix](matrix.md) has [full column rank](full-column-rank.md), so

$$
A^+=(A^TA)^{-1}A^T
=\frac13\begin{pmatrix}2&-1&1\\-1&2&1\end{pmatrix},
\qquad
\boxed{x_*=A^+b=(2,3)^T.}
$$

The fitted output and residual are

$$
Ax_*=(2,3,5)^T,
\qquad
r=b-Ax_*=(-1,-1,1)^T,
\qquad
A^Tr=0.
$$

Thus the two direct measurements are each overshot by one, and the measured sum is undershot by one. The residual has [Euclidean norm](euclidean-norm.md) $\sqrt3$ and is [orthogonal](orthogonal-vectors.md) to the [column space](column-space.md), the [plane](plane.md) $z=y_1+y_2$ in output coordinates $(y_1,y_2,z)$.

<a id="image-the-pseudoinverse-projects-inconsistent-data-onto-the-attainable-output-plane"></a>
![](pseudoinverse-least-squares-projection.png)

**[Figure 4](#image-the-pseudoinverse-projects-inconsistent-data-onto-the-attainable-output-plane). The pseudoinverse projects inconsistent data onto the attainable output plane**. For $b=(1,2,6)^T$, the closest attainable output is $Ax_*=(2,3,5)^T$. The segment between them is the residual $(-1,-1,1)^T$, perpendicular to the [column space](column-space.md). The drawing is an orthonormal two-dimensional slice of output space; the attainable [plane](plane.md) intersects this slice in the blue [straight line](straight-line.md).

For any perturbation $h\in\mathbb R^2$, the [orthogonality](orthogonal-vectors.md) of $r$ to $Ah$ gives

$$
\|b-A(x_*+h)\|_2^2=\|r\|_2^2+\|Ah\|_2^2
=3+\|Ah\|_2^2.
$$

Since the [kernel](kernel-of-a-linear-map-split.md) of $A$ is trivial, every nonzero $h$ increases the residual. The [least-squares solution](least-squares-solution-of-a-linear-inverse-problem.md) is unique in this example. The formula using $A^TA$ is convenient for these small exact calculations; an actual numerical computation can use a [QR decomposition](qr-decomposition.md) or [singular value decomposition](singular-value-decomposition.md) to avoid the extra conditioning cost of the [least-squares normal equations](normal-equations-for-linear-least-squares.md). For [full column rank](full-column-rank.md), the squared [singular values](singular-value.md) of $A$ are the [eigenvalues](eigenvalue.md) of $A^TA$, so its [condition number](condition-number.md) in the [Euclidean norm](euclidean-norm.md) is $\kappa_2(A^TA)=\kappa_2(A)^2$. [Strang, MIT 18.065 Lecture 9: four ways to solve least-squares problems](https://ocw.mit.edu/courses/18-065-matrix-methods-in-data-analysis-signal-processing-and-machine-learning-spring-2018/resources/lecture-9-four-ways-to-solve-least-squares-problems/)

## ↑ Ancestors (7)

1. [Moore-Penrose inverse](moore-penrose-inverse.md)
2. [Matrix inverse](matrix-inverse-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
