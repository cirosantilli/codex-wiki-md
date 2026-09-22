<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Lateral artifacts of a subdivision surface](../../../../../lateral-artifacts-of-a-subdivision-surface.md) are spurious changes along an intended straight extrusion. For example, if every row of a [control net](../../../../../control-net.md) is the same profile translated along a straight direction, a refinement rule should not create periodic ripples along that direction. This is distinct from changing or smoothing the transverse profile itself.

Use triangular-lattice coordinates $(i,j)$ with basis vectors $e_1=(1,0)$ and $e_2=(1/2,\sqrt3/2)$. The displayed mask is supported on $|i|,|j|,|i+j|\le3$, with the central entry at $(0,0)$. Write its coefficients as $a_{i,j}$, including their division by12. For data constant along horizontal rows, $p_{i,j}=q_j$, ternary refinement gives

$$
p'_{I,J}=\sum_kq_k\sum_{i\equiv I\ (\mathrm{mod}\ 3)}a_{i,J-3k}.
$$

Thus the three residue sums in every mask row must agree if arbitrary row-constant data are to remain row-constant. Equal whole-stencil sums alone only reproduce constants and do not guarantee straight-extrusion preservation.

For the original row $j=1$, the numerator coefficients at $i=-3,-2,-1,0,1,2$ are $2,4,5,5,4,2$. Their three residue sums are $7,8,7$, which do not agree. For $j=2$ the sums are $5,5,4$. In particular input $q_j=\delta_{j0}$ yields heights $7/12,8/12,7/12$ along the refined row $J=1$. **The original mask has lateral artifacts**, since it introduces a three-phase ripple into a straight extrusion. The residue-sum criterion is also the usual symbol-factor test: the mask polynomial must contain the ternary averaging factor in the extrusion direction. The original does not. This connects the concrete calculation with the directional artifact analysis in [Deriving Box-Spline Subdivision Schemes](https://neildodgson.com/pubs/arrows.pdf), while the coefficients and correction here are computed directly from the exam PDF.

A symmetric correction with the same denominator and support is to **replace the six nearest-center coefficients5 by6, and the six second-ring corner coefficients3 by2**. Leave every other coefficient unchanged, including the central6. The added and subtracted weights balance. For a complete computational specification, the corrected numerator rows are

$$
\begin{array}{c|r|l}
j&\text{first }i&\text{coefficients at successive }i\\\hline
3&-3&(1,2,2,1)\\
2&-3&(2,2,4,2,2)\\
1&-3&(2,4,6,6,4,2)\\
0&-3&(1,2,6,6,6,2,1)\\
-1&-2&(2,4,6,6,4,2)\\
-2&-1&(2,2,4,2,2)\\
-3&0&(1,2,2,1).
\end{array}
$$

Every entry in this new table is divided by12. The corresponding horizontal residue sums, before division, are

$$
\begin{array}{c|ccc}
j& i\equiv0&i\equiv1&i\equiv2\\\hline
-3&2&2&2\\
-2&4&4&4\\
-1&8&8&8\\
0&8&8&8\\
1&8&8&8\\
2&4&4&4\\
3&2&2&2.
\end{array}
$$

Consequently the corrected rule has [extrusion invariance of a ternary triangular scheme](../../../../../extrusion-invariance-of-a-ternary-triangular-scheme.md). Sixfold symmetry gives the same residue-sum property in the other two lattice-edge directions. Every two-dimensional residue class still sums to12 before normalization, so each refinement stencil sums to one. The weights are nonnegative. Symmetry about the stencil's refined parameter location also reproduces affine coordinates: the class first moments vanish, so an initial straight geometric translation direction remains straight.

The associated univariate boundary [subdivision mask](../../../../../subdivision-mask.md) is the common sum in each transverse row, rather than the central row of the bivariate mask. Centering it at indices $-3,\ldots,3$ gives

$$
\boxed{b=\frac16[1,2,4,4,4,2,1].}
$$

Its ternary stencils can be written explicitly as

$$
\boxed{\begin{aligned}
q'_{3k}&=\tfrac16q_{k-1}+\tfrac23q_k+\tfrac16q_{k+1},\\
q'_{3k+1}&=\tfrac23q_k+\tfrac13q_{k+1},\\
q'_{3k+2}&=\tfrac13q_k+\tfrac23q_{k+1}.
\end{aligned}}
$$

Each stencil sums to one and has the correct affine parameter moment. Applying this rule to a boundary profile agrees with the bivariate rule on a straight extrusion. Endpoint or corner rules must still be chosen for a finite open boundary. The artifact-free conclusion established here concerns the three lattice-edge extrusion directions; it does not promise exact extrusion preservation for every arbitrary off-grid direction. The directional limitation is intrinsic to the mask test, not a reason to substitute the central mask row as a boundary rule.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
