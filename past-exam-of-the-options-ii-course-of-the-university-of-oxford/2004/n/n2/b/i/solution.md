<h1 id="n/n2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $K\geq1$ is an integer, $0<p<1$, and put $q=1-p$. There is a discrepancy between the printed state definition and the formula requested later. We first follow the stated cumulative count, which retains previous good items when a defective item appears during phase A. The transition probabilities are

$$
P_{i,i}=p,\quad P_{i,i+1}=q\quad(0\leq i<K),\qquad
P_{K,0}=p/r,\quad P_{K,K}=1-p/r,
$$

with all others zero. The balance equations imply $q\pi_i=q\pi_{i-1}$ for $1\leq i<K$ and $(p/r)\pi_K=q\pi_{K-1}$. Thus

$$
\boxed{\pi_i=\frac p{Kp+rq}\quad(0\leq i<K),\qquad\pi_K=\frac{rq}{Kp+rq}}.
$$

For comparison, if clearance requires $K$ consecutive good items, each defect in phase A resets the state to zero. Replace its transitions by $P_{i,0}=p$, $P_{i,i+1}=q$, combining contributions if destinations coincide. Phase B retains its two transitions. For this [consecutive-clearance inspection model](../../../../../../consecutive-clearance-inspection-model.md), balance yields $\pi_i=q^i\pi_0$ and $(p/r)\pi_K=q^K\pi_0$. With $D=1+(r-1)q^K$, normalization gives

$$
\boxed{\pi_i=\frac{pq^i}{D}\quad(0\leq i<K),\qquad\pi_K=\frac{rq^K}{D}}.
$$

This second model is the one giving the printed formula in part (iii). It is a different transition rule, rather than an algebraic simplification of the cumulative model.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [N2](../../../n2.md)
4. [N](../../../../n.md)
5. [2004](../../../../../2004-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
