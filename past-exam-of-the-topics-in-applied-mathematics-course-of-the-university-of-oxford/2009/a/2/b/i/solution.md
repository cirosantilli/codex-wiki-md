<h1 id="a/2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

While $q>0$ and $s>0$, division of the equations gives $dq/ds=(1-s)/[(1+\eta)s]$ and $dv/ds=-\eta/(1+\eta)$. Integrating from the initial data yields

$$
q(s)=q_0+\frac{s_0-s+\log(s/s_0)}{1+\eta},\qquad v(s)=\frac\eta{1+\eta}(s_0-s).
$$

Let $s_\infty$ be the final susceptible level. Using $q_\infty=0$ gives

$$
\boxed{s_\infty-\log s_\infty=s_0-\log s_0+(1+\eta)q_0,\qquad0<s_\infty<\min(s_0,1).}
$$

This is the smaller positive root selected by decreasing susceptibility; the function $s-\log s$ is decreasing on $(0,1)$, so that selected root is unique. Its upper bound below $s_0$ also follows directly because the added positive term moves the decreasing-branch root left.

Conservation of the total count, or integration of $m_t=q$, then gives the number killed, including those initially infected:

$$
\boxed{m_\infty=q_0+\frac{s_0-s_\infty}{1+\eta}.}
$$

The remaining susceptible loss is split between [infection](../../../../../../infection.md) and [vaccination](../../../../../../vaccination.md) in fixed ratio $1:\eta$; this explains the factor multiplying $s_0-s_\infty$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../../../split.md)
7. [Topics in applied mathematics course of the University of Oxford](../../../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
