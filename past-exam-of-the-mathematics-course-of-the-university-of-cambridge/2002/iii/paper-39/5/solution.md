<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Code each factor level by $x_j\in\{-1,1\}$. A nonconstant [factorial contrast](../../../../../factorial-contrast.md) indexed by a nonempty factor set $A$ has sign column $g_A(x)=\prod_{j\in A}x_j$. Flipping any coordinate in $A$ reverses that sign and pairs the [treatment](../../../../../treatment.md) combinations, so exactly $2^{m-1}$ have each sign. Allocating the two signs to two [experimental blocks](../../../../../blocks-in-experimental-design.md) therefore divides the full [factorial design](../../../../../factorial-design.md) into equal [experimental blocks](../../../../../blocks-in-experimental-design.md). The [contrast](../../../../../contrast-statistics.md) is confounded with [experimental blocks](../../../../../blocks-in-experimental-design.md) because its column is constant within each [experimental block](../../../../../blocks-in-experimental-design.md): changing its coefficient and compensating by the two [experimental block](../../../../../blocks-in-experimental-design.md) [intercepts](../../../../../regression-intercept.md) leaves every fitted value unchanged. It has no information separate from [experimental block](../../../../../blocks-in-experimental-design.md) differences. Randomize the allocation of the two groups to days and the run order within days.

Write $A,B,C$ for temperature, pressure and catalyst, respectively, with low levels and catalyst one coded minus. In the supplied allocation, $ABC=-1$ on day one and $ABC=1$ on day two. Thus **the three-factor [interaction](../../../../../interaction-statistics.md) $ABC$ is confounded with days**. Every other nonconstant factorial column is [orthogonal](../../../../../orthogonal-vectors.md) to the day [contrast](../../../../../contrast-statistics.md), because its product with $ABC$ is a nonconstant sign column on the full cube and consequently sums to zero.

If all [interactions](../../../../../interaction-statistics.md) are negligible, the fitted model contains an [intercept](../../../../../regression-intercept.md), one day [contrast](../../../../../contrast-statistics.md) and the three [main effects](../../../../../main-effect.md). The corrected total [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) partition as

$$
\boxed{7=1\ \text{(days)}+1\ \text{(temperature)}+1\ \text{(pressure)}
+1\ \text{(catalyst)}+3\ \text{(residual)}.}
$$

The three residual [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md) are the unused [two-factor interaction](../../../../../two-factor-interaction.md) columns $AB,AC,BC$, pooled as error under the stated negligible-interaction assumption. There is no independent pure-error replication of [treatment](../../../../../treatment.md) combinations.

For four days with two runs each, **all three [main effects](../../../../../main-effect.md) can be estimated**. One regular allocation pairs each [treatment](../../../../../treatment.md) combination with its complete opposite:

$$
\begin{array}{c|cc}
\text{block}&\text{first }(A,B,C)&\text{second }(A,B,C)\\\hline
1&(-,-,-)&(+,+,+)\\
2&(-,-,+)&(+,+,-)\\
3&(-,+,-)&(+,-,+)\\
4&(-,+,+)&(+,-,-)
\end{array}
$$

The block-generating columns can be $AB$ and $AC$; their product $BC$ is also constant in [experimental blocks](../../../../../blocks-in-experimental-design.md). Thus $AB,AC,BC$ span the three [experimental block](../../../../../blocks-in-experimental-design.md) [contrasts](../../../../../contrast-statistics.md), while $A,B,C$ and $ABC$ vary within [experimental blocks](../../../../../blocks-in-experimental-design.md). The [main effects](../../../../../main-effect.md) remain mutually [orthogonal](../../../../../orthogonal-vectors.md) and separate from the [experimental block](../../../../../blocks-in-experimental-design.md) effects; with an additive main-effect model there is one residual degree of freedom, represented by $ABC$.

For the further request about $AC$, the distinction between regular confounding and unrestricted pairing is important. **A regular four-block allocation cannot retain all three [main effects](../../../../../main-effect.md) and $AC$.** Its three confounded columns form a rank-two defining subgroup. To preserve [main effects](../../../../../main-effect.md), these columns must lie in $\{AB,AC,BC,ABC\}$. If the subgroup includes $ABC$ and a two-factor column, their product is a main-effect column, which is forbidden. Hence the only permissible nonidentity subgroup is $\{AB,AC,BC\}$, and it necessarily confounds $AC$. This proves impossibility in the usual regular factorial-blocking framework, rather than relying on a count of available [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md).

The literal request does not explicitly restrict arrangements to regular [experimental blocks](../../../../../blocks-in-experimental-design.md). If arbitrary pairings are permitted, a nonregular construction can estimate $A,B,C,AC$ together, assuming the other [interactions](../../../../../interaction-statistics.md) are omitted from the model. An explicit allocation is

$$
\begin{array}{c|cc}
\text{block}&\text{first }(A,B,C)&\text{second }(A,B,C)\\\hline
1&(-,-,-)&(-,-,+)\\
2&(-,+,-)&(+,-,-)\\
3&(-,+,+)&(+,+,+)\\
4&(+,-,+)&(+,+,-)
\end{array}
$$

Every [treatment](../../../../../treatment.md) combination occurs exactly once. Fit one unrestricted [intercept](../../../../../regression-intercept.md) per day and the four coefficients $\beta_A,\beta_B,\beta_C,\beta_{AC}$. By [estimability from within-block differences](../../../../../estimability-from-within-block-differences.md), subtracting the second run from the first in each [experimental block](../../../../../blocks-in-experimental-design.md) removes all day effects and yields the coefficient [matrix](../../../../../matrix.md)

$$
D=\begin{pmatrix}
0&0&-2&2\\
-2&2&0&2\\
-2&0&0&-2\\
0&-2&2&2
\end{pmatrix},\qquad\det D=-64\ne0.
$$

Thus all four coefficients are uniquely determined from the four day differences. In this broader design class the answer is **yes, under the reduced four-effect model**. The resulting fit is saturated: four [experimental block](../../../../../blocks-in-experimental-design.md) [intercepts](../../../../../regression-intercept.md) plus four [treatment](../../../../../treatment.md) coefficients use all eight observations, leaving no residual estimate of error [variance](../../../../../variance-split.md). Replication or external error information would be needed for inference. This does not contradict the impossibility for regular [orthogonal](../../../../../orthogonal-vectors.md) confounding, and it does not claim simultaneous unbiased estimation when arbitrary additional [interactions](../../../../../interaction-statistics.md) are retained.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
