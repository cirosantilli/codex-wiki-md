<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For based maps $\alpha:S^p\to Y$ and $\beta:S^q\to Y$, use the standard cell decomposition

$$
S^p\times S^q=(S^p\vee S^q)\cup_w D^{p+q}.
$$

The attaching map $w:S^{p+q-1}\to S^p\vee S^q$ is obtained from the boundary of $D^p\times D^q$, collapsing the appropriate coordinate boundaries. The geometric [Whitehead product](../../../../../../whitehead-product.md) is the [homotopy class](../../../../../../homotopy-class.md)

$$
[\alpha,\beta]_W=[(\alpha\vee\beta)\circ w]
\in\pi_{p+q-1}(Y).
$$

Orient the product cell consistently with the ordinary product orientation. Its class depends only on the two [homotopy](../../../../../../homotopy.md) classes, and it is natural: $f_*[\alpha,\beta]_W=[f_*\alpha,f_*\beta]_W$.

For $p,q\ge2$ it is additive in both variables:

$$
[\alpha+\alpha',\beta]_W=[\alpha,\beta]_W+[\alpha',\beta]_W,
\qquad[\alpha,\beta+\beta']_W=[\alpha,\beta]_W+[\alpha,\beta']_W.
$$

Thus it is bilinear over $\mathbb Z$, and after [rationalization of a topological space](../../../../../../rationalization-of-a-topological-space.md) over $\mathbb Q$. In the geometric convention its symmetry is

$$
[\alpha,\beta]_W=(-1)^{pq}[\beta,\alpha]_W.
$$

For a genuine graded Lie convention, put a class in $\pi_pY$ in shifted degree $p-1$ and set $\{\alpha,\beta\}=(-1)^p[\alpha,\beta]_W$. Equivalently transport the [Samelson product](../../../../../../samelson-product.md) through [reduced suspension](../../../../../../reduced-suspension.md) and [loop space](../../../../../../loop-space.md) adjunction. Writing $|\alpha|=p-1$, this bracket has degree zero, satisfies

$$
\{\alpha,\beta\}=-(-1)^{|\alpha||\beta|}\{\beta,\alpha\},
$$

and has the graded [Jacobi identity](../../../../../../jacobi-identity.md)

$$
(-1)^{|\alpha||\gamma|}\{\alpha,\{\beta,\gamma\}\}
+(-1)^{|\beta||\alpha|}\{\beta,\{\gamma,\alpha\}\}
+(-1)^{|\gamma||\beta|}\{\gamma,\{\alpha,\beta\}\}=0.
$$

These are two equivalent sign presentations of the same [Whitehead product](../../../../../../whitehead-product.md). In particular the square of an odd-dimensional geometric class is two-torsion, whereas an even-dimensional sphere class can have a nonzero rational square. [Reduced suspension](../../../../../../reduced-suspension.md) kills [Whitehead products](../../../../../../whitehead-product.md), since the suspended attaching map of the product cell is null-homotopic. No proofs of these remaining algebraic properties are needed here.

Bilinearity has a specific fundamental-group exception. If both inputs lie in $\pi_1Y$, the attaching loop of the torus is the [commutator](../../../../../../commutator.md), so the operation is $ghg^{-1}h^{-1}$, with the possible inverse corresponding to reversal of its boundary orientation. This is not a homomorphism in either input in a general nonabelian group.

If one input is $g\in\pi_1Y$ and the other is $\beta\in\pi_qY$, $q\ge2$, the product records the action difference $g\cdot\beta-\beta$, up to the fixed overall boundary sign. Choose the action convention matching that boundary orientation and write $\delta_g\beta=g\cdot\beta-\beta$. Then

$$
\delta_g(\beta+\gamma)=\delta_g\beta+\delta_g\gamma,
\qquad
\delta_{gh}\beta=\delta_g\beta+g\cdot(\delta_h\beta).
$$

The second formula is a crossed-additivity law, not ordinary additivity in $g$. It follows by expanding $gh\cdot\beta-\beta=g\cdot(h\cdot\beta-\beta)+(g\cdot\beta-\beta)$. Consequently the higher-homotopy variable remains additive, while the fundamental-group variable is generally not. If the action is trivial the mixed product is zero. This explains exactly where the usual bilinearity statement fails.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
