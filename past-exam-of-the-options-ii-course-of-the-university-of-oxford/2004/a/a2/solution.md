<h1 id="a/a2/solution">Solution</h1>

↑ **Parent:** [A2](../a2.md)

The [permutation](../../../../permutation.md) inverse is $\rho_{g^{-1}}$: applying the two maps successively sends $\omega$ to $(\omega g)g^{-1}=\omega$. With the paper's right-action convention, [permutation](../../../../permutation.md) products also act on the right, and

$$
\omega(\rho_g\rho_h)=(\omega g)h=\omega(gh)=\omega\rho_{gh}.
$$

Thus $\boxed{\rho(gh)=\rho(g)\rho(h)}$. If function composition is written on the left instead, the same right action is represented by $g\mapsto\rho_{g^{-1}}$; keeping these conventions consistent avoids an artificial reversal. The kernel consists precisely of elements fixing every point, so

$$
\boxed{\ker\rho=\bigcap_{\omega\in\Omega}G_\omega.}
$$

The rotational tetrahedral [group](../../../../group-split.md) acts transitively on its four vertices. A [rotation](../../../../rotation-mathematics.md) fixing a vertex must preserve its opposite face and rotate its three vertices cyclically; its [stabilizer](../../../../stabilizer-subgroup.md) has order three. The [orbit-stabilizer theorem](../../../../orbit-stabilizer-theorem.md) gives $|G|=4\cdot3=12$. The rotations are the identity, two nontrivial rotations about each of the four vertex-to-opposite-face axes, and a half-turn about each of the three opposite-edge-midpoint axes. Therefore the counts by element order are

$$
\boxed{\begin{array}{c|rrrrrr}n&1&2&3&4&6&12\\\#&1&3&8&0&0&0\end{array}.}
$$

A [rotation](../../../../rotation-mathematics.md) fixing all vertices fixes three [linearly independent](../../../../linear-independence.md) vertex vectors and is the identity. The vertex [permutation](../../../../permutation.md) action is therefore faithful. The listed rotations induce the identity, 3-cycles and double transpositions, all even permutations. Its injective image has order 12, the full order of $A_4$. Hence $\boxed{G\cong A_4}$.

## ↑ Ancestors (12)

1. [A2](../a2.md)
2. [A](../../a.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
