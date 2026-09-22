<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Expanding the squared [Euclidean norm](../../../../../../euclidean-norm.md) gives

$$
x\in B(c,r)\quad\Longleftrightarrow\quad
\|x\|^2-2c\cdot x+\|c\|^2-r^2\leq0.
$$

In lifted coordinates $(z,t)=\Phi(x)=(x,\|x\|^2)$, this is the [closed half-space](../../../../../../closed-half-space.md)

$$
\boxed{t-2c\cdot z+\|c\|^2-r^2\leq0.}
$$

Every labelling of the original points obtainable by a [Euclidean ball](../../../../../../euclidean-ball.md) is therefore obtainable on their lifted images by an [affine linear classifier](../../../../../../affine-linear-classifier.md). The [feature map](../../../../../../feature-map.md) is [injective](../../../../../../injective-function.md), since it preserves the first $d$ coordinates; distinct original points remain distinct. If the original points are shattered, every labelling of the lifted points is realized, as required.

Here “linear separator” means a separator with an intercept, namely an [affine hyperplane](../../../../../../affine-hyperplane.md). If a convention demands strict separation on the finite sample, increase the constant term of the positive score $r^2-\|c\|^2+2c\cdot z-t$ by a sufficiently small positive amount. Positive points then have strictly positive score, and the finitely many negative scores remain strictly negative. A homogeneous separator can alternatively be obtained after adjoining one more constant coordinate; this distinction matters for dimension counts.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Computational learning theory](../../../../computational-learning-theory-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
