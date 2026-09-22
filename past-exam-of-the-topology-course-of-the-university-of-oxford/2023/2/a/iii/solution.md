<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here $D^2$ must denote the [closed disc](../../../../../closed-disc.md) $\{(x,y):x^2+y^2\leq1\}$, as its boundary points participate in the identification. For $r=\sqrt{x^2+y^2}$, define

$$
F(x,y)=\begin{cases}
\left(\dfrac{\sin(\pi r)}r x,\dfrac{\sin(\pi r)}r y,\cos(\pi r)\right),&r>0,\\
(0,0,1),&r=0.
\end{cases}
$$

The [Pythagorean trigonometric identity](../../../../../pythagorean-trigonometric-identity.md) gives $\|F(x,y)\|^2=1$, so the image lies in the [sphere](../../../../../sphere.md) $S^2$. Away from the origin the formula is [continuous](../../../../../continuous-function.md). At the origin, the first two coordinates have absolute value at most $|\sin(\pi r)|\to0$ and the third tends to $1$, proving [continuity](../../../../../continuous-function.md) there as well.

Every boundary point maps to $(0,0,-1)$, while the origin maps to $(0,0,1)$. For a point $(u,v,w)\in S^2$ with $-1<w<1$, there is a unique $r\in(0,1)$ with $\cos(\pi r)=w$, and its unique [preimage](../../../../../preimage.md) is

$$
(x,y)=\frac{r}{\sin(\pi r)}(u,v).
$$

This point has radius $r$, because $u^2+v^2=1-w^2=\sin^2(\pi r)$. The two poles have the [preimages](../../../../../preimage.md) already described. Thus $F$ is [surjective](../../../../../surjective-function.md) and its [fibers](../../../../../fiber-of-a-function.md) are exactly the prescribed [equivalence classes](../../../../../equivalence-class.md).

The [closed disc](../../../../../closed-disc.md) is [compact](../../../../../compact-space.md) by the [Heine-Borel theorem](../../../../../heine-borel-theorem.md), and $S^2$ is [Hausdorff](../../../../../hausdorff-space.md) with the [subspace topology](../../../../../subspace-topology.md) from [Euclidean space](../../../../../euclidean-norm.md). The preceding result gives the [homeomorphism](../../../../../homeomorphism.md)

$$
\boxed{D^2/{\sim}\ \cong\ S^2,\qquad [x,y]\longmapsto F(x,y)}.
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the topology course of the University of Oxford](../../../../split.md)
6. [Topology course of the University of Oxford](../../../../../topology-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
