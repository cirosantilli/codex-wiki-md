<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the standard convention that the [finite-variation process](../../../../../../finite-variation-process.md) $X$ has [càdlàg](../../../../../../cadlag.md) paths and that the [stochastic integral](../../../../../../stochastic-integral.md) starts from zero. Write $V(X)$ for its [total-variation process](../../../../../../total-variation-process.md). The necessary admissibility condition is $\int_{(0,t]}|H_s|\,dV_s(X)<\infty$ [almost surely](../../../../../../almost-sure-convergence.md) for each finite $t$; it holds, for example, for locally bounded $H$. Define the pathwise [Lebesgue-Stieltjes integral](../../../../../../lebesgue-stieltjes-integration.md)

$$
\boxed{(H\mathbin\cdot X)_t=\int_{(0,t]}H_s\,dX_s,\qquad(H\mathbin\cdot X)_0=0.}
$$

An atom at $s>0$ contributes $H_s\Delta X_s$, so this convention also fixes the treatment of jumps.

Fix $t$. For a generator $H_s=\mathbf1_A\mathbf1_{(a,b]}(s)$ of the [predictable sigma-algebra](../../../../../../predictable-sigma-algebra.md), with $A\in\mathcal F_a$, the [Lebesgue-Stieltjes integral](../../../../../../lebesgue-stieltjes-integration.md) is

$$
\mathbf1_A\bigl(X_{b\wedge t}-X_{a\wedge t}\bigr).
$$

It vanishes when $t\leq a$ and is $\mathcal F_t$-measurable otherwise. The [total-variation process](../../../../../../total-variation-process.md) is [adapted](../../../../../../adapted-process.md): for a [càdlàg](../../../../../../cadlag.md) path its value at $t$ is the [supremum](../../../../../../supremum.md) over a countable collection of [partitions of an interval](../../../../../../partition-of-an-interval.md) using rational interior points and endpoint $t$. Thus the positive and negative [Lebesgue-Stieltjes measures](../../../../../../lebesgue-stieltjes-measure.md) $dX^\pm=(dV(X)\pm dX)/2$ have $\mathcal F_t$-measurable masses on the generator intervals.

The [Monotone class theorem](../../../../../../monotone-class-theorem.md), applied separately to these positive [random measures](../../../../../../random-measure.md) on $[0,t]$, extends this measurability from the generators of the [predictable sigma-algebra](../../../../../../predictable-sigma-algebra.md) to all nonnegative [predictable processes](../../../../../../predictable-process.md). Truncation and positive/negative decomposition then cover every admissible $H$. Consequently **$H\mathbin\cdot X$ is [adapted](../../../../../../adapted-process.md).**

**The integrability condition is essential.** Taken literally, an arbitrary [previsible process](../../../../../../predictable-process.md) cannot always be integrated against a [finite-variation process](../../../../../../finite-variation-process.md): with $X_t=t$ and deterministic $H_s=s^{-1}$ for $s>0$, $H_0=0$, the proposed value at every $t>0$ diverges. The usual [càdlàg](../../../../../../cadlag.md) convention is also what identifies $dX$ by $dX((a,b])=X_b-X_a$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
