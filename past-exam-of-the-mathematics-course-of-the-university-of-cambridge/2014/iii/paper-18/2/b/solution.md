<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [Category of sets](../../../../../../category-of-sets.md), an [epimorphism](../../../../../../epimorphism.md) is exactly a [surjective function](../../../../../../surjective-function.md). A [surjective function](../../../../../../surjective-function.md) is right-cancellable. If $q:X\to Y$ misses $y\in Y$, the constant-zero function and the function that is one at $y$ and zero elsewhere are distinct maps $Y\to\{0,1\}$ with equal composites with $q$.

If every $\alpha_A$ is surjective, equality $\beta\alpha=\gamma\alpha$ for [natural transformations](../../../../../../natural-transformation.md) $\beta,\gamma:G\Rightarrow H$ gives $\beta_A=\gamma_A$ for every $A$. Thus $\alpha$ is an [epimorphism](../../../../../../epimorphism.md) in the [functor category](../../../../../../functor-category.md).

For the converse, construct the pointwise amalgamated double

$$
H(A)=(G(A)\times\{0,1\})/\sim,
$$

where exactly the two copies of each element of $\operatorname{im}\alpha_A$ are identified; different elements of $G(A)$ remain different. Define $H(u)[y,i]=[G(u)y,i]$. Naturality of $\alpha$ implies that $G(u)$ takes its image into the image at the target, so this formula is well-defined and gives a [functor](../../../../../../functor.md). The maps $j_{i,A}(y)=[y,i]$ form [natural transformations](../../../../../../natural-transformation.md) $j_0,j_1:G\Rightarrow H$, with $j_0\alpha=j_1\alpha$.

If $\alpha$ is an [epimorphism](../../../../../../epimorphism.md), $j_0=j_1$. Since the two copies of an element outside $\operatorname{im}\alpha_A$ would be distinct, every element must lie in that image. Hence **$\alpha$ is epic if and only if every component is epic**. This proves the [pointwise epimorphism in a functor category](../../../../../../pointwise-epimorphism-in-a-functor-category.md) criterion directly, including the needed existence and naturality of the separating functor.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
