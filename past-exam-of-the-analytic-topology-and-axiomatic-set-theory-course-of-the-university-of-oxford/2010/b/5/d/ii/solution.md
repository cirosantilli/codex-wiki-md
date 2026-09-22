<h1 id="b/5/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $\kappa=\aleph_\omega$. Apply [König theorem for cardinal numbers](../../../../../../konig-s-theorem-set-theory.md) to the sequences $\aleph_n<\aleph_{n+1}$:

$$
\kappa=\sum_{n<\omega}\aleph_n
<\prod_{n<\omega}\aleph_{n+1}\leq\kappa^{\aleph_0}.
$$

The sum is $\kappa$ because the countable [union](../../../../../../set-union.md) has [cardinality](../../../../../../cardinality.md) at most $\kappa$ and its summands are cofinal in $\kappa$. Thus the power is strictly larger than $\kappa$, a fact that cannot be replaced by the regular-cardinal calculation of the preceding part.

For an upper bound, use $\kappa\leq2^\kappa$ and the [currying law for cardinal exponentiation](../../../../../../currying-law-for-cardinal-exponentiation.md):

$$
\kappa^{\aleph_0}\leq(2^\kappa)^{\aleph_0}
=2^{\kappa\cdot\aleph_0}=2^\kappa=\kappa^+,
$$

where the last step is GCH at $\kappa$. There is no cardinal strictly between $\kappa$ and its successor, so

$$
\boxed{\aleph_\omega^{\aleph_0}=\aleph_{\omega+1}.}
$$

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../../split.md)
7. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
