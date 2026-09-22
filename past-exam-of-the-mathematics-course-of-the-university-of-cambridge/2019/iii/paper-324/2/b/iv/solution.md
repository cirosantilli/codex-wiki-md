<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

An injective self-map of the finite set $\mathbb Z_N$ is a [bijection](../../../../../../../bijection.md). For sufficiently large $N$, exactly

$$
m=\lfloor N^{1/4}\rfloor+1
$$

outputs satisfy the integer comparison, so there are exactly $m$ good inputs. Prepare the [uniform superposition state](../../../../../../../uniform-superposition-state.md) $|\psi\rangle=N^{-1/2}\sum_x|x\rangle$, whose good probability is

$$
p=\frac mN=\Theta(N^{-3/4}).
$$

Use the phase oracle from the previous part and the reflection $2|\psi\rangle\langle\psi|-I$. The [amplitude amplification theorem](../../../../../../../amplitude-amplification.md) requires $O(p^{-1/2})$ iterations; each uses two $U_f$ queries, while the state preparation and its reflection are independent of $f$. With the nearest-integer iteration count from that theorem, the failure probability is at most $p$, tending to zero. Therefore the success probability eventually exceeds $0.9$, with

$$
\boxed{O(N^{3/8})\text{ queries to }U_f.}
$$

This is a bound on [quantum query complexity](../../../../../../../quantum-query-complexity.md); implementation costs of the known gates are not counted as oracle queries.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
