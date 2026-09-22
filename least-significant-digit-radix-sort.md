# Least-significant-digit radix sort

↑ **Parent:** [Radix sort](radix-sort.md)

A least-significant-digit radix sort processes [numerical digits](numerical-digit.md) from smallest to largest [place value](place-value.md). Fix [integers](integer-split.md) $R\ge2$ and $d\ge1$, and take $n$ complete [sorting records](sorting-record.md) whose [sort keys](sort-key.md) satisfy $0\le k<R^d$. Use exactly $d$ positions in [positional notation](positional-notation.md) with [radix](radix.md) $R$, including leading zeros. At pass $j=0,\ldots,d-1$, apply a [stable digit sort](stable-digit-sort.md) to the current [array](array-data-structure.md) using

$$
\delta_j(k)=\left\lfloor\frac{k}{R^j}\right\rfloor\bmod R.
$$

The [floor function](floor-function.md) selects the integer [quotient](quotient.md), and the [remainder](remainder.md) selects the current [numerical digit](numerical-digit.md). Move the complete [sorting record](sorting-record.md), including its associated data. There are exactly $d$ passes, so this procedure terminates even for an empty [array](array-data-structure.md). The [radix sort suffix invariant](radix-sort-suffix-invariant.md) supplies its [algorithm correctness](algorithm-correctness.md) argument.

For an original [input](input-computer-science.md), let the letters identify the attached data:

$$
(314_A,027_B,305_C,042_D,217_E,005_F,127_G,040_H).
$$

Here $R=10$, $d=3$, and leading zeros only align [place values](place-value.md); $005$ represents the [integer](integer-split.md) five. The exact pass ledger is:

$$
\begin{array}{c|llllllll}
\text{input}&314_A&027_B&305_C&042_D&217_E&005_F&127_G&040_H\\
\text{units}&040_H&042_D&314_A&305_C&005_F&027_B&217_E&127_G\\
\text{tens}&305_C&005_F&314_A&217_E&027_B&127_G&040_H&042_D\\
\text{hundreds}&005_F&027_B&040_H&042_D&127_G&217_E&305_C&314_A
\end{array}
$$

After the units pass, the [numerical digits](numerical-digit.md) are $0,2,4,5,5,7,7,7$. The ties retain $C$ before $F$ and $B$ before $E$ before $G$. This [array](array-data-structure.md) is not yet ordered by its whole [integer](integer-split.md) [sort keys](sort-key.md): $314$ still precedes $305$. After the tens pass, the two-position suffixes are $05,05,14,17,27,27,40,42$. In particular, $217_E$ now precedes $027_B$: their tens [numerical digits](numerical-digit.md) differ, so [stable sorting](stable-sorting.md) does not require retaining their previous order. The hundreds pass produces the final [sorted array](sorted-array.md), with all attached letters preserved.

<a id="image-three-stable-digit-passes-order-successively-longer-suffixes"></a>
![](radix-sort-stable-digit-pass-ledger.png)

**[Figure 22](#image-three-stable-digit-passes-order-successively-longer-suffixes). Three stable digit passes order successively longer suffixes**. Original decimal [radix sort](radix-sort.md) ledger. Each card carries an unchanged record label. Orange marks the [numerical digit](numerical-digit.md) read in the current pass; green marks lower positions already processed. The suffix row beneath each pass shows precisely what is ordered, rather than claiming whole-key [sortedness](sortedness.md) early.

**Table of contents**

- [Radix sort suffix invariant](radix-sort-suffix-invariant.md)

## ↑ Ancestors (5)

1. [Radix sort](radix-sort.md)
2. [Sorting algorithm](sorting-algorithm.md)
3. [Algorithm](algorithm-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Stable digit sort](stable-digit-sort.md)
