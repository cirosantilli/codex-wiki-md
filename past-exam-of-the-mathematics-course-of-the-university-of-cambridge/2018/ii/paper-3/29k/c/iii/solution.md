<h1 id="29k/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume (iii). Fix $t\in\{1,\ldots,T\}$, a coordinate $i$, and an event $A\in\mathcal F_{t-1}$. Choose the bounded predictable risky strategy

$$
\theta_s=\mathbf1_Ae_i\mathbf1_{\{s=t\}},
$$

and choose the numéraire holding to make the strategy self-financing with $V_0=0$. Its terminal discounted value is

$$
V_T=\mathbf1_A(X_t^i-X_{t-1}^i).
$$

Condition (iii) yields

$$
\mathbb E_{\mathbb Q}[
\mathbf1_A(X_t^i-X_{t-1}^i)]=0
$$

for every $A\in\mathcal F_{t-1}$. The defining property of [conditional expectation](../../../../../../../conditional-expectation.md) implies

$$
\mathbb E_{\mathbb Q}[X_t^i\mid\mathcal F_{t-1}]
=X_{t-1}^i.
$$

Every coordinate is therefore a $\mathbb Q$-martingale, so **(iii) $\Rightarrow$ (i)**. This proves the [martingale characterization by bounded self-financing strategies](../../../../../../../martingale-characterization-by-bounded-self-financing-strategies.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [29K](../../../29k.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
