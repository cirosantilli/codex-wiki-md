<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\mathcal V_4=i\Gamma^{(4)}$ denote the amputated Feynman vertex, with tree term $v_4=-i\lambda$. A one-loop [one-particle-irreducible Feynman diagram](../../../../one-particle-irreducible-feynman-diagram.md) has $V_3+2V_4=4$, allowing three families: two quartic vertices, two cubic vertices and one quartic vertex, or four cubic vertices. Define

$$
I_4(P,Q,R,S)=\int_kD(k)D(k+P)D(k+P+Q)D(k-S),\quad P+Q+R+S=0.
$$

Using $I_2,I_3$ from part c and writing $P_{ij}=p_i+p_j$, the complete one-loop result is

$$
\boxed{\begin{aligned}
\mathcal V_{4,\,1\text{-loop}}={}&\frac{v_4^2}{2}
\left[I_2(P_{12})+I_2(P_{13})+I_2(P_{14})\right]\\
&+v_3^2v_4\sum_{1\leq i<j\leq4}I_3(P_{ij},p_k,p_l)\\
&+v_3^4\left[I_4(p_1,p_2,p_3,p_4)+I_4(p_1,p_2,p_4,p_3)+I_4(p_1,p_3,p_2,p_4)\right].
\end{aligned}}
$$

In each term of the middle sum, $k,l$ are the two complementary indices. Their order does not change the integral after a loop-[momentum](../../../../momentum-split.md) redefinition.

The first line contains three bubble channels, one for each partition of the four labelled external legs into two pairs. Each has $S=2$ from interchanging its two identical internal lines. In the second line, the quartic vertex carries a chosen pair of external legs, giving $\binom42=6$ mixed triangles. Each has $S=1$. In the last line, cyclic orderings of four labelled external legs are identified under rotation and reversal, leaving $(4-1)!/2=3$ boxes, again with $S=1$ each. The figure in part b shows one representative of each family and its multiplicity. External-leg corrections and tadpoles connected by bridges are excluded because $\Gamma^{(4)}$ is a [one-particle-irreducible vertex](../../../../one-particle-irreducible-vertex.md). All integrals are left unevaluated, as appropriate here.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
