<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The trial uses $N_1$ observations per arm if it stops at the first analysis and $N_2$ if it continues. Since $Z_1\sim N(\delta\sqrt{I_1},1)$,

$$
\mathbb P_\delta(\text{continue})
=\Phi(e_1-\delta\sqrt{I_1})-\Phi(f_1-\delta\sqrt{I_1}).
$$

Therefore the expected per-arm sample size is

$$
\boxed{
\mathbb E_\delta N
=N_1+(N_2-N_1)
\left\{\Phi(e_1-\delta\sqrt{I_1})-\Phi(f_1-\delta\sqrt{I_1})\right\}}.
$$

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
