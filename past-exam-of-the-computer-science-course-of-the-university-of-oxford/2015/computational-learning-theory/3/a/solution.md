<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [two-interval approximation by one interval](../../../../../two-interval-approximation-by-one-interval.md) supplies an approximation guarantee for every input [probability distribution](../../../../../probability-distribution-split.md) $D$. Merge overlapping target [intervals](../../../../../interval-mathematics.md), and write the target positive [set](../../../../../set-split.md) as at most two disjoint ordered [intervals](../../../../../interval-mathematics.md) $I_1,I_2$. Put $p_j=D(I_j)$ and $p=p_1+p_2$. If there is only one nonempty component, the target already belongs to the [interval](../../../../../interval-mathematics.md) [hypothesis class](../../../../../concept-class.md) and has zero [misclassification risk](../../../../../misclassification-risk.md). If the [interval](../../../../../interval-mathematics.md) notation permits empty [intervals](../../../../../interval-mathematics.md) and the target is empty, choose that same empty [interval](../../../../../interval-mathematics.md) in $H$.

In the two-component case, choosing the heavier component as the hypothesis loses only the lighter component, so its [misclassification risk](../../../../../misclassification-risk.md) is

$$
\min(p_1,p_2)\leq\frac p2.
$$

Alternatively, choose the single [interval](../../../../../interval-mathematics.md) $J$ spanning both components. This produces no false negatives, and its false positives lie in the gap. Its [misclassification risk](../../../../../misclassification-risk.md) is at most $1-p$. Both candidates are in $H$, so there exists an [interval](../../../../../interval-mathematics.md) $h^*$ with

$$
\operatorname{err}_D(h^*)\leq\min\left(\frac p2,1-p\right)\leq\frac13.
$$

For the last step, use $p/2\leq1/3$ if $p\leq2/3$, and $1-p\leq1/3$ if $p\geq2/3$. This avoids any assumption that an empty [interval](../../../../../interval-mathematics.md) or the whole real line belongs to $H$.

Use [empirical risk minimization](../../../../../empirical-risk-minimization.md) over [intervals](../../../../../interval-mathematics.md) on independent labelled examples. The generalization result needed here is the [VC uniform convergence theorem](../../../../../vc-uniform-convergence-theorem.md): for a binary [hypothesis class](../../../../../concept-class.md) of finite [VC dimension](../../../../../vc-dimension.md) $v$, there is a universal constant $A$ such that, for any labelled-data [probability distribution](../../../../../probability-distribution-split.md) and $0<\eta,\delta<1$, a sample size

$$
m\geq\frac A{\eta^2}\left(v\log\frac2\eta+\log\frac2\delta\right)
$$

ensures, with probability at least $1-\delta$, that every hypothesis's [empirical misclassification risk](../../../../../empirical-misclassification-risk.md) differs from its [misclassification risk](../../../../../misclassification-risk.md) by at most $\eta$. This theorem does not require the labels to be realizable by the [hypothesis class](../../../../../concept-class.md).[Sections “Uniform Convergence implies Agnostic PAC Learnability” and “Fundamental Theorem of Learnability”](../../../../../learnability-and-vc-dimension-in-mit-6-790.md)

The [interval](../../../../../interval-mathematics.md) [hypothesis class](../../../../../concept-class.md) has [VC dimension](../../../../../vc-dimension.md) two: any two ordered points can receive all four labellings, whereas an [interval](../../../../../interval-mathematics.md) cannot label three ordered points $1,0,1$. Take $\eta=1/24$ and choose an [interval](../../../../../interval-mathematics.md) $\widehat h$ minimizing the [empirical misclassification risk](../../../../../empirical-misclassification-risk.md). On the simultaneous convergence event,

$$
\begin{aligned}
\operatorname{err}_D(\widehat h)
&\leq\widehat{\operatorname{err}}(\widehat h)+\eta\\
&\leq\widehat{\operatorname{err}}(h^*)+\eta\\
&\leq\operatorname{err}_D(h^*)+2\eta\\
&\leq\frac13+\frac1{12}=\frac5{12}=\frac12-\frac1{12}.
\end{aligned}
$$

Therefore

$$
\boxed{C\text{ is weakly PAC learnable using }H,\qquad\gamma=\frac1{12}.}
$$

Since $v$ and $\eta$ are fixed constants, **$O(1+\log(1/\delta))$ examples suffice**, which is polynomial in $1/\delta$ as required by the paper's definition of [weak PAC learning](../../../../../weak-pac-learning.md).

For completeness, [empirical risk minimization](../../../../../empirical-risk-minimization.md) over [intervals](../../../../../interval-mathematics.md) is computationally effective. Sort the sample and group equal coordinates, since one [interval](../../../../../interval-mathematics.md) cannot split identical inputs. Give each group weight equal to the number of positive labels minus the number of negative labels in that group. The number of empirical mistakes made by an [interval](../../../../../interval-mathematics.md) is the total number of positives minus the total weight of the consecutive groups it contains. Select the consecutive block of maximum weight, or select a finite [interval](../../../../../interval-mathematics.md) outside the sample if every nonempty block has negative weight. This enumerates all possible sample labellings by [intervals](../../../../../interval-mathematics.md) and attains the minimum [empirical misclassification risk](../../../../../empirical-misclassification-risk.md); sorting and a maximum-block scan are sufficient. The [time complexity](../../../../../time-complexity.md) is $O(m\log m)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
