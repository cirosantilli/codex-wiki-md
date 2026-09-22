<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $v=\log u_\varepsilon$, [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) and part (a.ii) imply

$$
\rho^{1-n}\int_{B_\rho(z)\cap B_1}|Dv|
\leq C\left(\rho^{2-n}\int|Dv|^2\right)^{1/2}
\leq M(n,\mu).
$$

The [John-Nirenberg inequality](../../../../../../../john-nirenberg-inequality.md) therefore supplies $p_0=p_0(n,\mu)>0$ such that, with $v_{B_1}$ denoting the average,

$$
\int_{B_1}e^{p_0|v-v_{B_1}|}\leq C(n).
$$

Since $e^{p_0(v-v_{B_1})}$ and $e^{-p_0(v-v_{B_1})}$ are each bounded by this integrand,

$$
\boxed{\left(\int_{B_1}u_\varepsilon^{p_0}\right)
\left(\int_{B_1}u_\varepsilon^{-p_0}\right)
=\left(\int e^{p_0(v-v_{B_1})}\right)
\left(\int e^{-p_0(v-v_{B_1})}\right)
\leq C.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
