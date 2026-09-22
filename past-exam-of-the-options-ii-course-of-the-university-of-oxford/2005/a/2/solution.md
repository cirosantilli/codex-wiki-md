<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Count the pairs $(g,\omega)$ for which $g$ fixes $\omega$. Counting first by [group elements](../../../../group-element.md) gives $\sum_g\operatorname{Fix}(g)$, while counting first by points gives $\sum_\omega|\operatorname{Stab}(\omega)|$. On a [group orbit](../../../../orbit-group-theory.md) of size $r$, [orbit-stabilizer theorem](../../../../orbit-stabilizer-theorem.md) makes each [stabilizer](../../../../stabilizer-subgroup.md) have size $|G|/r$, so that [group orbit](../../../../orbit-group-theory.md) contributes $|G|$ to the second sum. Dividing by $|G|$ proves [Burnside's lemma](../../../../burnside-s-lemma.md):

$$
\boxed{\text{number of orbits}=\frac1{|G|}\sum_{g\in G}\operatorname{Fix}(g).}
$$

A [tetrahedron](../../../../tetrahedron.md) has four vertices. A [rotational symmetry](../../../../rotational-symmetry.md) is determined by the [image](../../../../image-of-a-function.md) of one vertex, with four possibilities, and the cyclic orientation of the three vertices around it, with three possibilities. All these choices are realizable, so its [rotational symmetry group of a tetrahedron](../../../../rotational-symmetry-group-of-a-tetrahedron.md) has order $12$. More explicitly, its elements are the identity, the two nontrivial [rotational symmetries](../../../../rotational-symmetry.md) around each of four vertex-to-opposite-face axes, and the half-turn about each of three axes through opposite edge midpoints. Thus there is **one element of order 1, eight of order 3, and three of order 2**. The induced [permutations](../../../../permutation.md) of vertices are the [even permutations](../../../../even-permutation.md), identifying the [group](../../../../group-split.md) with $A_4$.

Apply the [group action](../../../../group-action-split.md) to the [set](../../../../set-split.md) of [edge colourings](../../../../edge-coloring.md). A colouring is fixed by a [rotational symmetry](../../../../rotational-symmetry.md) precisely when its colour is constant on each cycle of the induced edge [permutation](../../../../permutation.md). The identity has six edge cycles and fixes $4^6$ colourings. A vertex-axis [rotational symmetry](../../../../rotational-symmetry.md) has two cycles of length three, fixing $4^2$. An opposite-edge half-turn fixes the two edges on its axis as [sets](../../../../set-split.md) and exchanges the other four in two pairs, giving four cycles and $4^4$ fixed colourings. Therefore

$$
\boxed{\frac{4^6+8\cdot4^2+3\cdot4^4}{12}=416.}
$$

Reflections are excluded because the equivalence in the source uses [rotational symmetries](../../../../rotational-symmetry.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
