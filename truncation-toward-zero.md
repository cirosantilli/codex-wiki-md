# Truncation toward zero

↑ **Parent:** [Floor and ceiling functions](floor-and-ceiling-functions.md)

Truncation toward zero removes the fractional magnitude of a [real number](real-number.md), giving the [integer](integer-split.md) obtained by applying the [floor function](floor-function.md) to its [absolute value](absolute-value.md) and restoring the original sign; a magnitude below one gives zero. More precisely,

$$
\operatorname{trunc}(x)=\begin{cases}\lfloor x\rfloor&x\geq0,\\\lceil x\rceil&x<0.\end{cases}
$$

The result is zero for $-1<x<1$. For example, $\operatorname{trunc}(2.7)=2$ and $\operatorname{trunc}(-2.7)=-2$, whereas $\lfloor-2.7\rfloor=-3$. Python's `math.trunc` uses this towards-zero convention, so replacing it by `math.floor` changes calculations with negative noninteger inputs. [Python 3.14 math.trunc documentation: floor on positive inputs, ceiling on negative inputs](https://docs.python.org/3.14/library/math.html#math.trunc).

<a id="image-truncation-toward-zero-is-symmetric-in-sign-while-the-fractional-part-defined-by-the-floor-function-is-always-nonnegative"></a>
![](truncation-toward-zero-and-signed-errors.png)

**[Figure 4](#image-truncation-toward-zero-is-symmetric-in-sign-while-the-fractional-part-defined-by-the-floor-function-is-always-nonnegative). Truncation toward zero is symmetric in sign, while the fractional part defined by the floor function is always nonnegative**. Left: exact integer endpoint values distinguish the two sign-dependent truncation rules; a whole neighborhood of zero maps to zero. Right: $x-\operatorname{trunc}(x)$ takes the sign of a noninteger input, while $x-\lfloor x\rfloor$ lies in $[0,1)$ on both sides of zero. Open endpoints show excluded limiting values.

For every [real number](real-number.md) $x$,

$$
|x-\operatorname{trunc}(x)|<1,\qquad \operatorname{trunc}(-x)=-\operatorname{trunc}(x).
$$

The discarded difference $x-\operatorname{trunc}(x)$ has the sign of $x$ when $x$ is noninteger. In contrast, the [fractional part](fractional-part.md) $x-\lfloor x\rfloor$ is always in $[0,1)$. At $x=-2.7$, these two differences are $-0.7$ and $0.3$. Thus specifying a signed fractional remainder requires specifying which integer-valued operation is used.

Unlike the [floor function](floor-function.md) and [ceiling function](ceiling-function.md), [truncation toward zero](truncation-toward-zero.md) need not commute with adding an [integer](integer-split.md). At $x=-0.7$ and $j=1$, $\operatorname{trunc}(x+j)=\operatorname{trunc}(0.3)=0$, whereas $\operatorname{trunc}(x)+j=1$. This matters if negative coordinates are assigned to equal-width bins by converting a quotient to an [integer](integer-split.md): $x=-0.7$ belongs to the bin $[-1,0)$ under the [floor function](floor-function.md), but truncation gives zero. The appropriate operation follows from the declared bin [intervals](interval-mathematics.md).

[Truncation toward zero](truncation-toward-zero.md) is a [nondecreasing function](nondecreasing-function.md) with a [discontinuity of a function](discontinuity-of-a-function.md) at each nonzero [integer](integer-split.md). It has no [discontinuity of a function](discontinuity-of-a-function.md) at zero, because it is identically zero on $(-1,1)$. Its agreement with the [floor function](floor-function.md) on the positive side and the [ceiling function](ceiling-function.md) on the negative side explains the different closed endpoints in the diagram.

## ↑ Ancestors (7)

1. [Floor and ceiling functions](floor-and-ceiling-functions.md)
2. [Calculus](calculus-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Floor and ceiling functions](floor-and-ceiling-functions.md)
- [Fractional part](fractional-part.md)
- [Truncation toward zero](truncation-toward-zero.md)
