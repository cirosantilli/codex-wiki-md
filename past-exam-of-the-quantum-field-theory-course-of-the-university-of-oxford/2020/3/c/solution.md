<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Hold the external endpoints fixed and distinguish the three [Feynman diagrams](../../../../feynman-diagram.md) by their left-to-right order in the source. Write $S$ for the divisor and $w=1/S$ for the multiplying combinatorial weight. Each line below includes external [Feynman propagators](../../../../feynman-propagator.md); [amputation](../../../../amputation-of-external-propagators.md) leaves the same $w$.

**Left: two-point bubble.** There are two cubic [interaction vertices](../../../../interaction-vertex.md) and two parallel internal lines. Interchanging those lines preserves the labelled external endpoints, giving $S=2$. Direct [Wick contraction](../../../../wick-contraction.md) counting gives two assignments of the external endpoints to the vertices, $3^2$ choices of their field slots, and $2!$ pairings of the remaining slots:

$$
N_{\rm left}=2\cdot3^2\cdot2=36,\qquad
\boxed{w_{\rm left}=\frac{36}{2!(3!)^2}=\frac12.}
$$

With $\Delta=\Delta_F$ and external points $x_1,x_2$, its contribution is

$$
\frac{(-i\lambda)^2}{2}\int d^4y\,d^4z\,
\Delta(x_1-y)\Delta(y-z)^2\Delta(z-x_2).
$$

**Middle: three-point triangle.** The three labelled external endpoints fix their three adjacent cubic [interaction vertices](../../../../interaction-vertex.md), so no nonidentity [graph automorphism](../../../../graph-automorphism.md) remains. Counting gives $3!$ assignments of endpoints to vertices, $3^3$ choices of external field slots, and $2^3$ assignments of remaining slots to the two specified neighbours:

$$
N_{\rm middle}=3!\,3^3\,2^3=1296,\qquad
\boxed{w_{\rm middle}=\frac{1296}{3!(3!)^3}=1.}
$$

Its contribution is

$$
(-i\lambda)^3\int\prod_{r=1}^3 d^4y_r\,
\left[\prod_{r=1}^3\Delta(x_r-y_r)\right]
\Delta(y_1-y_2)\Delta(y_2-y_3)\Delta(y_3-y_1).
$$

The apparent rotational symmetry of an unlabelled triangle does not survive fixing three distinct external endpoints.

**Right: two-point graph with a chord.** There are four cubic [interaction vertices](../../../../interaction-vertex.md): the left and right attachment vertices $A,B$ and the two chord ends $C,D$. Its internal edges are $AC,AD,BC,BD,CD$. Reflection interchanges $C,D$, fixes $A,B$, and preserves the two external labels. This is the only nontrivial [graph automorphism](../../../../graph-automorphism.md), so $S=2$.

For a separate [Wick contraction](../../../../wick-contraction.md) count, choose the ordered external attachment vertices in $4\cdot3$ ways and their field slots in $3^2$ ways. Assign their two remaining slots to $C,D$ in $2^2$ ways. At each of $C,D$, choose the slot joining $A$ and then the slot joining $B$ in $3\cdot2$ ways; the last slots join each other. Thus

$$
N_{\rm right}=12\cdot9\cdot4\cdot6^2=15552,\qquad
\boxed{w_{\rm right}=\frac{15552}{4!(3!)^4}=\frac12.}
$$

Its contribution is

$$
\frac{(-i\lambda)^4}{2}\int d^4A\,d^4B\,d^4C\,d^4D\,
\Delta(x_1-A)\Delta(B-x_2)
\Delta(A-C)\Delta(A-D)\Delta(B-C)\Delta(B-D)\Delta(C-D).
$$

Consequently the three multiplying weights are $\boxed{(1/2,1,1/2)}$, or divisors $\boxed{(2,1,2)}$. The central chord is a single internal line joining two vertices, not a vertex at the centre of the circle.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
