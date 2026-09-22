<h1 id="20f/solution">Solution</h1>

↑ **Parent:** [20F](../20f.md)

At a noncritical point a [holomorphic map](../../../../../holomorphic-map.md) has a local holomorphic inverse. Fibres of a nonconstant map between compact connected [Riemann surfaces](../../../../../riemann-surfaces.md) are finite: zeros are isolated and compactness precludes infinitely many. Around a nonbranch value $w$, choose disjoint inverse neighbourhoods of every point in its fibre. Compactness of the remaining source ensures a sufficiently small disc about $w$ has no additional preimages. Its preimage is therefore a disjoint union of open sets each mapped biholomorphically onto that disc. This proves a finite-sheeted unbranched [covering map](../../../../../covering-space.md) after removing the branch fibres.

Here the word “regular” must mean locally unbranched or evenly covered, rather than the stronger modern normal-cover condition. A general holomorphic map does not give a normal covering, and the example below itself shows the distinction.

Lift a loop based at $w$ uniquely from each point of $f^{-1}(w)$. Its endpoint defines a permutation; reversing the loop gives the inverse permutation, and concatenation gives composition. Homotopic loops yield the same endpoints. The [monodromy group of a covering](../../../../../monodromy-group-of-a-covering.md) consists of these permutations. Removing finitely many points from a connected surface leaves it path-connected. Any two points in the same fibre can therefore be joined upstairs; the projection of that path is a loop whose lift joins them. Thus **the monodromy action is transitive**.

For the rational map of degree three, differentiation gives

$$
f'(z)=\frac{z^2(3-z^2)}{(1-z^2)^2}.
$$

At $z=0$, the local degree is three, so a small loop around its value $0$ acts as a 3-cycle. At $z=\pm\sqrt3$, the local degree is two; their distinct branch values are $\mp3\sqrt3/2$, and a loop around either acts as a transposition. The poles $\pm1$ and the point at infinity are simple and unramified. A 3-cycle and a transposition generate the full symmetric group, so

$$
\boxed{H=S_3}.
$$

The corresponding degree-three connected cover is not normal: a normal cover would have a regular monodromy action, whereas $S_3$ on three letters has nontrivial point stabilizers. Thus the stronger interpretation of the printed terminology cannot hold.

## ↑ Ancestors (10)

1. [20F](../20f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
