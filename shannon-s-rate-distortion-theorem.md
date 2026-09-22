<h1 id="shannon-s-rate-distortion-theorem">Shannon's rate-distortion theorem</h1>

↑ **Parent:** [Rate-distortion function](rate-distortion-function.md)

For a finite [alphabet](alphabet.md) source with [independent and identically distributed](independent-and-identically-distributed-random-variables.md) symbols, a finite [reconstruction alphabet](reconstruction-alphabet.md), and a bounded nonnegative [separable distortion](separable-distortion.md), the [rate-distortion function](rate-distortion-function.md) is the asymptotic limit for [fixed-length lossy codes](fixed-length-lossy-code.md). In particular, for a distortion target in the interior of the feasible range and every $\varepsilon>0$, sufficiently long [block codes](block-code.md) exist with rate at most $R(D)+\varepsilon$ and [expected distortion](expected-distortion.md) at most $D+\varepsilon$. Every such $n$-symbol code obeys $R_n\geq R(D_n)$, where $D_n$ is its actual [expected distortion](expected-distortion.md).[§24.1, Theorem 24.1, printed pp. 246–247; §24.2, Theorem 24.2, printed p. 247](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-24-rate-distortion-achievability-bounds.md)

The outline is instructive. The [data processing inequality](data-processing-inequality.md) bounds the [mutual information](mutual-information.md) in a reconstruction by the [information entropy](information-entropy.md) of the transmitted message, which is at most $\log_2 M_n$. [Independence](independent-random-variables.md) and the [convexity](convex-function.md) of the [rate-distortion function](rate-distortion-function.md) then give the per-symbol lower bound. For achievability, choose many reconstruction blocks using a suitable [probability distribution](probability-distribution.md), so that the source's typical blocks are likely to have an acceptable nearby reconstruction. This is a covering argument; it does not require recovering the original block exactly.

## ↑ Ancestors (7)

1. [Rate-distortion function](rate-distortion-function.md)
2. [Rate-distortion theory](rate-distortion-theory.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
