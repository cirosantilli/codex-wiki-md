<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use uniform [expectations](../../../../../../expected-value.md) on the nonempty sets $X,Y$. Define the rectangle fourth moment and the normalized [cut norm](../../../../../../cut-norm.md) by

$$
Q(f)=\mathbb E_{x,x',y,y'}f(x,y)f(x,y')f(x',y)f(x',y'),\qquad D(f)=\max_{A\subseteq X,\,B\subseteq Y}|\mathbb E_{x,y}f(x,y)1_A(x)1_B(y)|.
$$

The first quantity is nonnegative, since

$$
Q(f)=\mathbb E_{x,x'}\left(\mathbb E_y f(x,y)f(x',y)\right)^2;
$$

its fourth root is the [box norm](../../../../../../box-norm.md). To bound the [cut norm](../../../../../../cut-norm.md), fix $A,B$ and put $T=\mathbb E_{x,y}f(x,y)1_A(x)1_B(y)$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in $y$ gives

$$
|T|^2\leq\mathbb E_y\left|\mathbb E_x1_A(x)f(x,y)\right|^2=\mathbb E_{x,x'}1_A(x)1_A(x')\mathbb E_y f(x,y)f(x',y).
$$

A second [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md), now in $(x,x')$, yields

$$
|T|^4\leq\mathbb E_{x,x'}\left(\mathbb E_y f(x,y)f(x',y)\right)^2=Q(f),
$$

because the squared mean of $1_A(x)1_A(x')$ is at most one. Taking the maximum over rectangles gives the first direction of [cut norm and rectangle fourth-moment equivalence](../../../../../../cut-norm-and-rectangle-fourth-moment-equivalence.md):

$$
\boxed{D(f)\leq Q(f)^{1/4},\qquad c_2=c_1^{1/4}\text{ is admissible}.}
$$

The normalization divides the rectangle sum by $mn$ and the fourth-moment sum by $m^2n^2$, so the bound is independent of the two set sizes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
