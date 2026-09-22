# Stars and bars (combinatorics)

↑ **Parent:** [Combinatorics](combinatorics-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stars_and_bars_(combinatorics))

[Stars and bars](stars-and-bars-combinatorics.md) counts [tuples](finite-tuple.md) of [nonnegative integers](natural-number.md) with a prescribed [sum](sum.md). For [integers](integer-split.md) $N\geq0$ and $k\geq1$, its statement is

$$
\#\{(x_1,\ldots,x_k):x_i\geq0,\ x_1+\cdots+x_k=N\}
=\binom{N+k-1}{k-1}.
$$

Such a [tuple](finite-tuple.md) is a [weak composition of an integer](weak-composition-of-an-integer.md). Think of $k$ labelled bins: $x_1$ counts identical objects in the first bin, $x_2$ in the second, and so on. Bin names distinguish positions even when counts agree. [Stars and bars](stars-and-bars-combinatorics.md) counts these count [tuples](finite-tuple.md); assigning individually distinct objects requires additional information. [Felix Gotti, MIT 18.211, Lecture 6: Compositions, Proposition 1 and Example 3](https://math.mit.edu/~fgotti/docs/Courses/C.%20Combinatorial%20Analysis/6.%20Compositions/Compositions.pdf)

**Computed example.** With $N=5$ and $k=3$, the number of [weak compositions of an integer](weak-composition-of-an-integer.md) is $\binom72=21$. The string `••|•|••` encodes $(2,1,2)$: two dots before the first bar, one between the bars, and two after the second. For a fixed first-bin count $x_1=a$, the second-bin count can be any [integer](integer-split.md) from $0$ to $5-a$ and the third is forced. Thus the direct count is $6+5+4+3+2+1=21$.

<a id="image-stars-and-bars-for-five-identical-objects-and-three-labelled-bins-ordinary-splits-adjacent-bars-and-bars-at-either-end"></a>
![](stars-and-bars-three-bin-allocation.png)

**[Figure 17](#image-stars-and-bars-for-five-identical-objects-and-three-labelled-bins-ordinary-splits-adjacent-bars-and-bars-at-either-end). Stars and bars for five identical objects and three labelled bins: ordinary splits, adjacent bars, and bars at either end**.

Adjacent bars encode an empty middle bin: `••||•••` gives $(2,0,3)$. A bar at the left end encodes an empty first bin, as in `|••|•••` for $(0,2,3)$; a bar at the right end encodes an empty third bin, as in `••|•••|` for $(2,3,0)$. These are valid [weak compositions of an integer](weak-composition-of-an-integer.md). For $N=0$ every count is zero, and for $k=1$ the unique [tuple](finite-tuple.md) is $(N)$, consistent with $\binom{N}{0}=1$.

**Proof outline.** Replace each count $x_i$ by that many dots and separate successive groups with $k-1$ bars. Reading the group sizes reverses this construction, so it is a [bijection](bijection.md) between [weak compositions of an integer](weak-composition-of-an-integer.md) and strings of $N$ dots and $k-1$ bars. Choose the bar positions among $N+k-1$ positions; the [binomial coefficient](binomial-coefficient-split.md) counts the choices. The beauty is that empty bins need no separate cases: end bars and adjacent bars encode them automatically.

If every bin must be nonempty, the [tuples](finite-tuple.md) are [compositions of an integer](composition-of-an-integer.md), and their count is $\binom{N-1}{k-1}$ for $N\geq k\geq1$; for $N<k$ there are none. Subtract one from every count, setting $y_i=x_i-1$. This is a [bijection](bijection.md) to [weak compositions of an integer](weak-composition-of-an-integer.md) of $N-k$, so [stars and bars](stars-and-bars-combinatorics.md) gives $\binom{(N-k)+k-1}{k-1}=\binom{N-1}{k-1}$. For five objects and three bins, this is $\binom42=6$, with the six positive [tuples](finite-tuple.md)

$$
(3,1,1),\ (1,3,1),\ (1,1,3),\ (2,2,1),\ (2,1,2),\ (1,2,2).
$$

For instance, $(2,1,2)$ shifts to $(1,0,1)$, whose [sum](sum.md) is $2=5-3$. Sorting the six positive [tuples](finite-tuple.md) collapses them to just two [integer partitions](integer-partition.md), $3+1+1$ and $2+2+1$. Thus named bins and unordered summands answer different questions.

[Stars and bars](stars-and-bars-combinatorics.md) is useful for allocating identical resources or enumerating [integer](integer-split.md) solutions without listing them individually. Prescribed lower bounds can be subtracted just like the nonempty-bin requirement. Upper bounds require removing forbidden [tuples](finite-tuple.md); the existing [bounded weak compositions](bounded-weak-compositions.md) article applies the [inclusion-exclusion principle](inclusion-exclusion-principle.md) to those violations.

**Table of contents**

- [Composition of an integer](composition-of-an-integer.md)
  - [Weak composition of an integer](weak-composition-of-an-integer.md)
- [Bounded weak compositions](bounded-weak-compositions.md)

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Dirichlet convolution](dirichlet-convolution.md)
