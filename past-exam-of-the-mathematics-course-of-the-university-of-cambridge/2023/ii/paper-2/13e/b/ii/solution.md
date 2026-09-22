<h1 id="13e/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At $z=1$, the branch value is the [complete elliptic integral of the first kind](../../../../../../../complete-elliptic-integral-of-the-first-kind.md)

$$
K=H(1).
$$

A contour that goes once around $1$ and then to $z$ applies the reflection about $K$, giving

$$
R_1(H(z))=2K-H(z).
$$

Similarly, the branch value at $-1$ is $-K$, so a loop around $-1$ acts as $R_{-1}(w)=-2K-w$. A contour that loops first around $-1$ and then around $1$ therefore gives

$$
R_1R_{-1}(H(z))=2K-(-2K-H(z))
=\boxed{4K+H(z)}.
$$

Finally approach the interval $(1,1/k)$ through the upper half-plane. There

$$
\sqrt{1-t^2}=-i\sqrt{t^2-1},
$$

so the branch value at $1/k$ is

$$
H(1/k)=K+i\int_1^{1/k}
\frac{dt}{\sqrt{(t^2-1)(1-k^2t^2)}}
=K+iL.
$$

It follows that a loop around $1/k$ acts as

$$
R_{1/k}(w)=2K+2iL-w.
$$

A contour that loops first around $1$ and then around $1/k$ consequently gives

$$
R_{1/k}R_1(H(z))
=2K+2iL-(2K-H(z))
=\boxed{2iL+H(z)}.
$$

Here $L=K'(k)$ is the [complementary complete elliptic integral of the first kind](../../../../../../../complementary-complete-elliptic-integral-of-the-first-kind.md). These contours exhibit all three requested values.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [13E](../../../13e.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
