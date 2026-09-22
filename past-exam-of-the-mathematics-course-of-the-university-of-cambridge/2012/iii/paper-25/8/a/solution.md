<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take any [morphism](../../../../../../morphism.md) $h:A\to B$ and let $c:B\to C$ be its [categorical cokernel](../../../../../../cokernel-in-a-category.md). Let $i:I\to B$ be the [categorical kernel](../../../../../../kernel-in-a-category.md) of $c$. Since $ch=0$, kernel universality gives $e:A\to I$ with $h=ie$. The map $i$ is a [monomorphism](../../../../../../monomorphism.md). We must establish the [pseudo-epimorphism](../../../../../../pseudo-epimorphism.md) property of $e$, rather than merely name $I$ an image.

Suppose $t:I\to Z$ satisfies $te=0$. Let $k:K\to I$ be its [categorical kernel](../../../../../../kernel-in-a-category.md). Then $e=ka$ for some $a:A\to K$. The composite $ik$ is a [monomorphism](../../../../../../monomorphism.md), so the hypothesis that every [monomorphism](../../../../../../monomorphism.md) is normal provides a map $q:B\to D$ of which $ik$ is a [categorical kernel](../../../../../../kernel-in-a-category.md), up to its unique compatible isomorphism. Now $qh=qika=0$. The [categorical cokernel](../../../../../../cokernel-in-a-category.md) property of $c$ gives $q=\bar q c$, and therefore $qi=\bar q ci=0$.

Since $ik$ is the [categorical kernel](../../../../../../kernel-in-a-category.md) of $q$, the map $i$ factors through it: $i=ik\ell$ for some $\ell:I\to K$. Cancel the [monomorphism](../../../../../../monomorphism.md) $i$ to get $k\ell=1_I$. As $k$ is also a [monomorphism](../../../../../../monomorphism.md), $\ell k=1_K$, so $k$ is an [isomorphism](../../../../../../isomorphism.md). Finally $t=tk\ell=0$, proving that $e$ is a [pseudo-epimorphism](../../../../../../pseudo-epimorphism.md).

Thus

$$
\boxed{h=ie,\qquad i=\ker(\operatorname{coker}h),\qquad e\text{ pseudo-epic},\quad i\text{ monic}.}
$$

The [pseudo-epimorphism factorization through the kernel of a cokernel](../../../../../../pseudo-epimorphism-factorization-through-the-kernel-of-a-cokernel.md) proof uses a [pointed category](../../../../../../pointed-category.md), existence of [categorical kernels](../../../../../../kernel-in-a-category.md) and [categorical cokernels](../../../../../../cokernel-in-a-category.md), and normality of every monic map. It does not silently replace pseudo-epic cancellation against zero by the stronger [epimorphism](../../../../../../epimorphism.md) condition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [8](../../8.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
