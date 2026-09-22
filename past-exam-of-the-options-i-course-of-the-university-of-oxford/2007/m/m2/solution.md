<h1 id="m/m2/solution">Solution</h1>

↑ **Parent:** [M2](../m2.md)

A state $i$ is absorbing if $p_{ii}=1$, so once visited it is never left. Condition on the first step and use the [Markov property](../../../../markov-property.md): for $i\ne1$, the subsequent probability of ever reaching state one is $h_j$ given $X_1=j$. Hence $h_i=\sum_jp_{ij}h_j$, with $h_1=1$.

In this chain state four is a separate [absorbing state](../../../../absorbing-state.md), so $h_4=0$. The other two equations are

$$
h_2=\tfrac13+\tfrac23h_3,\qquad h_3=\tfrac14h_2.
$$

Solving gives

$$
\boxed{h_2=2/5,\qquad h_3=1/10,\qquad h_4=0}.
$$

Let $t_i$ be the mean time to hit the absorbing set. From either [transient state](../../../../transient-state.md) the next-step absorption probability is at least $1/3$, so its tail is geometrically bounded and the expectations are finite. [First-step analysis](../../../../first-step-analysis.md) gives $t_2=1+\tfrac23t_3$ and $t_3=1+\tfrac14t_2$. Thus $t_3=5/4+t_3/6$ and

$$
\boxed{\mathbb E_3\tau_{\{1,4\}}=3/2}.
$$

## ↑ Ancestors (12)

1. [M2](../m2.md)
2. [M](../../m.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the options I course of the University of Oxford](../../../split.md)
5. [Options I course of the University of Oxford](../../../../options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
