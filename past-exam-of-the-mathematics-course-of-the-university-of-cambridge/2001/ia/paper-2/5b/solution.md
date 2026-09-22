<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

For the homogeneous [linear recurrence relation](../../../../../linear-recurrence-relation.md), substitute $y_k=r^k$. Its [characteristic equation of a linear recurrence](../../../../../characteristic-equation-of-a-linear-recurrence.md) is $r^2-r+1=0$, with roots $e^{i\pi/3}$ and $e^{-i\pi/3}$. Taking real [linear combinations](../../../../../linear-combination.md) gives

$$
\boxed{y_k=A\cos(k\pi/3)+B\sin(k\pi/3).}
$$

These two real sequences are [linearly independent](../../../../../linear-independence.md): their values at $k=1,2$ form a matrix with [determinant](../../../../../determinant.md) $\sqrt3/2\ne0$. Thus their two constants account uniquely for arbitrary first two values.

Let $P_k=\sum_{n=1}^k a_n/(k-n+1)$ and reindex as $P_k=\sum_{j=1}^k a_{k-j+1}/j$. In $P_{k+2}-P_{k+1}+P_k$, each term with $1\le j\le k$ has coefficient

$$
a_{k-j+3}-a_{k-j+2}+a_{k-j+1}=0.
$$

The term $j=k+1$ is $(a_2-a_1)/(k+1)=0$, and the remaining term is $a_1/(k+2)=1/(k+2)$. This explicitly proves that $P_k$ is the required particular solution, a [discrete Green convolution for the period-six recurrence](../../../../../discrete-green-convolution-for-the-period-six-recurrence.md).

The unit-response coefficients have the homogeneous form just found. The values $a_1=a_2=1$ give zero cosine coefficient and sine coefficient $2/\sqrt3$, so

$$
a_n=\frac2{\sqrt3}\sin(n\pi/3).
$$

Subtracting this particular solution from any other solution leaves a homogeneous recurrence. Thus the complete answer is

$$
\boxed{y_k=A\cos(k\pi/3)+B\sin(k\pi/3)
+\frac2{\sqrt3}\sum_{n=1}^k\frac{\sin(n\pi/3)}{k-n+1},\qquad k\ge1.}
$$

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
