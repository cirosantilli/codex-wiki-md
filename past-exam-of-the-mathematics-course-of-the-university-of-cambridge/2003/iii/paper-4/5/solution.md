<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For the [Johnson graph](../../../../../johnson-graph.md), an [edge](../../../../../edge-of-a-graph.md) exchanges one member of a $k$-set. Along one [edge](../../../../../edge-of-a-graph.md), intersection size with a fixed target can increase by at most one, so any [path in a graph](../../../../../path-in-a-graph.md) from $A$ to $B$ has length at least $k-|A\cap B|$. Replacing the elements of $A\setminus B$ successively by elements of $B\setminus A$ gives a [path in a graph](../../../../../path-in-a-graph.md) attaining that bound. Hence the [distance in a Johnson graph](../../../../../distance-in-a-johnson-graph.md) is

$$
\boxed{d(A,B)=k-|A\cap B|.}
$$

If two ordered pairs have the same distance $r$, their four regions (intersection, first-only, second-only and outside the union) have sizes $k-r,r,r,n-k-r$. Choose bijections between corresponding regions. Their union is a ground-set [permutation](../../../../../permutation.md) sending the ordered pair to the other pair and preserving [graph adjacency](../../../../../graph-adjacency.md). **The [symmetric group](../../../../../symmetric-group.md) is [distance-transitive](../../../../../distance-transitive-graph.md).** For $n\ge2k$ the [graph diameter](../../../../../graph-diameter.md) is $k$.

For the [Grassmann graph](../../../../../grassmann-graph.md), a codimension-one exchange changes intersection [dimension](../../../../../dimension-vector-space.md) with a fixed target by at most one. More explicitly, if $A,A'$ are adjacent, their common $(k-1)$-space shows $\dim(A'\cap B)\ge\dim(A\cap B)-1$, and exchanging the two gives the reverse bound. Thus distance is at least $r=k-\dim(A\cap B)$.

Choose a [basis](../../../../../basis.md) $c_1,\ldots,c_{k-r}$ of $I=A\cap B$, complement it in $A$ by $a_1,\ldots,a_r$, and in $B$ by $b_1,\ldots,b_r$. These combined vectors are independent because $A\cap B=I$. The spaces

$$
A_j=I+\langle b_1,\ldots,b_j,a_{j+1},\ldots,a_r\rangle,\qquad 0\le j\le r,
$$

form a [path in a graph](../../../../../path-in-a-graph.md) of length $r$. Consequently

$$
\boxed{d(A,B)=k-\dim(A\cap B).}
$$

Equal-distance ordered pairs have the same [dimensions](../../../../../dimension-vector-space.md) in this adapted [basis](../../../../../basis.md) construction. Extend both combined [bases](../../../../../basis.md) to [bases](../../../../../basis.md) of $V$, and match them by a [invertible linear map](../../../../../invertible-linear-map.md). It maps the first ordered pair to the second and preserves [dimensions](../../../../../dimension-vector-space.md) of intersections, hence [graph adjacency](../../../../../graph-adjacency.md). **$GL_n(F)$ is [distance-transitive](../../../../../distance-transitive-graph.md)**, over an arbitrary [field](../../../../../field.md), with [graph diameter](../../../../../graph-diameter.md) $k$ under $n\ge2k$.

For the [symplectic dual polar graph](../../../../../symplectic-dual-polar-graph.md), [vertices](../../../../../vertex-graph-theory.md) are Lagrangian $m$-spaces. Let $I=A\cap B$ have [dimension](../../../../../dimension-vector-space.md) $m-r$. The quotient $I^\perp/I$ is a nonsingular [symplectic vector space](../../../../../symplectic-vector-space.md) of [dimension](../../../../../dimension-vector-space.md) $2r$, and $A/I,B/I$ are complementary [Lagrangian subspaces](../../../../../lagrangian-subspace.md). Their mutual pairing is nonsingular: a vector orthogonal to both lies in $(A+B)^\perp=I$, so vanishes in the quotient. Choose dual [bases](../../../../../basis.md) $e_1,\ldots,e_r$ in $A/I$ and $f_1,\ldots,f_r$ in $B/I$, and lift them into $A,B$. Their span is a nonsingular symplectic $2r$-space. Complete it by a [basis](../../../../../basis.md) $e_{r+1},\ldots,e_m$ of $I$ and suitable dual partners. This gives the pair normal form

$$
A=\langle e_1,\ldots,e_m\rangle,\qquad
B=\langle f_1,\ldots,f_r,e_{r+1},\ldots,e_m\rangle.
$$

The spaces $A_j=\langle f_1,\ldots,f_j,e_{j+1},\ldots,e_m\rangle$ remain [totally isotropic subspace](../../../../../totally-isotropic-subspace.md): a present $f_i$ pairs only with the absent $e_i$. They give an adjacent-step [path in a graph](../../../../../path-in-a-graph.md) of length $r$. The previous intersection-dimension lower bound still applies, proving

$$
\boxed{d(A,B)=m-\dim(A\cap B).}
$$

For two ordered pairs at the same distance, match their adapted [symplectic bases](../../../../../symplectic-basis.md). The resulting map preserves the [alternating bilinear form](../../../../../alternating-bilinear-form.md) and sends the pairs to each other, so lies in $Sp_{2m}(F)$. Equivalently, construct the [isometry of a space with a form](../../../../../isometry-of-a-space-with-a-form.md) on $A+B$ from the displayed normal form and extend it by [Witt's lemma](../../../../../witt-s-theorem.md). **The action of the [symplectic group over a field](../../../../../symplectic-group-over-a-field.md) is [distance-transitive](../../../../../distance-transitive-graph.md)**, over every [field](../../../../../field.md), and its graph has [graph diameter](../../../../../graph-diameter.md) $m$. The zero-dimensional boundary cases give a single [vertex](../../../../../vertex-graph-theory.md) and trivial transitivity.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
