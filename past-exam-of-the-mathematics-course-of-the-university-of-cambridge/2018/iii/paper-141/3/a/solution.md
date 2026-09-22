<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Label the four crossings $A,B,C,D$ in top, left-middle, right-middle, bottom order. Label the bounded regions $d$ (left), $e$ (right), $a$ (upper middle), $b$ (central bigon), $c$ (lower middle), and the unbounded region $o$. The drawing preserves the crossings and the orientation of the supplied [figure-eight knot](../../../../../../figure-eight-knot.md) diagram. Its overpassing strands are the outer-left/upper-right strand at $A$, the upper-left/lower-central strand at $B$, the upper-central/lower-right strand at $C$, and the lower-left/outer-right strand at $D$.

<a id="3/a/image-the-figure-eight-graph-regions-and-heegaard-state"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-141-dehn.png)

**[Figure 3](#3/a/image-the-figure-eight-graph-regions-and-heegaard-state). The figure-eight graph, regions and Heegaard state**.

Here is the [Dehn presentation Heegaard diagram](../../../../../../dehn-presentation-heegaard-diagram.md) specified by this drawing. Replace the underlying four-valent planar graph $G$ by a small three-dimensional regular neighborhood $N(G)$ and put $\Sigma=\partial N(G)$. Since $G$ has four vertices and eight edges, $\Sigma$ has [genus](../../../../../../genus-of-a-surface.md) $8-4+1=5$. On $\Sigma$, take the five $\alpha$ curves bordering the bounded faces, pushed slightly onto the boundary of $N(G)$. They bound a complete disk system in the complementary [handlebody](../../../../../../handlebody.md) $S^3\setminus\operatorname{int}N(G)$; their labels are $\alpha_d,\alpha_e,\alpha_a,\alpha_b,\alpha_c$.

The four $\beta$ curves bound the disks dual to the four short crossing tunnels in $N(G)\setminus\operatorname{int}\nu K_8$. Lift the crossing circles shown in red onto the upper and lower sheets of $\Sigma$, routing them along the corresponding face boundaries; the crossing's overpassing strand determines the lift. Orient the $\alpha$ disk normals and the $\beta$ curves so that their signed successive intersections with the $\alpha$ curves are

$$
\begin{array}{c|l}
\beta_A&a\ e^{-1}\ d^{-1}\\
\beta_B&a\ d^{-1}\ c\ b^{-1}\\
\beta_C&b\ a^{-1}\ e\ c^{-1}\\
\beta_D&c\ d^{-1}\ e^{-1}.
\end{array}
$$

At $A,D$ the missing fourth corner is the unbounded region $o$, whose generator is omitted. This sheet-lifting prescription, together with the projected graph, specifies the curves on the [Heegaard surface](../../../../../../heegaard-surface.md); the red circles alone are only their local projections.

To recover the [knot exterior](../../../../../../knot-exterior.md) from $\Sigma\times I$, attach five [two-handles](../../../../../../two-handle.md) along the $\alpha$ curves on one side and cap the resulting [sphere](../../../../../../sphere.md) with a [three-handle](../../../../../../three-handle.md). On the other side attach four [two-handles](../../../../../../two-handle.md) along the $\beta$ curves. Compressing that side leaves the boundary [torus](../../../../../../torus.md) of the [knot exterior](../../../../../../knot-exterior.md), which is retained. In particular, the counts are five $\alpha$ compressions and four $\beta$ compressions, rather than two complete genus-five disk systems.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 141](../../../paper-141-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
