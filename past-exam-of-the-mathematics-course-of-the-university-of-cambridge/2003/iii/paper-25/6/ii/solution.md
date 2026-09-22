<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The proof of [Szemerédi theorem](../../../../../../szemeredi-s-theorem.md) for four-term progressions follows a uniformity-versus-density-increment iteration. Fix a positive starting density; the quantitative parameters below depend only on that density.

First apply the counting argument in part (i). A sufficiently long set with no nonconstant four-term [arithmetic progression](../../../../../../arithmetic-progression.md) cannot have small balanced [Gowers U3 norm](../../../../../../gowers-u3-norm.md). Thus its balanced function has a quantitatively large cube average. The [Derivative identity for the Gowers U3 norm](../../../../../../derivative-identity-for-the-gowers-u3-norm.md) expresses this as an average of fourth Fourier moments of the multiplicative derivatives $x\mapsto f(x+h)\overline{f(x)}$. Many shifts therefore have a derivative with a large [Fourier coefficient](../../../../../../fourier-coefficient.md).

The next step is the inverse argument. Choose these frequencies as a function of the shifts. The relations between repeated derivatives force a large part of the resulting frequency graph to have many additive quadruples. A [Balog-Szemerédi-Gowers theorem](../../../../../../balog-szemeredi-gowers-theorem.md) extraction followed by [Freiman theorem for integer sets](../../../../../../freiman-theorem-for-integer-sets.md) organizes this graph on a bounded-complexity additive model. Integrating the organized derivative frequencies yields correlation of $f$ with a locally quadratic phase on a structured region. On integer intervals this is generally a local quadratic phase on a Bohr-type region, or equivalent two-step structure; it need not be one global quadratic polynomial on the entire interval.

The quantitative density-increment lemma obtained from that inverse argument says that either the interval is bounded in size by a function of its density, or there is a nonempty integer progression of length at least $c(\delta)N^{c(\delta)}$ on which the density increases by at least $c(\delta)>0$. The passage from correlation to this increment partitions the structured region into progressions on which the phase varies very little, controls discarded boundaries, and uses the balanced function's zero mean to find a positive-density gain. Both the gain and the size exponent are bounded away from zero for densities above the fixed starting density.

Reidentify the new progression with an interval and repeat. The property of having no nonconstant four-term progression is preserved under this affine identification. Density can increase only finitely many times before it exceeds one. Starting with $N$ sufficiently large ensures that the successive power-type length losses never reach the exceptional bounded-size case during those finitely many steps. This contradiction proves that every fixed positive density has a threshold beyond which a four-term progression must occur. The counting lemma, inverse structural argument, density increment and final iteration are the main steps; the deep inverse step is only outlined here, as permitted by this part of the question.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
