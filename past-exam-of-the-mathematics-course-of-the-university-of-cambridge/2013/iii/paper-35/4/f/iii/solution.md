<h1 id="4/f/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

This produces a **[split-plot design](../../../../../../../split-plot-design.md)**: assign spray to whole orchards, with six sprayed and six unsprayed, then independently randomize ten trees to each pruning method inside every orchard. Orchards remain [experimental units](../../../../../../../experimental-unit.md) for spray; individual trees become [experimental units](../../../../../../../experimental-unit.md) for pruning. Pruning contrasts and the spray-by-pruning [interaction term](../../../../../../../interaction-term.md) now lie in the [within-block ANOVA stratum](../../../../../../../within-block-anova-stratum.md), while spray is tested between orchards.

The between-orchard [ANOVA stratum](../../../../../../../anova-stratum.md) has eleven [statistical degrees of freedom](../../../../../../../statistical-degrees-of-freedom.md), split into one for spray and ten for error. The within-orchard [ANOVA stratum](../../../../../../../anova-stratum.md) has 348, split into two for pruning, two for the [interaction term](../../../../../../../interaction-term.md) and 344 for error. This pooling of within-orchard error is appropriate under the stated [compound-symmetry covariance](../../../../../../../compound-symmetry-covariance.md) model; additional orchard-specific pruning variation would need its own [variance component](../../../../../../../variance-component.md) rather than this simplified error model.

The shared orchard effect cancels in a pruning difference within an orchard. Its [variance](../../../../../../../variance-split.md) is $2a/10$, so averaging across twelve orchards gives

$$
\boxed{\widehat{\operatorname{Var}}(\text{pruning difference})=\frac{2\cdot180}{10\cdot12}=3.}
$$

The spray contrast still compares means of six orchards per group, each based on 30 trees, so its estimated [variance](../../../../../../../variance-split.md) remains $8/3$. For a difference of pruning differences between the two spray groups, each group's pruning difference has estimated [variance](../../../../../../../variance-split.md) $2\cdot180/(10\cdot6)=6$, and the resulting [interaction contrast](../../../../../../../interaction-contrast.md) has estimated [variance](../../../../../../../variance-split.md) $12$, compared with $16$ in the original allocation.

**Splitting pruning within orchards improves pruning and interaction precision without extra trees, and gives spray a less sparse error estimate; it does not reduce the spray contrast's [variance](../../../../../../../variance-split.md).** This option requires tree-level pruning to be practical without interference between neighboring trees. The numerical gains, like those in the other options, assume the current [variance components](../../../../../../../variance-component.md) remain applicable next year.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [F](../../f.md)
3. [4](../../../4.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
