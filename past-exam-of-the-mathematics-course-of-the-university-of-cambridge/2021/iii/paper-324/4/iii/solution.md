<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Take any bounded-error polynomial-size quantum circuit for a language in $\mathrm{BQP}$ and express it using $H,CX,S,T$. Replace each $T$ gate by the supplied $T$-gadget. Before measurements and conditional corrections, the resulting circuit uses only [Clifford gates](../../../../../../clifford-gate.md) and has a product input consisting of the original input and one magic state $|A\rangle$ per gadget.

Consider the branch in which all $t=\operatorname{poly}(n)$ gadget measurements return zero. No conditional $S$ corrections are then needed, so the ancilla measurements may be deferred to the end. This branch has known probability $2^{-t}$, and conditioned on it the remaining output is exactly that of the original universal circuit.

The assumed simulator applies with $K=t+1$: ask it for the joint probabilities

$$
p(0^t,{\rm accept}),\qquad p(0^t)=2^{-t}.
$$

Using polynomially many bits of requested precision, compute

$$
\Pr({\rm accept}\mid0^t)
=2^t p(0^t,{\rm accept}).
$$

The usual bounded-error gap separates yes instances from no instances, so this conditional probability decides the language deterministically in polynomial time. Hence $\mathrm{BQP}\subseteq\mathrm P$. The reverse inclusion is immediate because a quantum computer can implement classical deterministic computation, and therefore

$$
\boxed{\mathrm P=\mathrm{BQP}}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
