<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $m_I:X^3\to X$ add the coordinates indexed by a nonempty subset $I$ of the three-element index set. The [Theorem of the Cube](../../../../../../theorem-of-the-cube.md) says that for every line bundle $\mathcal L$ on an abelian variety,

$$
m_{123}^*\mathcal L
\otimes m_{12}^*\mathcal L^\vee
\otimes m_{13}^*\mathcal L^\vee
\otimes m_{23}^*\mathcal L^\vee
\otimes m_1^*\mathcal L
\otimes m_2^*\mathcal L
\otimes m_3^*\mathcal L
$$

is trivial, up to the harmless constant line given by the fiber of $\mathcal L$ at the identity.

Pull this line bundle back along $(f,g,h):Y\to X^3$. Pullback commutes with tensor products and duals, and $m_I\circ(f,g,h)$ is the corresponding sum of morphisms. The resulting bundle is precisely $\mathcal M_{f,g,h}$, so it is trivial.

Take $Y=X$, $f=\operatorname{id}_X$, and let $g,h$ be the constant maps with values $x,y$. All pullbacks along constant maps are trivial line bundles. The formula for $\mathcal M_{f,g,h}$ then becomes

$$
T_{x+y}^*\mathcal L\otimes
(T_x^*\mathcal L)^\vee\otimes
(T_y^*\mathcal L)^\vee\otimes\mathcal L
\simeq\mathcal O_X,
$$

or equivalently

$$
T_{x+y}^*\mathcal L
\simeq T_x^*\mathcal L\otimes T_y^*\mathcal L\otimes\mathcal L^\vee.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
