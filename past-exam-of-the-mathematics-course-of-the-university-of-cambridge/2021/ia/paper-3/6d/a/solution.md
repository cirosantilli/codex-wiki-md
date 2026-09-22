<h1 id="6d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $x\in X$,

$$
\operatorname{Orb}(x)=\{gx:g\in G\},
\qquad
\operatorname{Stab}(x)=\{g\in G:gx=x\}.
$$

The stabilizer contains the identity; if $g,h$ fix $x$, then

$$
(gh^{-1})x=g(h^{-1}x)=gx=x,
$$

so it is a subgroup.

The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) states

$$
\boxed{|G|=|\operatorname{Orb}(x)|\,|\operatorname{Stab}(x)|}.
$$

Define

$$
G/\operatorname{Stab}(x)\longrightarrow\operatorname{Orb}(x),
\qquad
g\operatorname{Stab}(x)\longmapsto gx.
$$

The map is well defined and bijective: two elements give the same image exactly when they differ by an element of the stabilizer. Lagrange's theorem then proves the formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
