<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

We first prove that [fixed-point-free sphere maps are homotopic to the antipodal map](../../../../../../fixed-point-free-sphere-maps-are-homotopic-to-the-antipodal-map.md). If $f:S^d\to S^d$ has no fixed point, define

$$
H_t(x)=\frac{(1-t)f(x)-tx}{\|(1-t)f(x)-tx\|},
\qquad 0\leq t\leq1.
$$

The denominator could vanish only if $f(x)$ is a positive multiple of $x$. Both are unit vectors, so this would require $f(x)=x$ and $t=1/2$, excluded by the hypothesis. Thus $H$ is a [continuous](../../../../../../continuous-function.md) [homotopy](../../../../../../homotopy.md) from $f$ to $x\mapsto-x$.

On $S^{2r}$, with $r\geq1$, the antipodal map has degree $(-1)^{2r+1}=-1$, since it is the boundary map of the ambient linear transformation $-I$ on $\mathbb R^{2r+1}$. Homotopy invariance therefore gives degree minus one for every fixed-point-free action map. The degree of each [homeomorphism](../../../../../../homeomorphism.md) is $\pm1$, and functoriality makes degree a [group homomorphism](../../../../../../group-homomorphism.md)

$$
G\longrightarrow\{1,-1\}.
$$

Every nonidentity element in a free action has degree minus one, so this homomorphism has trivial kernel. Hence

$$
\boxed{|G|\leq2.}
$$

For $S^0$ the same bound follows immediately from its two points. This proves that [free actions on even-dimensional spheres have order at most two](../../../../../../free-actions-on-even-dimensional-spheres-have-order-at-most-two.md), without an Euler-characteristic argument requiring a cell structure on the quotient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
