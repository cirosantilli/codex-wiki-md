<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Part b shows that $H(Q_\alpha)$ decreases continuously from $H(Q_0)=\log_2|\mathcal A|$ to $H(Q_1)=H(Q)$. Because $Q$ is nonuniform, the variance in part b is positive, so for each intermediate $R$ there is a unique $\alpha^*\in(0,1)$ with $H(Q_{\alpha^*})=R$.

To minimize $D(P\|Q)$ subject to $H(P)\geq R$, the optimum lies on the boundary $H(P)=R$. The [Lagrange multiplier](../../../../../../lagrange-multiplier.md) equations for

$$
D(P\|Q)+\lambda\{R-H(P)\}+\nu\left(\sum_xP(x)-1\right)
$$

give $P(x)\propto Q(x)^\alpha$ for some $\alpha\in(0,1)$. The entropy constraint selects $\alpha=\alpha^*$ uniquely. Therefore

$$
\boxed{D^*(R,Q)=D(Q_{\alpha^*}\|Q).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
