# Cross product equation with a fixed unit vector

↑ **Parent:** [Cross product](cross-product.md)

For a fixed [unit vector](unit-vector.md) $g\in\mathbb R^3$, the [linear map](linear-map.md) $r\mapsto r\times g$ has [kernel](kernel-of-a-linear-map-split.md) $\mathbb Rg$ and [image](image-of-a-function.md) the perpendicular [plane](plane.md) $g^\perp$. Thus $r\times g=f$ is solvable exactly when $f\cdot g=0$, and then its full solution set is

$$
r=g\times f+tg,\qquad t\in\mathbb R.
$$

For the proof, a [cross product](cross-product.md) with $g$ must be perpendicular to $g$. Conversely the [vector triple product identity](vector-triple-product.md) gives $g\times(r\times g)=r-(r\cdot g)g$, which determines the perpendicular [orthogonal projection](orthogonal-projection.md) of $r$. The remaining parallel component is arbitrary. Finally $(g\times f)\times g=f$ when $f\cdot g=0$, verifying sufficiency.

Geometrically, the solution set is a [straight line](straight-line.md) with direction $g$. Its nearest point to the origin is $g\times f$ and its distance from the origin is $|f|$. For a general nonzero fixed [vector](vector.md) $a$, the corresponding formula is $r=(a\times f)/|a|^2+ta$, again subject to $f\cdot a=0$.

## ↑ Ancestors (8)

1. [Cross product](cross-product.md)
2. [Vector](vector.md)
3. [Vector space](vector-space-split.md)
4. [Linear algebra](linear-algebra-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
