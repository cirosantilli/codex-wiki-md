<h1 id="5e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [universal property of Cartesian products](../../../../../../universal-property-of-cartesian-products.md) constructs the desired map pointwise:

$$
\boxed{g(y)=(f_1(y),f_2(y)).}
$$

Its coordinate [projection maps](../../../../../../projection-map.md) are $f_1$ and $f_2$. Any other map with those [projection maps](../../../../../../projection-map.md) must have the same two coordinates at every $y$, and hence must equal $g$. This also covers $Y=\varnothing$.

For [joint injectivity of a pair of functions](../../../../../../joint-injectivity-of-a-pair-of-functions.md), equality $g(y)=g(y')$ means equality of both coordinate images. If either coordinate [function](../../../../../../function-split.md) is [injective](../../../../../../injective-function.md), it follows that $y=y'$, so $g$ is [injective](../../../../../../injective-function.md). The converse fails: take $Y=\{a,b,c\}$ and map these points to $(0,0),(0,1),(1,0)$ in $\{0,1\}^2$. The paired map is [injective](../../../../../../injective-function.md), but the first coordinate identifies $a,b$ and the second identifies $a,c$.

There is an empty-factor defect in the printed surjectivity implication. If both $X_1$ and $X_2$ are nonempty and $g$ is [surjective](../../../../../../surjective-function.md), every element of either factor can be completed to a pair and then lifted through $g$. Hence both $f_i$ are [surjective](../../../../../../surjective-function.md). If both factors are empty, existence of the $f_i$ forces $Y$ to be empty and both coordinate maps are again [surjective](../../../../../../surjective-function.md). But take

$$
Y=X_2=\varnothing,\qquad X_1=\{0\}.
$$

Then $g:\varnothing\to X_1\times X_2=\varnothing$ is [surjective](../../../../../../surjective-function.md), while $f_1:\varnothing\to\{0\}$ is not. **Without a nonempty-factor assumption, the printed implication is false.** This is exactly the exception found for the [projection maps](../../../../../../projection-map.md) in part (ii).

Even when both factors are nonempty, the reverse implication fails. For $Y=X_1=X_2=\{0,1\}$, let $f_1(y)=f_2(y)=y$. Both coordinate maps are [surjective](../../../../../../surjective-function.md), but $g(y)=(y,y)$ misses $(0,1)$ and $(1,0)$. Thus **coordinate surjectivity does not guarantee that every pair is attained**.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
