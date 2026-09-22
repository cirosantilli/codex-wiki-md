# Three-input two-point additive-noise channel

↑ **Parent:** [Discrete memoryless channel](discrete-memoryless-channel.md)

Let the input [alphabet](alphabet.md) be $\{0,1,2\}$ and let the output be $Y=X+Z$, where [independent](independent-random-variables.md) noise is uniform on two distinct integers. Translating the output [alphabet](alphabet.md) reduces the noise to $\{0,d\}$, $d\geq1$. The reachable output [alphabet](alphabet.md) has size $3+\min(d,3)$: it is the union of two three-element intervals shifted by $d$.

For $d=1$, every row of the [transition matrix](stochastic-matrix.md) has conditional [information entropy](information-entropy-split.md) one [bit](bit.md), so $I(X;Y)\leq\log_2 4-1=1$. Input [probabilities](probability.md) $(1/2,0,1/2)$ make the output uniform and attain one [bit](bit.md) per use. For $d\geq3$, the two translated input [alphabets](alphabet.md) are disjoint and every output identifies its input. A uniform input then attains $\log_2 3$ [bits](bit.md) per use.

For $d=2$, [reflection](reflection-mathematics.md) [symmetry](symmetry-physics.md) and [concavity of information entropy](concavity-of-information-entropy.md) permit restricting to input [probabilities](probability.md) $(s/2,1-s,s/2)$. Conditional on output [parity](parity.md), outputs whose labels are [even integers](even-number.md) have [probabilities](probability.md) $(1/4,1/2,1/4)$ and outputs whose labels are [odd integers](odd-integer.md) have [probabilities](probability.md) $(1/2,1/2)$. Consequently $I(X;Y)=h_2(s)+s/2$. Its strictly negative [second derivative](second-derivative.md) and stationary equation $\log_2((1-s)/s)+1/2=0$ give $s=\sqrt2/(1+\sqrt2)$ and [channel capacity](channel-capacity.md) $\log_2(1+\sqrt2)$. All three values follow from overlap of translated input [alphabets](alphabet.md), rather than from output [alphabet](alphabet.md) size alone.

## ↑ Ancestors (6)

1. [Discrete memoryless channel](discrete-memoryless-channel.md)
2. [Coding theory](coding-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
