<h1 id="13a/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $r_+=\operatorname{Res}_{z=\alpha_+}g(z)$. For $\operatorname{Im}\lambda>-c$ and $\lambda\ne\alpha_+$, close $C_1$ upwards as before. The [residue theorem](../../../../../../../residue-theorem.md) includes the poles at $\lambda$ and $\alpha_+$, and the assumed decay in the upper region makes the arc contribution vanish. Thus

$$
H(\lambda)=g(\lambda)+\frac{r_+}{\alpha_+-\lambda}=g(\lambda)-\frac{r_+}{\lambda-\alpha_+}.
$$

It is essential to include the apparently exceptional point $\lambda=\alpha_+$. The [Laurent series](../../../../../../../laurent-series.md) there is $g(z)=r_+/(z-\alpha_+)+g_0(z)$ with $g_0$ [holomorphic](../../../../../../../complex-differentiability-at-a-point.md). At that point the integrand is $r_+/(z-\alpha_+)^2+g_0(z)/(z-\alpha_+)$, whose [residue](../../../../../../../residue.md) is $g_0(\alpha_+)$. Hence

$$
\boxed{H(\lambda)=g(\lambda)-\frac{r_+}{\lambda-\alpha_+},\quad H(\alpha_+)=g_0(\alpha_+)}.
$$

The displayed difference is interpreted by its [removable singularity](../../../../../../../removable-singularity.md). It therefore defines a [holomorphic](../../../../../../../complex-differentiability-at-a-point.md) function at every point of the required half-plane, including $\alpha_+$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [13A](../../../13a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
