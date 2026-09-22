<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Follow the printed examples by counting positive squares, so zero is not marked. For $N\geq2$, the marked output set is

$$
S=\{k^2:1\leq k\leq\lfloor\sqrt{N-1}\rfloor\},\qquad K=|S|=\lfloor\sqrt{N-1}\rfloor.
$$

A one-to-one map from the finite set $[N]$ to itself is a [permutation](../../../../../../permutation.md), so exactly $K$ inputs have outputs in $S$. In the [uniform quantum superposition](../../../../../../uniform-quantum-superposition.md) $|s\rangle=N^{-1/2}\sum_x|x\rangle$, the initial good probability is therefore $p=K/N$. For [permutation-preimage quantum search](../../../../../../permutation-preimage-quantum-search.md), this known [marked density under a permutation](../../../../../../marked-density-under-a-permutation.md) is $\Theta(N^{-1/2})$.

Define the efficiently computable predicate $h(y)$ to be one if and only if $y$ is a positive square. The assumed [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) for $h$, acting on $y$ and a $|-\rangle$ ancilla, implements its diagonal sign operation $D_h|y\rangle=(-1)^{h(y)}|y\rangle$. Compute the [modular-addition quantum oracle](../../../../../../modular-addition-quantum-oracle.md) into a zero output register, apply this sign operation, and uncompute:

$$
|x\rangle|0\rangle\xrightarrow{U_f}|x\rangle|f(x)\rangle
\xrightarrow{D_h}(-1)^{h(f(x))}|x\rangle|f(x)\rangle
\xrightarrow{U_f^\dagger}(-1)^{h(f(x))}|x\rangle|0\rangle.
$$

This implements $I_{\mathcal G}$ for $\mathcal G=\operatorname{span}\{|x\rangle:f(x)\in S\}$, with the work registers clean. Only forward calls to $U_f$ were promised, but its inverse costs one such call: if $J|y\rangle=|-y\bmod N\rangle$ on the second register, then

$$
\boxed{U_f^\dagger=(I\otimes J)U_f(I\otimes J).}
$$

Indeed the output addition is changed into subtraction. Thus each marked reflection costs exactly two queries to $U_f$; all other operations used here are independent of the unknown $f$.

Use the [amplitude amplification theorem](../../../../../../amplitude-amplification.md) with $|\psi\rangle=|s\rangle$, whose reflection is allowed by the assumptions. With $\theta=\arcsin\sqrt{K/N}$, choose $m$ nearest to $\pi/(4\theta)-1/2$. Here $p\leq1/2$ for every $N\geq2$, so a trial succeeds with probability at least $1/2$. Also

$$
m=O(\sqrt{N/K})=O(N^{1/4}).
$$

Measure $x$ and use one additional $U_f$ query to evaluate and check $f(x)$. On failure, restart with fresh registers. Four independent trials have failure probability at most $2^{-4}$, so **the required confidence and query bound are**

$$
\boxed{\Pr(\text{success})\geq\frac{15}{16}>0.9,\qquad
\#U_f\text{ queries}\leq4(2m+1)=O(N^{1/4}).}
$$

This is an upper bound on [quantum query complexity](../../../../../../quantum-query-complexity.md), not a claim that arbitrary reflections or every classical gate have constant cost. Including zero as a square would change $K$ to $K+1$ without changing the asymptotic bound. With the printed positive-square interpretation, $N=1$ has no valid output and no algorithm can satisfy the success requirement; the intended asymptotic task necessarily has $N\geq2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
