# North-east lattice path

↑ **Parent:** [Lattice path](lattice-path.md)

A [north-east lattice path](north-east-lattice-path.md) is a [lattice path](lattice-path.md) whose allowed steps are $E=(1,0)$ and $N=(0,1)$. From $(0,0)$ to $(a,b)$, with [nonnegative integers](natural-number.md) $a,b$, it has $a$ east steps and $b$ north steps. The number is

$$
\boxed{P(a,b)=\binom{a+b}{b}=\binom{a+b}{a}.}
$$

There is one zero-step [north-east lattice path](north-east-lattice-path.md) when $a=b=0$.[§1.2, Lattice Paths and Binomial Coefficients: encoding paths by step positions](discrete-mathematics-an-open-introduction-3rd-edition-by-oscar-levin.md)

**Seven positions, thirty-five paths.** To reach $(4,3)$, choose the three positions occupied by north steps in a seven-symbol word. For example, the [subset](subset.md) $\{2,4,7\}$ of $\{1,2,3,4,5,6,7\}$ gives `ENENEEN`: putting $N$ exactly in those positions and $E$ elsewhere reconstructs the [north-east lattice path](north-east-lattice-path.md). Reading the north-step positions recovers the [subset](subset.md), so these two operations give a [bijection](bijection.md). Hence

$$
P(4,3)=\binom73=\frac{7\cdot6\cdot5}{3\cdot2\cdot1}=35.
$$

The numerator counts ordered choices of three different positions; each [subset](subset.md) occurs in $3!=6$ orders. Dividing by this [factorial](factorial.md) counts each [north-east lattice path](north-east-lattice-path.md) once. A [binary string](binary-string.md) recording $N$ as $1$ and $E$ as $0$ gives the same example as `0101001`.

<a id="image-a-bijection-from-three-chosen-positions-to-a-north-east-lattice-path-and-the-recursive-grid-giving-p-4-3-35"></a>
![](north-east-path-positions-and-counts.png)

**[Figure 14](#image-a-bijection-from-three-chosen-positions-to-a-north-east-lattice-path-and-the-recursive-grid-giving-p-4-3-35). A bijection from three chosen positions to a north-east lattice path, and the recursive grid giving $P(4,3)=35$**. The original example `ENENEEN` reaches $(4,3)$. Both panels use east to the right and north upwards. The right panel counts all such [north-east lattice paths](north-east-lattice-path.md), rather than just the displayed one: twenty arrive with a final east step and fifteen with a final north step.

This interpretation is useful when arrangements have fixed totals but flexible order: a [subset](subset.md), a [binary string](binary-string.md), and a [north-east lattice path](north-east-lattice-path.md) become different views of one selection. It also separates endpoint restrictions from restrictions along the journey. Requiring the [lattice path](lattice-path.md) to avoid specified [points](point-geometry.md) changes the count; the unrestricted [binomial coefficient](binomial-coefficient-split.md) no longer suffices, but the local [north-east lattice path recurrence](north-east-lattice-path-recurrence.md) still suggests how to count allowed arrivals.

**Table of contents**

- [North-east lattice path recurrence](north-east-lattice-path-recurrence.md)

## ↑ Ancestors (5)

1. [Lattice path](lattice-path.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Lattice path](lattice-path.md)
- [North-east lattice path](north-east-lattice-path.md)
- [North-east lattice path recurrence](north-east-lattice-path-recurrence.md)
- [Pascal's rule](pascal-s-rule.md)
- [Pascal's triangle](pascal-s-triangle.md)
