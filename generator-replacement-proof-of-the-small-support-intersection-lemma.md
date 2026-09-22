# Generator replacement proof of the small-support intersection lemma

↑ **Parent:** [Small-support generating lemma for extremal intersecting families](small-support-generating-lemma-for-extremal-intersecting-families.md)

Let $m$ be the smallest supporting prefix for a maximum [left-compressed set family](left-compressed-set-family.md) of $k$-sets that is [t-intersecting](t-intersecting-family.md), and set $N=n-m$. The [maximum-support generator fibre](maximum-support-generator-fibre.md) gives exclusive count $\binom N{k-a}$ for a size-$a$ generator containing $m$. By [tight pairs of left-compressed generators](tight-pairs-of-left-compressed-generators.md), only classes $a,b$ with $a+b=m+t$ can conflict after deleting $m$. For unequal such sizes, replacing both classes by the shortened generators of either class would imply

$$
\binom N{k-a+1}\binom N{k-b+1}\leq\binom N{k-a}\binom N{k-b}.
$$

When $n\geq2k-t+2$ and the classes have positive fibres, the reverse inequality is strict. For the remaining central class $a=t+j$, $m=t+2j$, some earlier coordinate is absent from at least $j/(m-1)$ of its shortened generators. Those generators are mutually t-intersecting. Replacing the central class by that subfamily has gain-to-loss ratio at least

$$
\frac{j}{m-1}\frac{N+1}{k-t-j+1},
$$

which exceeds one exactly when $n>(k-t+1)(2+(t-1)/j)$. This forces the support bound in the [small-support generating lemma for extremal intersecting families](small-support-generating-lemma-for-extremal-intersecting-families.md).

## ↑ Ancestors (9)

1. [Small-support generating lemma for extremal intersecting families](small-support-generating-lemma-for-extremal-intersecting-families.md)
2. [Generating family for a uniform set family](generating-family-for-a-uniform-set-family.md)
3. [Uniform set family](uniform-set-family.md)
4. [Set family](set-family.md)
5. [Extremal set theory](extremal-set-theory-split.md)
6. [Combinatorics](combinatorics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-13/2/solution.md)
