<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the probability of failing to restore an arbitrary unknown input in the original encoded subspace as the error criterion. With no extraction fault, the [bit-flip repetition code](../../../../../../bit-flip-repetition-code.md) succeeds exactly on channel-error patterns of weight zero or one. Independent physical flips give

$$
A=(1-p)^3+3p(1-p)^2=1-3p^2+2p^3,
\qquad B=1-A=3p^2-2p^3.
$$

The probability $B$ is the logical bit-flip probability for the ideal recovery. The preceding calculation shows that every occurrence of the specified internal fault leaves the code space. Independence of that fault therefore gives [exact encoded-state failure with a faulty parity check](../../../../../../exact-encoded-state-failure-with-a-faulty-parity-check.md):

$$
\boxed{P_{\mathrm{fail}}=q+(1-q)B,qquad
P_{\mathrm{success}}=(1-q)A.}
$$

A single unencoded qubit has bit-flip error probability $p$. Thus the encoded scheme improves this error criterion precisely when

$$
q+(1-q)B<p.
$$

For $0<p<1/2$, $p-B=p(1-p)(1-2p)>0$ and $A=(1-p)^2(1+2p)>0$. Rearranging gives

$$
\boxed{q<q_{\mathrm{th}}(p)=\frac{p-3p^2+2p^3}{1-3p^2+2p^3}
=\frac{p(1-2p)}{(1-p)(1+2p)}.}
$$

Equality gives no improvement. At $p=0$ the unencoded channel is already perfect; at $p=1/2$ ideal recovery only ties it. For $1/2<p\leq1$, the stipulated majority correction is no better even without the internal fault, and this fault cannot improve it. Hence there is no nonnegative $q$ giving a strict improvement in those ranges.

The criterion concerns restoration of every possible logical state: a logical bit flip can accidentally preserve a particular logical $X$ eigenstate, but that is not protection of an unknown input. The threshold assumes the displayed single fault location and ideal encoding, measurement and conditional correction. Adding another recovery circuit or comparing a different average-fidelity metric would define a different noise model or performance criterion.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
