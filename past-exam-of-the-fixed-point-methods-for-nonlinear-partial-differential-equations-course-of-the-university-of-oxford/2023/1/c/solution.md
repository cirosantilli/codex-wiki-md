<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [retraction of a Hilbert ball onto its sphere](../../../../retraction-of-a-hilbert-ball-onto-its-sphere.md) exists. In the real [Hilbert space](../../../../hilbert-space-split.md) $\ell^2$, let $S(x_0,x_1,\ldots)=(0,x_0,x_1,\ldots)$ be the [unilateral shift operator](../../../../unilateral-shift-operator.md), and let $e_0=(1,0,\ldots)$. For $x$ in the [closed unit ball](../../../../closed-unit-ball.md) $\mathbb B$, define

$$
F(x)=\sqrt{1-\|x\|^2}\,e_0+Sx.
$$

The [orthogonality](../../../../orthogonal-vectors.md) of $e_0$ and $Sx$ gives $\|F(x)\|^2=1$. Thus $F$ is a [continuous map](../../../../continuous-map.md) into the [unit sphere](../../../../unit-sphere.md). It has no [fixed point](../../../../fixed-point.md): $F(x)=x$ would imply $x_{j+1}=x_j$ for every $j\geq0$. A constant [sequence](../../../../sequence.md) in $\ell^2$ must be zero, whereas $F(0)=e_0\ne0$.

Put $d=x-F(x)$, which is nonzero everywhere, and define

$$
\alpha(x)=\frac{2(1-\langle F(x),x\rangle)}{\|x-F(x)\|^2},
\qquad
\boxed{r(x)=F(x)+\alpha(x)(x-F(x)).}
$$

This is a [continuous map](../../../../continuous-map.md) on the whole [closed unit ball](../../../../closed-unit-ball.md), including zero. To check its range, observe that $\langle F(x),d\rangle=\langle F(x),x\rangle-1$, so

$$
\|F(x)+\alpha d\|^2
=1+2\alpha(\langle F(x),x\rangle-1)+\alpha^2\|d\|^2=1.
$$

If $\|x\|=1$, then $\|x-F(x)\|^2=2(1-\langle F(x),x\rangle)$, hence $\alpha(x)=1$ and $r(x)=x$. Therefore $r:\mathbb B\to\partial\mathbb B$ is a [retraction](../../../../retraction.md).

Geometrically this is the second intersection of the line from $F(x)$ through $x$ with the [unit sphere](../../../../unit-sphere.md). In fact

$$
\alpha(x)-1=\frac{1-\|x\|^2}{\|x-F(x)\|^2}\geq0.
$$

The construction illustrates why the finite-dimensional hypothesis in the [no-retraction theorem](../../../../no-retraction-theorem.md) matters. The [closed unit ball](../../../../closed-unit-ball.md) of $\ell^2$ is not a [compact set](../../../../compact-space.md) in the [norm topology](../../../../norm-topology.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
