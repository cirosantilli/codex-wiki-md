<h1 id="question-4/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

Take $\boxed{f(x)=\sin x}$. This [function](../../../../../../function-split.md) is not a [polynomial](../../../../../../polynomial-split.md): it is nonzero and satisfies $f''=-f$, whereas a nonzero [polynomial](../../../../../../polynomial-split.md) cannot satisfy that identity, since taking two [derivatives](../../../../../../derivative.md) reduces its degree or gives zero.

By [Fourier orthogonality](../../../../../../fourier-orthogonality.md), the [Fourier sine series](../../../../../../fourier-sine-series.md) consists of the single term $\sin x$. Thus every truncation with $N\geq1$ is **exact**, including at the endpoints. In contrast, using the product-to-sum [trigonometric identity](../../../../../../trigonometric-identity.md) in its [Fourier cosine coefficients](../../../../../../fourier-cosine-coefficient.md) gives

$$
a_0=\frac4\pi,\qquad
a_{2m}=-\frac4{\pi(4m^2-1)}\quad(m\geq1),\qquad
a_{2m-1}=0.
$$

For example, $\int_0^\pi\sin x\cos(2mx)\,dx=-2/(4m^2-1)$ follows by integrating the two resulting [sine](../../../../../../sine.md) terms. Therefore the [Fourier cosine series](../../../../../../fourier-cosine-series.md) is

$$
\sin x=\frac2\pi-\frac4\pi\sum_{m=1}^\infty
\frac{\cos(2mx)}{4m^2-1}.
$$

Every finite cosine truncation omits infinitely many nonzero [Fourier coefficients](../../../../../../fourier-coefficient.md), so [Parseval's identity](../../../../../../parseval-identity.md) gives it strictly positive squared [L2 norm](../../../../../../l2-norm.md) error. The one-term sine representation has zero error in both the [L2 norm](../../../../../../l2-norm.md) and the [supremum norm](../../../../../../supremum-norm.md), proving the requested advantage.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [Question 4](../../question-4.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
