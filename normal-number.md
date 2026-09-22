# Normal number

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_number)

A [real number](real-number.md) is normal in an [integer](integer.md) base $K\geq2$ when every finite [word](string.md) of digits occurs in its [positional notation](positional-notation.md) with the same limiting [digit block frequency](digit-block-frequency.md) as every other [word](string.md) of the same length. Write its [fractional part](fractional-part.md) as $x=0.d_1d_2\ldots$ in base $K$, using the expansion that is not eventually all $K-1$ digits when two expansions are possible. For every length $r\geq1$ and every [word](string.md) $w\in\{0,\ldots,K-1\}^r$, the requirement is

$$
\lim_{N\to\infty}\frac{\left|\{1\leq j\leq N-r+1:(d_j,\ldots,d_{j+r-1})=w\}\right|}{N-r+1}=K^{-r}.
$$

Occurrences overlap: the [word](string.md) $11$ occurs twice in $111$. There are $K^r$ possible [words](string.md) of length $r$, so $K^{-r}$ is the equal share for each. In a [decimal representation](decimal-representation.md), this means frequency $1/10$ for each digit, $1/100$ for each pair, and $1/1000$ for each triple, continuing through every finite length. The definition agrees with that used by Copeland and Erdős in their work on explicit [normal numbers](normal-number.md). [Arthur H. Copeland and Paul Erdős, Note on Normal Numbers, 1946, opening definition](https://users.renyi.hu/~p_erdos/1946-01.pdf)

The appeal is that a precise, deterministic [real number](real-number.md) can have the same limiting [digit block frequencies](digit-block-frequency.md) as repeated draws from a [uniform distribution on a finite set](discrete-uniform-distribution.md), with [independence](independent-random-variables.md) between draws. [Champernowne constant](champernowne-constant.md) is an explicit example. Normality is useful for studying digit distribution, but balanced digits alone establish only a [simply normal number](simply-normal-number.md), and a finite sample cannot establish any of these infinite [limits](limit-of-a-function.md).

Émile Borel introduced [normal numbers](normal-number.md) and established their prevalence in his 1909 paper applying [probability](probability.md) to [number theory](number-theory-split.md); the stronger all-base statement is discussed under [absolutely normal number](absolutely-normal-number.md). [Émile Borel, Les probabilités dénombrables et leurs applications arithmétiques, Rendiconti del Circolo Matematico di Palermo 27, 247–271, 1909](https://doi.org/10.1007/BF03019651)

**Table of contents**

- [Digit block frequency](digit-block-frequency.md)
- [Simply normal number](simply-normal-number.md)
- [Champernowne constant](champernowne-constant.md)
- [Normality and equidistribution under integer multiplication](normality-and-equidistribution-under-integer-multiplication.md)
- [Absolutely normal number](absolutely-normal-number.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Absolutely normal number](absolutely-normal-number.md)
- [Cantor Bernoulli measure](cantor-bernoulli-measure.md)
- [Champernowne constant](champernowne-constant.md)
- [Digit block frequency](digit-block-frequency.md)
- [Normal number](normal-number.md)
- [Normality and equidistribution under integer multiplication](normality-and-equidistribution-under-integer-multiplication.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-108/4/solution.md)
- [Simply normal number](simply-normal-number.md)
