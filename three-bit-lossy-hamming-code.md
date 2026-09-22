# Three-bit lossy Hamming code

↑ **Parent:** [Hamming distortion](hamming-distortion.md)

Let $X_1,X_2,X_3$ be [independent](independent-random-variables.md) fair [bits](bit.md). The [encoder](channel-encoder.md) sends their majority [bit](bit.md): zero when at least two inputs are zero, and one otherwise. The [decoder](channel-decoder.md) reconstructs $000$ or $111$ by repeating that received [bit](bit.md) three times. This is [lossy compression](lossy-compression.md): different original strings deliberately share a reconstruction.

There are eight equally likely inputs. The strings $000$ and $111$ have zero [Hamming distance](hamming-distance.md) from their reconstructions; each of the other six has [Hamming distance](hamming-distance.md) one. One transmitted [bit](bit.md) represents three source symbols, so

$$
\boxed{R=\frac13,\qquad D=\frac{2\cdot0+6\cdot1}{8\cdot3}=\frac14.}
$$

Every input has average [Hamming distortion](hamming-distortion.md) at most $1/3$, whereas the population average is $1/4$. The actual [block code](block-code.md) therefore obeys $R\geq R(D)\approx0.18872$, but does not reach the optimal long-block rate.

<a id="image-eight-equally-likely-source-strings-become-two-reconstructions-using-one-transmitted-bit"></a>
![](three-bit-lossy-hamming-code.png)

**[Figure 18](#image-eight-equally-likely-source-strings-become-two-reconstructions-using-one-transmitted-bit). Eight equally likely source strings become two reconstructions using one transmitted bit**. The [encoder](channel-encoder.md) sends the majority [bit](bit.md). Orange highlights a reconstructed [bit](bit.md) that differs from its input. Six source strings have one mismatch and two have none, giving average [Hamming distortion](hamming-distortion.md) $1/4$ per source symbol. No errors occur in the transmission model; the loss is introduced deliberately by the [encoder](channel-encoder.md).

This construction uses the same reconstruction strings as the threefold [binary repetition code](binary-repetition-code.md), but the tasks differ. An error-correcting [encoder](channel-encoder.md) expands one source [bit](bit.md) into three transmitted [bits](bit.md); this [lossy compression](lossy-compression.md) example compresses three source [bits](bit.md) into one transmitted [bit](bit.md). The source distribution and the direction of the mapping matter.

## ↑ Ancestors (8)

1. [Hamming distortion](hamming-distortion.md)
2. [Rate-distortion function](rate-distortion-function.md)
3. [Rate-distortion theory](rate-distortion-theory.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Rate-distortion function](rate-distortion-function.md)
