# Aliasing of discrete Fourier modes

↑ **Parent:** [Discrete Fourier transform](discrete-fourier-transform-split.md)

For [integers](integer-split.md) $m,q,n$, adding $qN$ to a [frequency](frequency.md) index changes the [complex exponential](complex-exponential-function.md) by $e^{2\pi iqn}=1$. Thus different continuous [Fourier modes](fourier-mode.md) become identical [discrete Fourier modes](discrete-fourier-mode.md) on the sampling grid. This is [aliasing](aliasing.md), caused by sampling before any [discrete Fourier transform](discrete-fourier-transform-split.md) is computed.

For $N=8$, compare the continuous [functions](function-split.md) $\cos(2\pi mt)$ and $\sin(2\pi mt)$ with $m=1$ and $m=9$, sampled at $t=n/8$, $n=0,\ldots,7$. With $a=\sqrt2/2$, both [cosines](cosine.md) give exactly the first row and both [sines](sine.md) give exactly the second:

$$
\begin{array}{c|rrrrrrrr}
n&0&1&2&3&4&5&6&7\\\hline
\cos(2\pi n/8)=\cos(18\pi n/8)&1&a&0&-a&-1&-a&0&a\\
\sin(2\pi n/8)=\sin(18\pi n/8)&0&a&1&a&0&-a&-1&-a
\end{array}
$$

The nine-cycle [sine](sine.md) agrees in sign as well as magnitude with the one-cycle [sine](sine.md): the [frequency](frequency.md) indices differ by $8$, rather than by a sign reversal. Consequently, either [cosine](cosine.md) produces the same [discrete Fourier transform](discrete-fourier-transform-split.md), $X_1=X_7=4$ with all other [coefficients](coefficient.md) zero; either [sine](sine.md) produces $X_1=-4i$, $X_7=4i$, with all other [coefficients](coefficient.md) zero.

<a id="image-one-cycle-and-nine-cycle-cosine-and-sine-waves-have-exactly-the-same-eight-samples"></a>
![](discrete-sampling-frequency-aliasing.png)

**[Figure 2](#image-one-cycle-and-nine-cycle-cosine-and-sine-waves-have-exactly-the-same-eight-samples). One-cycle and nine-cycle cosine and sine waves have exactly the same eight samples**.

An observed low [frequency](frequency.md) therefore does not establish that physical high [frequencies](frequency.md) are absent. To exclude such alternatives, the [Nyquist–Shannon sampling theorem](nyquist-shannon-sampling-theorem.md) requires a specified class of [bandlimited functions](bandlimited-function.md). For arbitrary pure [sinusoids](sinusoid.md) with [frequencies](frequency.md) at most $B$, choose sampling rate $f_s>2B$; equality needs care because $\sin(2\pi(f_s/2)t)$ vanishes at every $t=n/f_s$. The finite-energy [L2 space](l2-space-is-a-hilbert-space.md) version of the [Nyquist–Shannon sampling theorem](nyquist-shannon-sampling-theorem.md) permits equality under its own hypotheses. In either case, exact continuous reconstruction generally requires the entire infinite sample [sequence](sequence.md); eight observed samples alone do not supply it. Demanet derives the grid [aliasing](aliasing.md) condition as a difference by an [integer](integer-split.md) multiple of the sampling [angular frequency](angular-frequency.md).[Laurent Demanet, MIT 18.330 notes, §6.2, Definition 11, p. 57: aliases on a grid, 2012](https://math.mit.edu/icg/resources/teaching/18.330/18.330-Mar21.pdf)

## ↑ Ancestors (6)

1. [Discrete Fourier transform](discrete-fourier-transform-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Discrete Fourier transform](discrete-fourier-transform-split.md)
