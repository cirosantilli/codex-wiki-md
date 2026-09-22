<h1 id="a/2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [vaccinated epidemic-wave final size](../../../../../../vaccinated-epidemic-wave-final-size.md), write $s_-=s(-\infty)$. From the travelling-wave equations, $dv/ds=-\eta/(1+\eta)$ and $dm/ds=-1/[(1+\eta)s]$. Using the ahead-of-wave boundary data gives

$$
v(z)=\frac\eta{1+\eta}[s^*-s(z)],\qquad m(z)=\frac1{1+\eta}\log\frac{s^*}{s(z)}.
$$

Adding the four wave equations yields $q''+c(q+s+v+m)'=0$. Integrate once and use $q'(\infty)=0$ to obtain $q'+c(q+s+v+m)=cs^*$. At minus infinity the assumptions $q=q'=0$ therefore give $s_-+v_-+m_-=s^*$.

Combining these identities shows that $s_-$ satisfies

$$
\boxed{\log(s^*/s_-)=s^*-s_-.}
$$

The nontrivial positive epidemic-wave root has $0<s_-<1<s^*$; the other root $s_-=s^*$ is the disease-free solution. The assumed positive wave consequently requires $s^*>1$; for $s^*\leq1$ the displayed relation has no distinct smaller root.

At the back of the pulse there are no infectives, so the live [biological population](../../../../../../population-biology.md) consists of susceptible and vaccinated animals:

$$
\boxed{s_-+v_-=\frac{s_-+\eta s^*}{1+\eta}.}
$$

The final-size root is independent of [vaccination](../../../../../../vaccination.md) strength in this travelling-wave problem; [vaccination](../../../../../../vaccination.md) instead changes the split between deaths and survivors for the total [biological population](../../../../../../population-biology.md) lost from susceptibility.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
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
