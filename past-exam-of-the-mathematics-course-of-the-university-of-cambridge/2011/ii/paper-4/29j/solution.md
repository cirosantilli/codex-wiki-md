<h1 id="29j/solution">Solution</h1>

↑ **Parent:** [29J](../29j.md)

Write $c_1=X_1-Y$, $c_2=X_2+Y$, both positive, and $W_j=U_j'(c_j)>0$. As usual the utility expectations must be meaningful; the improvement below is supported where both consumptions and derivatives are bounded, so it produces finite strictly positive expected gains without a tail differentiation problem.

Suppose $R=W_1/W_2$ is not almost surely constant. Choose $0<l<h$ and positive-probability sets $A$ and $B$ on which respectively $R\ge h$ and $R\le l$. By restricting these sets if necessary, keep both consumptions bounded and bounded away from zero, and their marginal utilities bounded. Put $a=\mathbb E(W_2\mathbf1_A)>0$, $b=\mathbb E(W_2\mathbf1_B)>0$, and choose $d$ strictly between $lb/(ha)$ and $b/a$. For $Z=\mathbf1_B-d\mathbf1_A$, we have

$$
\mathbb E(W_2Z)=b-da>0,\qquad
\mathbb E(W_1Z)\le lb-dha<0.
$$

Replace $Y$ by $Y+\delta Z$ for small positive $\delta$. Agent one's utility has first derivative $-\mathbb E(W_1Z)>0$, and agent two's has derivative $\mathbb E(W_2Z)>0$. Positivity of consumptions is preserved on the bounded support, and uniform Taylor estimates there make both actual gains positive for sufficiently small $\delta$. Thus a Pareto-efficient transfer must satisfy

$$
\boxed{U_1'(X_1-Y)/U_2'(X_2+Y)=\lambda\quad\text{almost surely},\qquad\lambda>0.}
$$

For given total wealth $s=X_1+X_2>0$, let $c$ be agent two's consumption. The ratio $R_s(c)=U_1'(s-c)/U_2'(c)$ is continuous and strictly increasing for $0<c<s$, by [strict concavity](../../../../../strict-concavity.md). The endpoint marginal-utility assumptions give $R_s(c)\to0$ as $c\downarrow0$ and $R_s(c)\to\infty$ as $c\uparrow s$. Thus it has a unique solution $c=h_\lambda(s)$ to $R_s(c)=\lambda$. Continuous dependence on $s$ follows from strict monotonicity and continuity, so this solution is a measurable wealth-sharing rule. Therefore

$$
\boxed{X_2+Y_\lambda=h_\lambda(X_1+X_2),\qquad
Y_\lambda=h_\lambda(X_1+X_2)-X_2.}
$$

For a fixed weight, it is also the pointwise maximizer of $U_1(s-c)+\lambda U_2(c)$, whose [strict concavity](../../../../../strict-concavity.md) confirms uniqueness.

## ↑ Ancestors (10)

1. [29J](../29j.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
