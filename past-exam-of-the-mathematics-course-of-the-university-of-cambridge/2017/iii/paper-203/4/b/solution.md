<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\psi_A=g_A-g_A(0)$, and take another admissible [compact H-hull](../../../../../../compact-h-hull.md) $B$ in the image [complex upper half-plane](../../../../../../upper-half-plane-complex-analysis.md). Form the hull $C=A\cup\psi_A^{-1}(B)$, including its relative [closure](../../../../../../closure-topology.md) and filling bounded complementary components if needed. Its [mapping-out function of a compact H-hull](../../../../../../mapping-out-function-of-a-compact-h-hull.md) is

$$
g_C=g_B\circ\psi_A+g_A(0).
$$

Indeed, this composition maps the correct remaining [domain](../../../../../../domain-mathematical-analysis.md) onto $\mathbb H$, and its constant term at infinity is zero. Since $\psi_A(0)=0$, the [chain rule](../../../../../../chain-rule.md) gives

$$
g_C'(0)=g_B'(0)g_A'(0).
$$

Both [derivatives](../../../../../../derivative.md) are positive by local [Schwarz reflection principle](../../../../../../schwarz-reflection-principle.md) and [boundary](../../../../../../boundary-of-a-set.md) orientation. Therefore the assumed avoidance formula gives

$$
\mathbb P(\psi_A(\gamma)\cap B=\varnothing\mid\gamma\cap A=\varnothing)=\frac{g_C'(0)^\alpha}{g_A'(0)^\alpha}=g_B'(0)^\alpha=\mathbb P(\gamma\cap B=\varnothing).
$$

The conditioning event has positive probability because $g_A'(0)>0$.

It remains to justify that these equalities determine the law. For a proper [simple curve](../../../../../../simple-curve.md) from $0$ to infinity, its complement has two sides, each [connected](../../../../../../connected-space.md) to an interval of the real [boundary](../../../../../../boundary-of-a-set.md). Any point off the curve lies in a thin polygonal tube attached to that [boundary](../../../../../../boundary-of-a-set.md) which avoids both the curve and zero; its [closure](../../../../../../closure-topology.md), with an end cap, is an admissible [compact H-hull](../../../../../../compact-h-hull.md). A countable collection of tubes with rational geometry therefore reconstructs the complement as the union of the tubes avoided by the curve.

The joint distribution of their avoidance indicators is also determined. Avoiding finitely many tubes is equivalent to avoiding the filled union when that union is admissible. If the union separates $0$ from infinity, avoidance is impossible and the joint probability is zero. Otherwise a [simple curve](../../../../../../simple-curve.md) cannot enter the bounded complementary pockets without crossing the union, so filling does not change the avoidance event. Finite joint avoidance probabilities consequently come from the same single-hull formulas; [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) supplies every finite indicator pattern. These patterns determine the random complement and hence the unparameterized simple trace.

Thus [avoidance probabilities determine a simple chordal curve law](../../../../../../avoidance-probabilities-determine-a-simple-chordal-curve-law.md), and the conditional image law above equals the original law. This proves the [derivative avoidance criterion for chordal restriction](../../../../../../derivative-avoidance-criterion-for-chordal-restriction.md), giving **the chordal restriction property**. Simplicity is essential to this reconstruction argument; it should not be replaced by a claim that arbitrary random closed sets are determined by these hull-avoidance tests.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
