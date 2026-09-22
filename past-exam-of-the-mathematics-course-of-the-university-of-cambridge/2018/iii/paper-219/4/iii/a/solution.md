<h1 id="4/iii/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the abbreviations in (i). Keeping only terms involving $C_s$ in the joint kernel and completing the square gives

$$
\log p(C_s\mid\text{rest})=\text{constant}-\frac{(C_s-\mu_C)^2}{2v}-\frac{(o_s-E_s-C_s)^2}{2r_s}.
$$

Consequently the Gaussian latent-colour update is

$$
\boxed{C_s\mid\text{rest}\sim N(m_s,V_s),\qquad V_s=(v^{-1}+r_s^{-1})^{-1},\quad m_s=V_s\left(\frac{\mu_C}{v}+\frac{o_s-E_s}{r_s}\right)}.
$$

These $N$ updates are conditionally independent given the remaining variables. The flat mean prior gives one more normal full conditional:

$$
\boxed{\mu_C\mid\text{rest}\sim N\left(\overline C,\frac vN\right),\qquad\overline C=\frac1N\sum_sC_s}.
$$

The factorization uses $\sum_s(C_s-\mu_C)^2=\sum_s(C_s-\overline C)^2+N(\mu_C-\overline C)^2$. Together these are the $N+1$ normal draws in the formal [Gibbs sampler](../../../../../../../gibbs-sampler.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [Iii](../../iii.md)
3. [4](../../../4.md)
4. [Paper 219](../../../../paper-219-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
