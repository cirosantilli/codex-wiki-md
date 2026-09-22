<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a diagram shape $I$, a [functor](../../../../../functor.md) $F:\mathcal C\to\mathcal D$ preserves [categorical limits](../../../../../categorical-limit.md) of shape $I$ if every limiting cone $(L,\ell_i)$ over every diagram $D:I\to\mathcal C$ is carried to a limiting cone $(FL,F\ell_i)$ over $FD$. It reflects [categorical limits](../../../../../categorical-limit.md) of that shape if a cone in $\mathcal C$ is limiting whenever its image cone is limiting. These properties concern cones which are given; reflection is not an assertion that every cone in the target lifts.

Suppose $F$ is a [full and faithful functor](../../../../../full-and-faithful-functor.md) and the image of $(L,\ell_i)$ is limiting. A cone $(X,x_i)$ in $\mathcal C$ becomes a cone in $\mathcal D$, so there is a unique $h:FX\to FL$ with $(F\ell_i)h=Fx_i$. Fullness writes $h=Fk$ for some $k:X\to L$. Faithfulness gives $\ell_i k=x_i$, and also ensures uniqueness: two such $k$ would have the same image, by uniqueness of $h$. Hence the original cone is limiting. This proves **every [full and faithful functor](../../../../../full-and-faithful-functor.md) reflects [categorical limits](../../../../../categorical-limit.md)**, the [limits reflected by full and faithful functors](../../../../../limits-reflected-by-full-and-faithful-functors.md) criterion, with no essential-surjectivity requirement.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
