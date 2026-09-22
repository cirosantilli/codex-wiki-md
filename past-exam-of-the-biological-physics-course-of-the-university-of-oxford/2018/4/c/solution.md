<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At the final [steady state](../../../../steady-state.md), the [ligands](../../../../ligand-biochemistry.md) control activity as well as the amount of each factor. Assuming active X exceeds its thresholds and the high Y level exceeds $K_{yz}$, the normalized output production rates are

$$
\boxed{\begin{array}{cc|cc}
S_x&S_y&\text{I1 output rate}&\text{I4 output rate}\\
0&0&0&0\\
0&1&0&0\\
1&0&\beta_{\rm high}&\beta_{\rm low}\\
1&1&\beta_{\rm low}&\beta_{\rm low}
\end{array}}
$$

For [I1 incoherent feed-forward loop](../../../../i1-incoherent-feed-forward-loop.md), active X makes Y abundant, but Y can repress Z only if its own activating [ligand](../../../../ligand-biochemistry.md) is present. Without $S_y$, Y is inactive and the output remains high. For [I4 incoherent feed-forward loop](../../../../i4-incoherent-feed-forward-loop.md), active X represses Y to below its threshold, so the output is low regardless of $S_y$. If X is inactive, the direct permissive arm is absent and both outputs are zero even when Y is active.

Thus [I1 incoherent feed-forward loop](../../../../i1-incoherent-feed-forward-loop.md) can retain two-input combinatorial control at [steady state](../../../../steady-state.md) as well as generate the transient in part (a). [I4 incoherent feed-forward loop](../../../../i4-incoherent-feed-forward-loop.md) loses steady-state sensitivity to $S_y$ once X has suppressed Y, under these particular assumptions. That gives a functional reason the first motif may be more useful in many regulatory contexts. It is not a proof of an evolutionary frequency: [promoter](../../../../promoter-genetics.md) implementation, thresholds, noise, costs and other functions also influence how common a motif is. The argument follows the supplied rate table, including its nonzero $\beta_{\rm low}$, rather than a generic Boolean AND truth table.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
