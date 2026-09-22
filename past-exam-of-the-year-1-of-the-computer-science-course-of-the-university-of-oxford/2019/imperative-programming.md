# Imperative programming

↑ **Parent:** [2019](../2019.md)

Source paper: [released examination archive, member 2018/T/a10098w1.pdf](https://www.whatdotheyknow.com/request/ba_computer_science_past_papers/response/2577745/attach/2/202402%20183%20CS%20Papers.zip?cookie_passthrough=1). The original cover identifies the Trinity Term examination of Wednesday 19 June 2019; the archive directory does not determine its year. All eight questions are covered. Code uses [Scala](../../programming-language.md#scala) 2 syntax.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [i](#3/d/i)
      - [Solution](#3/d/i/solution)
    - [ii](#3/d/ii)
      - [Solution](#3/d/ii/solution)
    - [iii](#3/d/iii)
      - [Solution](#3/d/iii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
    - [iii](#5/b/iii)
      - [Solution](#5/b/iii/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)
  - [e](#6/e)
    - [Solution](#6/e/solution)
  - [f](#6/f)
    - [Solution](#6/f/solution)
  - [g](#6/g)
    - [Solution](#6/g/solution)
- [7](#7)
  - [a](#7/a)
    - [i](#7/a/i)
      - [Solution](#7/a/i/solution)
    - [ii](#7/a/ii)
      - [Solution](#7/a/ii/solution)
  - [b](#7/b)
    - [i](#7/b/i)
      - [Solution](#7/b/i/solution)
    - [ii](#7/b/ii)
      - [Solution](#7/b/ii/solution)
  - [c](#7/c)
    - [i](#7/c/i)
      - [Solution](#7/c/i/solution)
    - [ii](#7/c/ii)
      - [Solution](#7/c/ii/solution)
  - [d](#7/d)
    - [Solution](#7/d/solution)
- [8](#8)
  - [a](#8/a)
    - [Solution](#8/a/solution)
  - [b](#8/b)
    - [Solution](#8/b/solution)
  - [c](#8/c)
    - [Solution](#8/c/solution)
  - [d](#8/d)
    - [Solution](#8/d/solution)

## 1

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Accumulate the prefix by [Horner's method](../../polynomial.md#horner-s-method) in base two. `digit-'0'` converts either permitted digit to its numerical value:
```
var i = 0
var integerPart = 0.0
while (i < bin.length && bin(i) != '.') {
  integerPart = 2.0 * integerPart + (bin(i) - '0')
  i += 1
}
```
The [loop invariant](../../algorithm.md#loop-invariant), in exact arithmetic, is that `i` is the number of processed digits before the point and

$$
integerPart=\sum_{j=0}^{i-1}(bin(j)-\mathtt{'0'})2^{i-1-j}.
$$

Appending a digit shifts the old positional value by one binary place and adds that digit, which proves preservation. The [loop variant](../../algorithm.md#loop-variant) is $bin.length-i$. At exit, `i` is the binary-point index or the length if no point occurs, and **`integerPart` is the value of the [integer](../../integer.md) prefix**. An empty prefix contributes zero. There is one multiplication per processed digit, with no separate powers or repeated divisions. [Short-circuit evaluation](../../programming-language.md#short-circuit-evaluation) prevents an out-of-range access when the point is absent.

For `Double`, this exact-arithmetic [invariant](../../mathematics.md#invariant-mathematics) describes the intended value; the operational value is the rounded Horner recurrence. Very long prefixes can lose precision or overflow, as discussed in part (g). A fixed-width return type cannot represent every finite binary digit [string](../../foundations-of-mathematics.md#string) exactly.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let `point` be the known point index. Work backwards so that each step uses just one division, rather than separately computing positional weights:
```
var j = bin.length - 1
var fractionalPart = 0.0
while (j > point) {
  fractionalPart = (fractionalPart + (bin(j) - '0')) / 2.0
  j -= 1
}
```
The [loop invariant](../../algorithm.md#loop-invariant), under exact arithmetic, is

$$
fractionalPart=\sum_{t=j+1}^{bin.length-1}(bin(t)-\mathtt{'0'})2^{j-t}.
$$

Initially the suffix is empty. Incorporating digit $j$ and dividing by two gives exactly the same formula with $j$ replaced by $j-1$. At exit $j=point$, **the result is $\sum_{t>point}(bin(t)-\mathtt{'0'})2^{point-t}$**. The [loop variant](../../algorithm.md#loop-variant) is $j-point$ when a point exists. If a no-point input is handled by setting `point=bin.length`, the loop is skipped and the fractional contribution is zero; $\max(0,j-point)$ is a [loop variant](../../algorithm.md#loop-variant) covering that convention too. Trailing zeroes and an empty fractional suffix require no special arithmetic. [Floating-point rounding](../../floating-point-arithmetic.md#floating-point-rounding) qualifies the exact formula for long inputs.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Represent zero by one digit. Since `int_part` is nonnegative, a logical right shift is exactly [integer division](../../arithmetic.md#integer-division) by two:
```
var digits = 1
var scratch = int_part
while (scratch >= 2) {
  scratch = scratch >>> 1
  digits += 1
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $digits\geq1$ and $scratch=\lfloor int\_part/2^{digits-1}\rfloor$; for positive `int_part`, also $scratch\geq1$. The [loop variant](../../algorithm.md#loop-variant) is `scratch`, strictly decreased whenever the guard holds. On exit, a positive input has $scratch=1$, yielding $2^{digits-1}\leq int\_part<2^{digits}$. Therefore **`digits` is the required width**, including width one for zero. Shifting avoids an explicit multiplication or division in the code. This uses the supplied assumption that `dec.toInt` really is the mathematical floor; saturating or invalid conversions are not covered by that assumption.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Extract low bits and fill the [integer](../../integer.md) positions from right to left:
```
var remaining = int_part
var pos = digits - 1
while (pos >= 0) {
  res(pos) = if ((remaining & 1) == 0) '0' else '1'
  remaining = remaining >>> 1
  pos -= 1
}
```
At the start of an iteration, the [loop invariant](../../algorithm.md#loop-invariant) says that positions $pos+1,\ldots,digits-1$ contain the correct low bits and

$$
int\_part=remaining\,2^{digits-1-pos}
+\sum_{t=pos+1}^{digits-1}(res(t)-\mathtt{'0'})2^{digits-1-t}.
$$

The bitwise AND extracts the remainder modulo two; the shift supplies its quotient. These two facts preserve the [loop invariant](../../algorithm.md#loop-invariant). The [loop variant](../../algorithm.md#loop-variant) is $pos+1$. The width established in part (c) ensures that `remaining` is zero at exit, so **the first `digits` entries encode the whole [integer](../../integer.md) part**. For zero the single entry becomes `'0'`. There are no explicit multiplications or divisions, and no extra digit [array](../../data-structure.md#array-data-structure) is needed.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Generate the fractional bits by repeated doubling, keeping only the unconverted residual:
```
res(digits) = '.'
var fraction = dec - int_part.toDouble
var out = digits + 1
while (out < res.length) {
  fraction = 2.0 * fraction
  if (fraction >= 1.0) {
    res(out) = '1'
    fraction -= 1.0
  } else res(out) = '0'
  out += 1
}
```
Let $f_0=dec-int\_part$ and $k=out-digits-1$. The [loop invariant](../../algorithm.md#loop-invariant) is $0\leq fraction<1$, the first $k$ fractional digits have been written, and, in exact arithmetic,

$$
f_0=\sum_{t=1}^{k}(res(digits+t)-\mathtt{'0'})2^{-t}+fraction\,2^{-k}.
$$

Doubling exposes the next digit, and subtracting that digit leaves the next residual in $[0,1)$. This proves preservation. The [loop variant](../../algorithm.md#loop-variant) is $res.length-out$. The loop fills the whole suffix, even when the residual has become zero; subsequent bits are zero. There is one multiplication per output bit. With $F=res.length-digits-1$ fractional positions, **the result is truncated, with exact-arithmetic error $0\leq dec-value(res)<2^{-F}$**. An [integer](../../integer.md) has an all-zero suffix. No rounding-up step is performed.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

[Equivalence partitioning](../../computer-science.md#equivalence-partitioning) divides the input domain into classes expected to exercise the same relevant behavior, then chooses representatives and boundary cases from each class. It is a way to select tests, not a proof that every member of a class must behave identically in a faulty implementation.

Useful classes for this parser include [integer](../../integer.md)-only inputs, a leading point, a trailing point, and digits on both sides; all-zero inputs and inputs containing ones; leading or trailing zeroes; one-digit and longer blocks; and large [integer](../../integer.md) or tiny fractional magnitudes near [floating-point rounding](../../floating-point-arithmetic.md#floating-point-rounding), [floating-point overflow](../../floating-point-arithmetic.md#floating-point-overflow) and [floating-point underflow](../../floating-point-arithmetic.md#floating-point-underflow) boundaries. For instance, compare `'1'`, `'1.'`, `'.1'`, `'1.1'`, `'0001.1000'`, and digit [strings](../../foundations-of-mathematics.md#string) just beyond the exact [integer](../../integer.md) precision of `Double`. Empty digit blocks have the zero convention used above. If a surrounding validator rejects an entirely empty representation or a bare point, test those as separate invalid-format classes. Unexpected digits and multiple points are likewise validator tests, since the conversion fragments assume well-formed input. **Include representatives with independently calculated positional values**, rather than relying only on inverse conversion.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

The first proposed identity can fail even without numerical error because [binary fractions](../../arithmetic.md#binary-fraction) have nonunique textual representations. Leading zeroes, optional points and trailing fractional zeroes are normalized differently by a fixed-width output convention. It also fails if the input has more significant bits than `Double` can preserve, more fractional places than the output buffer can hold, an [integer](../../integer.md) part outside the assumed `Int` range, or a value that overflows or underflows during decoding. [Array](../../data-structure.md#array-data-structure) identity here must mean equal contents: a newly allocated [Scala](../../programming-language.md#scala) [array](../../data-structure.md#array-data-structure) is a different [software object](../../programming-language.md#software-object), so use `sameElements` rather than reference equality for a content test.

The second identity fails when the stored fractional precision truncates a nonzero bit; **with two fractional places, $0.125$ becomes zero**. It can also fail outside the finite nonnegative input and [integer](../../integer.md)-conversion assumptions. Within those assumptions, enough fractional positions to encode the finite `Double` exactly can permit the round trip, but an arbitrary fixed small width does not guarantee it. Every finite `Double` has a finite [binary expansion](../../arithmetic.md#binary-expansion); saying that a decimal-looking `Double` necessarily has an infinite binary expansion would confuse the represented number with an exact decimal real.

The source's introductory example is internally inconsistent: the displayed digit [string](../../foundations-of-mathematics.md#string) has value $22+1/4+1/32=22.28125$, whereas its shortened character [array](../../data-structure.md#array-data-structure) encodes $22+1/4+1/16=22.3125$. The conversion rules above follow the actual input digits. **[Round-trip testing](../../computer-science.md#round-trip-testing) needs an independent value oracle as well as the two compositions**, because two mutually consistent but incorrect routines can conceal each other's errors.

## 2

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Compare values directly, avoiding subtraction that could overflow:
```
def bestIndex(l: Int, r: Int): Int = {
  require(0 <= l && l < r && r <= a.length)
  val first = l
  val middle = l + (r - l) / 2
  val last = r - 1
  if (a(first) <= a(middle)) {
    if (a(middle) <= a(last)) middle
    else if (a(first) <= a(last)) last
    else first
  } else {
    if (a(first) <= a(last)) first
    else if (a(middle) <= a(last)) last
    else middle
  }
}
```
Each branch returns an index whose value lies between the other two sampled values. Non-strict comparisons make ties harmless. **The [precondition](../../algorithm.md#precondition) is a nonempty valid segment**, not a segment of at least three elements: for lengths one or two some sample indices coincide, but the code still returns a valid median of the sampled triple. This matters because selection can reach a two-element segment. With three distinct sample values, the pivot is not the minimum or maximum of the whole segment, but it need not be near the segment's true median. [Median-of-three pivot selection](../../algorithm.md#median-of-three-pivot-selection) is a heuristic, not a balance guarantee.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Set aside the selected pivot at the end, [array partitioning](../../algorithm.md#two-way-array-partition) the other entries, then move the pivot to the separation index:
```
def partition(l: Int, r: Int): Int = {
  require(0 <= l && l < r && r <= a.length)
  def swap(i: Int, j: Int): Unit = {
    val t = a(i); a(i) = a(j); a(j) = t
  }
  val chosen = bestIndex(l, r)
  val x = a(chosen)
  swap(chosen, r - 1)
  var p = l
  var j = l
  while (j < r - 1) {
    if (a(j) < x) {
      swap(p, j)
      p += 1
    }
    j += 1
  }
  swap(p, r - 1)
  p
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $l\leq p\leq j\leq r-1$, $a[l,p)<x$, $a[p,j)\geq x$, and $a(r-1)=x$. The segment's [multiset](../../set.md#multiset) is unchanged and all entries outside it are unchanged. A low entry is swapped into the low segment; a high entry simply extends the high segment. The [loop variant](../../algorithm.md#loop-variant) is $r-1-j$. At exit, exchanging the reserved pivot with `a(p)` gives **$a[l,p)<x$, $a(p)=x$, and $a[p+1,r)\geq x$**. The displaced value at the old pivot position was already at least $x$. Length one is handled by self-swaps and an empty loop. Duplicate pivot values belong to the high side. This costs $\Theta(r-l)$ time and $O(1)$ auxiliary space.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Ranks are relative to the current segment. The pivot's rank is `p-l`, not its absolute index:
```
def select(k: Int, l: Int, r: Int): Int = {
  require(0 <= l && l < r && r <= a.length)
  require(0 <= k && k < r - l)
  if (r - l == 1) a(l)
  else {
    val p = partition(l, r)
    val rank = p - l
    if (k == rank) a(p)
    else if (k < rank) select(k, l, p)
    else select(k - rank - 1, p + 1, r)
  }
}
```
The [array partitioning](../../algorithm.md#two-way-array-partition) places exactly `rank` strictly smaller entries before the pivot, with all later entries at least the pivot. Thus the pivot is the element of sorted rank `rank`, even when equal values occur later. A requested earlier rank is unchanged in the left segment; a later rank loses the low entries and the pivot, accounting for the subtraction `rank+1`. The recursive segment is nonempty in either branch that takes it, and its length strictly decreases. [Induction](../../foundations-of-mathematics.md#mathematical-induction) on segment length therefore proves **the returned value is the requested [order statistic](../../probability-theory.md#order-statistic)**, with at most one recursive call. Only the selected segment is permuted; all outside entries remain unchanged. This is [Quickselect](../../algorithm.md#quickselect).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Replace the tail call by updates to local bounds and a local rank:
```
def selectIterative(k: Int, l: Int, r: Int): Int = {
  require(0 <= l && l < r && r <= a.length)
  require(0 <= k && k < r - l)
  var low = l
  var high = r
  var rank = k
  while (high - low > 1) {
    val p = partition(low, high)
    val pivotRank = p - low
    if (rank == pivotRank) return a(p)
    if (rank < pivotRank) high = p
    else {
      rank -= pivotRank + 1
      low = p + 1
    }
  }
  a(low)
}
```
The [loop invariant](../../algorithm.md#loop-invariant) says that $l\leq low<high\leq r$, $0\leq rank<high-low$, and selecting rank `rank` in the active segment yields the originally requested [order statistic](../../probability-theory.md#order-statistic). The original segment's [multiset](../../set.md#multiset) is preserved, and outside it no entries change. The updates are exactly the recursive reductions proved in part (c). The [loop variant](../../algorithm.md#loop-variant) is $high-low$; a non-returning iteration strictly decreases it. A one-entry segment has only rank zero, establishing the final return. **Auxiliary space is $O(1)$**, rather than a potentially deep [call stack](../../data-structure.md#call-stack).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Test singleton and two-element segments, first/last/interior requested ranks, nonzero segment offsets, already sorted and reversed inputs, random inputs, all-equal inputs and several patterns of duplicates. Include `Int.MinValue` and `Int.MaxValue` to expose overflow-prone comparisons. An independent sorted copy supplies the value oracle; also check preservation of the segment's [multiset](../../set.md#multiset) and of all outside entries. For speed tests, increase segment size and include deliberately unfavorable pivot arrangements, rather than timing random inputs alone.

**Distinct entries do not guarantee linear worst-case time: the worst case is $\Theta(N^2)$.** A median of three can repeatedly be the second-smallest remaining value, leaving a segment of size $N-2$ when seeking its maximum. The [quadratic median-of-three selection family](../../algorithm.md#quadratic-median-of-three-selection-family) gives explicit distinct inputs realizing this behavior for the implementation above; one six-entry member is $[1,4,3,0,2,5]$. Its recurrence is $T(N)=T(N-2)+\Theta(N)$, yielding a quadratic sum. Balanced reductions instead give $T(N)=T(N/2)+\Theta(N)=\Theta(N)$. Randomized or suitable average-case analyses give expected linear selection, but this deterministic heuristic alone supplies no such worst-case guarantee. Unlike [Quicksort](../../algorithm.md#quicksort), [Quickselect](../../algorithm.md#quickselect) explores only one side, so a balanced run is linear rather than $\Theta(N\log N)$.

## 3

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

The first three subtractions are negative or return the already-seen zero, so addition is used. The fourth subtraction gives a new positive two; the next subtraction is negative. Thus **$r(1),\ldots,r(5)=1,3,6,2,7$**. These are the initial terms of [Recamán's sequence](../../sequence-and-series.md#recaman-s-sequence).[Initial terms, offset zero](../../mathematics-bibliography.md#oeis-entry-a005132)

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Use the already-filled prefix itself for membership tests. `Long` intermediates avoid overflow in the candidate calculations, while a checked conversion respects the required output type:
```
def recaman(a: Array[Int]): Unit = {
  if (a.length == 0) return
  a(0) = 0
  var i = 1
  while (i < a.length) {
    val candidate = a(i - 1).toLong - i.toLong
    var j = 0
    while (candidate > 0L && j < i && a(j).toLong != candidate) {
      j += 1
    }
    val next =
      if (candidate > 0L && j == i) candidate
      else a(i - 1).toLong + i.toLong
    require(next <= Int.MaxValue.toLong, "Sequence value exceeds Int")
    a(i) = next.toInt
    i += 1
  }
}
```
The outer [loop invariant](../../algorithm.md#loop-invariant) is $1\leq i\leq a.length$ and $a(t)=r(t)$ for $0\leq t<i$. The inner [loop invariant](../../algorithm.md#loop-invariant) says that $0\leq j\leq i$ and no processed entry before `j` equals the positive candidate. Its guard either reaches the end of the prefix, finds the candidate, or immediately rejects a nonpositive candidate. Its [loop variant](../../algorithm.md#loop-variant) is $i-j$. This establishes exactly the choice required by the recurrence, so the outer [loop invariant](../../algorithm.md#loop-invariant) is preserved. The outer [loop variant](../../algorithm.md#loop-variant) is $a.length-i$.

**Extra storage is $O(1)$** beyond the supplied result [array](../../data-structure.md#array-data-structure). Membership scans give an $O(N^2)$ upper bound for $N$ output entries. Addition, unlike the subtraction branch, is not required to avoid repeats: at indices $20$ and $24$ the value $42$ occurs twice. The code therefore does not try to enforce global distinctness. If an exact value eventually exceeds `Int`, the output interface cannot hold it; the check reports that limitation rather than wrapping the recurrence.

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

Regardless of which branch is taken, $r(n)\leq r(n-1)+n$. Starting from zero and applying [induction](../../foundations-of-mathematics.md#mathematical-induction) gives

$$
\boxed{0\leq r(n)\leq\sum_{i=1}^{n}i=\frac{n(n+1)}2.}
$$

For the inductive step, add $n$ to the bound $(n-1)n/2$ for the previous value. The subtraction branch gives an even smaller result, and positivity is checked there. This bound need not describe the actual growth sharply; it is sufficient to size a finite membership representation for a requested prefix.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $S_0$ denote the entry state. A conventional meaning for the Boolean returned by `add` is whether the call changes the [set](../../set.md):
```
// add(elem):
//   S' = S0 union {elem}
//   result == !S0.contains(elem)

// contains(elem):
//   S' = S0
//   result == S0.contains(elem)

// size:
//   S' = S0
//   result == cardinality(S0)
```
Initially $S=\varnothing$. In particular, re-adding an existing element returns false and does not increase the size. **All operations have the stated empty [precondition](../../algorithm.md#precondition)** at the abstract level. The comment that `add` adds an element does not itself completely specify its Boolean result; the explicit changed/not-changed convention above completes that contract. As with any `Int`-valued size operation, exact cardinalities are understood to be representable by that result type.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Represent the characteristic values of a bounded universe by one Boolean slot per possible member, a Boolean-[array](../../data-structure.md#array-data-structure) form of a [bitset](../../data-structure.md#bitset):
```
class BitMapSet(val MAXVALUE: Int) extends IntSet {
  require(MAXVALUE >= 0)
  private val bits = Array.fill(MAXVALUE)(false)
  private var count = 0

  def contains(elem: Int): Boolean =
    0 <= elem && elem < MAXVALUE && bits(elem)

  def add(elem: Int): Boolean = {
    require(0 <= elem && elem < MAXVALUE, "Outside bitmap universe")
    if (bits(elem)) false
    else {
      bits(elem) = true
      count += 1
      true
    }
  }

  def size: Int = count
}
```
The [abstraction function](../../computer-science.md#abstraction-function) is $\alpha(bits,count)=\{x:0\leq x<MAXVALUE,\ bits(x)\}$. The [representation invariant](../../computer-science.md#representation-invariant) is that `bits.length==MAXVALUE`, its entries are Boolean, and `count` equals the number of true entries. Initialization gives the empty [set](../../set.md); changing a false entry to true adds exactly its index and increments the count once. A repeated addition preserves both. All three operations have $O(1)$ [time complexity](../../theoretical-computer-science.md#time-complexity) after initialization; storage and explicit [array](../../data-structure.md#array-data-structure) initialization are $\Theta(MAXVALUE)$.

**The constructor requires $MAXVALUE\geq0$, and `add` requires $0\leq elem<MAXVALUE$.** `contains` remains total by returning false outside the representable universe; [short-circuit evaluation](../../programming-language.md#short-circuit-evaluation) protects the index. This finite representation cannot implement unrestricted addition of every `Int` while preserving the abstract contract. Its strengthened `add` [precondition](../../algorithm.md#precondition) therefore makes it a restricted implementation, not a behaviorally substitutable implementation of the unrestricted trait for arbitrary clients. The [sequence](../../sequence-and-series.md#sequence) client below proves that it stays within the restricted universe.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/i">i</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/i/solution">Solution</h5>

↑ **Parent:** [I](#3/d/i)

For $N$ result entries the largest required index is $N-1$, so the bound in part (a)(iii) permits universe size $M=N(N-1)/2+1$. Check that the chosen universe can itself be expressed as an [array](../../data-structure.md#array-data-structure) length:
```
def recamanBitmap(a: Array[Int]): Unit = {
  val n = a.length
  if (n == 0) return
  val capacity = n.toLong * (n.toLong - 1L) / 2L + 1L
  require(capacity <= Int.MaxValue.toLong, "Bitmap universe too large")
  val seen = new BitMapSet(capacity.toInt)
  a(0) = 0
  seen.add(0)
  var i = 1
  while (i < n) {
    val candidate = a(i - 1).toLong - i.toLong
    val next =
      if (candidate > 0L && !seen.contains(candidate.toInt)) candidate
      else a(i - 1).toLong + i.toLong
    a(i) = next.toInt
    seen.add(a(i))
    i += 1
  }
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is that the result prefix contains exactly $r(0),\ldots,r(i-1)$ and the [abstraction function](../../computer-science.md#abstraction-function) of `seen` is their [set](../../set.md) of values. The universe bound ensures that each positive candidate being queried and each actual next value is less than `capacity`; values are nonnegative. Thus the conversions and the restricted `add` [precondition](../../algorithm.md#precondition) are justified, rather than merely hoped to succeed. At a repeated addition, `add` returning false is harmless: the set of previously seen values is still updated correctly. The [loop variant](../../algorithm.md#loop-variant) is $n-i$. **At return every result entry agrees with the original recurrence.**

<h4 id="3/d/ii">ii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/d/ii)

The original routine uses $O(1)$ auxiliary space and at most $O(N^2)$ membership work. A bitmap with universe size $M$ uses **$\Theta(M)$ extra storage and $\Theta(N)$ work in the [sequence](../../sequence-and-series.md#sequence)-generation loop** because membership and insertion each take constant time. Here the safe universal bound chooses $M=N(N-1)/2+1$, so extra storage is $\Theta(N^2)$ for growing $N$.

Initialization must be accounted for separately: creating and clearing a Boolean [array](../../data-structure.md#array-data-structure) of length $M$ takes $\Theta(M)$ work in the usual [array](../../data-structure.md#array-data-structure)-initialization model. Consequently **the complete one-shot routine takes $\Theta(M+N)$**, which is $\Theta(N^2)$ with this conservative universe bound. The faster lookup does not make that quadratic setup disappear. If the bitmap is already initialized, or the analysis explicitly charges only the generation phase, the remaining phase is linear. A tighter known bound on values can reduce the universe cost, but no unproved growth bound is needed here.

<h4 id="3/d/iii">iii</h4>

↑ **Parent:** [D](#3/d)

<h5 id="3/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/d/iii)

A fixed [array](../../data-structure.md#array-data-structure) containing the distinct seen [integers](../../integer.md) needs capacity at most $N$, because at most one new distinct value is introduced per result entry. Its auxiliary space is therefore **$O(N)$**, rather than the bitmap's $O(M)$ universe storage. A size field identifies the occupied prefix; insertion first checks membership, and appends only when absent.

An unsorted occupied prefix needs linear membership scans, giving **$O(N^2)$ total work** by the same summation as in the original version. Keeping it sorted permits [binary search](../../algorithm.md#binary-search) membership in $O(\log N)$, but inserting a new value can shift $O(N)$ entries, so the overall worst-case upper bound remains quadratic. Unlike a bitmap, the space cost depends on the number of stored values rather than their largest possible numerical magnitude. Compared with part (a)(ii), this extra set [array](../../data-structure.md#array-data-structure) also duplicates information already present in the output prefix; its principal benefit is a separate set interface, not an automatic asymptotic speedup.

## 4

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Check entries against their own indices, stopping on the first mismatch:
```
def isIdentity: Boolean = {
  var i = 0
  while (i < game.length && game(i) == i) {
    i += 1
  }
  i == game.length
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $0\leq i\leq game.length$ and $game(j)=j$ for every $j<i$. The [loop variant](../../algorithm.md#loop-variant) is $game.length-i$. A false guard means either every position has passed or the next position is wrong, so **the returned Boolean is true exactly for the identity [permutation](../../combinatorics.md#permutation)**. Neither the game nor its history is changed. [Short-circuit evaluation](../../programming-language.md#short-circuit-evaluation) protects the final indexed comparison.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Allocate a distinct game and copy every destination entry from the corresponding source position:
```
def flip(k: Int): Flip = {
  require(1 < k && k <= game.length)
  val result = new Flip(game.length)
  var i = 0
  while (i < game.length) {
    val source = if (i < k) k - 1 - i else i
    result.game(i) = game(source)
    i += 1
  }
  result.flips = k :: flips
  result
}
```
The [loop invariant](../../algorithm.md#loop-invariant) says that the receiver is unchanged and destination positions before `i` equal the reversal of the first $k$ source entries followed by the untouched suffix. The [loop variant](../../algorithm.md#loop-variant) is $game.length-i$. At exit the copying is complete. Reversal is a bijection on positions, so the destination remains a [permutation](../../combinatorics.md#permutation). **The returned object's [array](../../data-structure.md#array-data-structure) is independent of the receiver's [array](../../data-structure.md#array-data-structure)**, while the immutable tail of its history [list](../../data-structure.md#list-abstract-data-type) can safely be shared. The source's only supplied constructor randomizes the new [array](../../data-structure.md#array-data-structure) before the copy; that work is redundant but does not affect correctness. An additional private constructor could avoid it without changing the required result.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The history is built by prepending, so reverse it when displaying chronological moves:
```
override def toString: String =
  game.mkString("[", ", ", "]") +
    "    history of flips: " + flips.reverse.toString
```
Thus a reverse-stored history `[3,2,4]` is displayed as **`List(4, 2, 3)`**. The initial empty history remains `List()`. Neither traversal mutates the game or the immutable history. Displaying the stored list without reversing it would describe the moves backwards.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Use [breadth-first search](../../tree-graph-theory.md#breadth-first-search) with the supplied [FIFO queue](../../data-structure.md#fifo-queue), taking one edge to mean one permitted [prefix reversal](../../combinatorics.md#prefix-reversal):
```
def solve(puzzle: Flip): Flip = {
  val pending = scala.collection.mutable.Queue[Flip]()
  pending.enqueue(puzzle)
  while (!pending.isEmpty) {
    val current = pending.dequeue()
    if (current.isIdentity) return current
    var k = 2L
    while (k <= current.game.length.toLong) {
      pending.enqueue(current.flip(k.toInt))
      k += 1L
    }
  }
  throw new IllegalStateException("No solution")
}

val puzzle = new Flip(n)
println("Solving:")
println(puzzle)
val answer = solve(puzzle)
println("Solved:")
println(answer)
```
The [FIFO queue](../../data-structure.md#fifo-queue) holds pending paths in nondecreasing history length. Initially it holds only the zero-move path. Removing a path at depth $d$ and appending its children at depth $d+1$ preserves that order. The inner [loop invariant](../../algorithm.md#loop-invariant) says that precisely moves $2,\ldots,k-1$ of the removed state have been appended; its [loop variant](../../algorithm.md#loop-variant) is $n-k+1$ while the guard holds. The first identity state removed therefore has **the minimum possible number of moves**. A [stack](../../data-structure.md#stack-data-structure)-based [depth-first search](../../algorithm.md#depth-first-search) does not generally have that property.

Termination does not rely on avoiding repeats in this first version. Every [permutation](../../combinatorics.md#permutation) can be sorted by [prefix reversal sorting](../../algorithm.md#prefix-reversal-sorting): place the largest misplaced value at the front if necessary, flip it into its final position, and repeat on the shorter prefix. This constructs a route of at most $2(n-1)$ moves. Each search depth has finitely many paths, with at most $n-1$ children per path, so [breadth-first search](../../tree-graph-theory.md#breadth-first-search) reaches some solution depth after finitely many expansions. This gives a finite bound on remaining expansions before the first solution even though the repeated-state path tree is infinite. The one-element game is already solved. Repeated paths can nevertheless make time and storage enormous; part (e) removes that waste.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Give each solving session a shared visited [set](../../set.md) keyed by immutable snapshots of [permutation](../../combinatorics.md#permutation) contents, for example `game.toList`, and insert the initial snapshot immediately. Have all successor objects refer to that same session's set. The refined `flip` first constructs the candidate state; if its key is present, return `None`. Otherwise add the key immediately and return `Some(candidate)`. The search enqueues only `Some` results. Keys must compare contents rather than [array](../../data-structure.md#array-data-structure) identities, and a fresh solving session must start with a fresh visited set.

Marking at generation time prevents the same state from being queued repeatedly, including the immediate cycle made by applying the same reversal twice. **First discovery in [breadth-first search](../../tree-graph-theory.md#breadth-first-search) already has minimum depth**, so discarding later discoveries cannot remove a shorter solution. The graph now has at most $n!$ admitted states. If only cycles along one path were to be rejected, a path-local set would suffice, but it would still repeat states reached by different paths; the shared session-wide set avoids both kinds of repetition. Public game fields must not be externally mutated while their states are being searched.

## 5

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The abstract state is a finite [multiset](../../set.md#multiset) $Q$ of ordered values, initially empty. Multiplicity matters: deleting the minimum removes one occurrence, not every equal occurrence. Assume a consistent [total order](../../set.md#total-order) on `T`.
```
trait PriorityQueue[T] {
  // Pre: true. Post: Q' is the empty multiset.
  def clear(): Unit

  // Pre: true. Post: Q' = Q with one additional occurrence of x.
  def insert(x: T): Unit

  // Pre: Q is nonempty.
  // Post: result is a minimum of Q;
  //       Q' is Q with exactly one occurrence of result removed.
  def delMin(): T

  // Pre: true. Post: result iff Q is empty, and Q' = Q.
  def isEmpty(): Boolean
}
```
This [abstract data type](../../computer-science.md#abstract-data-type) places no fixed-capacity bound on insertion. **The only operation requiring a nonempty collection is `delMin`**. The representation must preserve duplicates even if it uses a [data structure](../../data-structure.md) commonly associated with [sets](../../set.md).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

**Yes, provided balancing guarantees logarithmic height.** In a suitably maintained [balanced binary tree](../../data-structure.md#balanced-binary-tree) of height $O(\log(n+1))$, insertion searches one root-to-leaf path and deletion of the minimum follows the leftmost path. Reconnecting the tree and performing the required rebalancing also costs at most a constant amount per level for the standard logarithmic-time schemes. Thus both operations take $O(\log(n+1))$ time, conventionally written $O(\log n)$ for nontrivial sizes. Merely calling a tree approximately balanced would not prove that height bound; it is the balancing guarantee that matters. Without it, a [binary search tree](../../data-structure.md#binary-search-tree) can have linear height.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

**Not automatically: the duplicate-value policy must implement a [multiset](../../set.md#multiset).** A strict [binary search tree](../../data-structure.md#binary-search-tree) storing one entry per distinct key represents a [set](../../set.md); inserting a second equal value then loses a required occurrence. A fixed rule that puts all equal values on one side also needs care, because ordinary balancing rotations need not preserve that one-sided equality rule.

One valid refinement stores a multiplicity at each distinct key. Inserting an equal key increments its count; `delMin` decrements the minimum key's count and removes that node only at zero. Alternatively, use distinct internal keys such as `(value, uniqueSerial)` while ordering primarily by value and returning only the value. With an appropriate balanced representation either approach preserves every occurrence and the required operation bounds. A bare claim about balanced search trees, with no treatment of duplicates, does not establish the abstract specification.

<h4 id="5/b/iii">iii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/b/iii)

A minimum-oriented [binary heap](../../data-structure.md#binary-heap) is an appropriate alternative. Store a complete [binary tree](../../data-structure.md#binary-tree) in an [array](../../data-structure.md#array-data-structure) and maintain [heap order](../../data-structure.md#heap-order). Insertion appends a value and moves it upward; removing the root replaces it by the last value and moves that value downward. Each path has $O(\log(n+1))$ levels, and equal values can be stored in separate slots. Both operations therefore take **$O(\log(n+1))$ time when capacity is available**.

Unlike a [binary search tree](../../data-structure.md#binary-search-tree), the heap does not maintain a complete search order, so finding an arbitrary specified value can require $O(n)$ inspections. A simple [array](../../data-structure.md#array-data-structure) implementation also has a capacity issue: a fixed [array](../../data-structure.md#array-data-structure) can fill, and resizing a growable [array](../../data-structure.md#array-data-structure) occasionally costs $O(n)$, giving an amortized insertion guarantee unless allocation is otherwise managed. This capacity cost is an implementation tradeoff, not an inherent inability of heaps to represent the [priority queue](../../data-structure.md#priority-queue) abstraction.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Use one real [linked list node](../../data-structure.md#linked-list-node) per occurrence, with a private reference to the first:
```
class Node(val value: Int, var next: Node)

// Inside the queue implementation:
private var first: Node = null
```
The [representation invariant](../../computer-science.md#representation-invariant) says that the reachable chain is finite, acyclic and nondecreasing in `value`, and is owned by the queue. Equal adjacent values are explicitly allowed. The [abstraction function](../../computer-science.md#abstraction-function) is the [multiset](../../set.md#multiset) containing one occurrence of `v.value` for every reachable real [linked list node](../../data-structure.md#linked-list-node) `v`. Initially `first==null` represents the empty [multiset](../../set.md#multiset). No artificial smallest `Int` is needed as a sentinel, and `Int.MinValue` remains a valid real value.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Insert before the first entry that is at least the new value; equal values remain separate occurrences:
```
class ListPriorityQueue extends PriorityQueue[Int] {
  private var first: Node = null

  def clear(): Unit = { first = null }

  def isEmpty(): Boolean = first == null

  def insert(x: Int): Unit = {
    if (first == null || x <= first.value) {
      first = new Node(x, first)
    } else {
      var p = first
      while (p.next != null && p.next.value < x) {
        p = p.next
      }
      p.next = new Node(x, p.next)
    }
  }

  def delMin(): Int = {
    require(first != null, "Empty priority queue")
    val result = first.value
    first = first.next
    result
  }
}
```
In the scanning branch, the [loop invariant](../../algorithm.md#loop-invariant) says that `p` is reachable and all values from `first` through `p` are strictly smaller than `x`. The rest of the chain is unchanged and remains sorted. The [loop variant](../../algorithm.md#loop-variant) is the number of nodes after `p`. At exit either the next value is at least `x` or there is no next node, so inserting between `p` and `p.next` preserves the [representation invariant](../../computer-science.md#representation-invariant) and adds exactly one occurrence under the [abstraction function](../../computer-science.md#abstraction-function). The head branch covers an empty chain, a new minimum and equality with the old minimum. `delMin` returns the head's minimum value and removes exactly that occurrence.

**Insertion is $O(n)$ worst-case; `delMin`, `isEmpty` and the head-resetting `clear` are $O(1)$**. Reclaiming an abandoned chain later is garbage-collection work, not an explicit traversal performed by `clear`. Storage is $\Theta(n)$, including separate nodes for duplicate values. No fixed insertion-capacity [precondition](../../algorithm.md#precondition) has been added.

## 6

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The [Iterator pattern](../../programming-language.md#iterator-pattern) gives clients a uniform way to inspect and consume the elements of a collection without exposing how that collection is stored. An [iterator](../../data-structure.md#iterator) has a traversal state separate from the abstract collection interface, so the same client loop can process an [array](../../data-structure.md#array-data-structure), a [linked list](../../data-structure.md#linked-list) or generated values. **It preserves [encapsulation](../../computer-science.md#encapsulation-computer-programming) and [representation independence](../../computer-science.md#representation-independence)**: changing the underlying [data structure](../../data-structure.md) need not change the traversal client. Separate [iterator](../../data-structure.md#iterator) instances can track separate traversals; two aliases of one consuming [iterator](../../data-structure.md#iterator) instead share its progress.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The essential abstract methods are:
```
def hasNext: Boolean
def next(): T
```
`hasNext` reports whether another result is available. `next()` returns that result and advances; if exhausted, it throws `NoSuchElementException`. The other ordinary [iterator](../../data-structure.md#iterator) operations are implemented using these primitives. An availability check must not silently discard a result visible to the client, although an adapter may need to fetch and cache underlying values in order to decide availability.[[Iterator](../../data-structure.md#iterator) abstract members hasNext and next; exhaustion contract](../../computer-science-bibliography.md#scala-2-12-iterator-api-documentation)

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The plus marks a [covariant type parameter](../../programming-language.md#covariant-type-parameter): **if $S<:T$, then `Iterator[S] <: Iterator[T]`**. An [iterator](../../data-structure.md#iterator) producing a subtype's values can be used where an [iterator](../../data-structure.md#iterator) of the supertype is required. For example, a [string](../../foundations-of-mathematics.md#string) [iterator](../../data-structure.md#iterator) can be viewed as an [iterator](../../data-structure.md#iterator) of `AnyRef`, because [strings](../../foundations-of-mathematics.md#string) are reference values. The direction is appropriate for a producer: calling `next()` gives a value valid at the wider type. It would not be safe to expose an ordinary insertion method accepting arbitrary wider-type values into a subtype-only collection. This is a [subtyping](../../programming-language.md#subtyping) relationship, not a request to transform each produced value.[Conformance of parameterized types with covariant parameters](../../computer-science-bibliography.md#scala-2-12-types-specification)

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Use [iterator concatenation](../../data-structure.md#iterator-concatenation) and short-circuit the second availability test while the first [iterator](../../data-structure.md#iterator) still has results:
```
class ConcatIterator[T](first: Iterator[T], second: Iterator[T])
    extends Iterator[T] {
  def hasNext: Boolean = first.hasNext || second.hasNext

  def next(): T = {
    if (first.hasNext) first.next()
    else second.next()
  }
}
```
The abstract remaining [sequence](../../sequence-and-series.md#sequence) is the remaining [sequence](../../sequence-and-series.md#sequence) of `first` followed by that of `second`. Each `next()` consumes the head of precisely this [sequence](../../sequence-and-series.md#sequence). When both are exhausted, delegation to `second.next()` raises the required exception. **Construction consumes no elements**, and `hasNext` never calls either underlying `next()`. As usual, clients should not separately consume these [iterators](../../data-structure.md#iterator) while relying on the adapter's traversal. Sharing one underlying [iterator](../../data-structure.md#iterator) between both arguments also shares its state; it does not duplicate its elements.

<h3 id="6/e">e</h3>

↑ **Parent:** [6](#6)

<h4 id="6/e/solution">Solution</h4>

↑ **Parent:** [E](#6/e)

The expression constructs a valid [iterator](../../data-structure.md#iterator) object; it does not itself return the concatenated numeric or character values. The element types have a common supertype `AnyVal`, and covariance lets `Iterator[Int]` and `Iterator[Char]` serve as the two inputs to `ConcatIterator[AnyVal]`. In the ordinary Scala 2 typing of this expression, the common element type is `AnyVal`. One can make the intended widening explicit:
```
new ConcatIterator[AnyVal](
  List(1, 2, 3).iterator,
  List('a', 'b', 'c').iterator
)
```
**Successive calls return `1, 2, 3, 'a', 'b', 'c'`, then exhaustion.** Characters remain characters: viewing an existing [iterator](../../data-structure.md#iterator) at a wider type does not convert its contents to [integer](../../integer.md) character codes. No `next()` is invoked merely by constructing this adapter. The common-type argument uses [subtype polymorphism](../../programming-language.md#subtype-polymorphism) and [covariant type parameters](../../programming-language.md#covariant-type-parameter), rather than requiring the two concrete input types to be equal.

<h3 id="6/f">f</h3>

↑ **Parent:** [6](#6)

<h4 id="6/f/solution">Solution</h4>

↑ **Parent:** [F](#6/f)

Use one cached optional result. Only a request for availability or the next result fills that cache:
```
class FilterIterator[T](test: T => Boolean, iter: Iterator[T])
    extends Iterator[T] {
  private var cached: Option[T] = None

  private def prepare(): Unit = {
    while (cached.isEmpty && iter.hasNext) {
      val x = iter.next()
      if (test(x)) cached = Some(x)
    }
  }

  def hasNext: Boolean = {
    prepare()
    cached.nonEmpty
  }

  def next(): T = {
    prepare()
    cached match {
      case Some(x) =>
        cached = None
        x
      case None => throw new NoSuchElementException("Filtered iterator exhausted")
    }
  }
}
```
This is a [demand-driven filtering iterator](../../data-structure.md#demand-driven-filtering-iterator). When the cache is empty, its abstract remaining [sequence](../../sequence-and-series.md#sequence) is the filtered remaining input. When it holds `Some(x)`, the abstract [sequence](../../sequence-and-series.md#sequence) is `x` followed by the filtered remaining input. The [loop invariant](../../algorithm.md#loop-invariant) for `prepare` says that all input elements consumed during the present search have failed `test`, except for the one cached passing value if one has been found. The first passing value stops the loop, so it cannot read past a result that the client has not yet consumed.

**Construction performs no underlying reads, and repeated `hasNext` calls reuse a cached result.** `next` also works without a preceding `hasNext`, clears only the result it returns, and does not prefetch its successor. `Some(x)`, rather than `Option(x)`, allows a passing null value to remain a genuine cached value. For finite remaining input, its length is a [loop variant](../../algorithm.md#loop-variant); for infinite input, availability can legitimately run forever if no further passing element exists. Deterministic terminating tests and exclusive ownership of the consuming input are assumed. One cache slot is $O(1)$ extra storage.

<h3 id="6/g">g</h3>

↑ **Parent:** [6](#6)

<h4 id="6/g/solution">Solution</h4>

↑ **Parent:** [G](#6/g)

Make two separate character [iterators](../../data-structure.md#iterator) so that scanning uppercase letters does not consume the lowercase pass:
```
def upperLower(s: String): Iterator[Char] = {
  val upper = new FilterIterator[Char]((c: Char) => c.isUpper, s.iterator)
  val lower = new FilterIterator[Char]((c: Char) => c.isLower, s.iterator)
  new ConcatIterator[Char](upper, lower)
}
```
Each filtering [iterator](../../data-structure.md#iterator) preserves the original order of its selected characters. Concatenation therefore yields **all uppercase letters in source order, then all lowercase letters in source order**, omitting other characters. The two `s.iterator` calls are essential: reusing a single consuming [iterator](../../data-structure.md#iterator) would let the first pass discard lowercase characters before the second pass could return them. Construction remains lazy; an empty [string](../../foundations-of-mathematics.md#string) yields an exhausted [iterator](../../data-structure.md#iterator) without a special case.

## 7

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7/a/i)

[Encapsulation](../../computer-science.md#encapsulation-computer-programming) exposes operations with contracts while hiding representation details and controlling changes to state. In a text editor, a document object can privately store text and cursor position and expose `insert`, `delete` and `moveCursor`. Clients cannot directly splice internal storage or set a cursor outside the document. **The document's methods enforce its [representation invariant](../../computer-science.md#representation-invariant)**, and the implementation can later replace a character [array](../../data-structure.md#array-data-structure) by a different text representation without changing the public editing interface. Merely declaring a field private is insufficient if an accessor returns the mutable representation itself.

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/a/ii)

[Class inheritance](../../programming-language.md#class-inheritance) defines a subclass by extending another class's behavior, often with [method overriding](../../programming-language.md#method-overriding) and [subtyping](../../programming-language.md#subtyping). An editor might have an abstract `Command` type with `execute`, and subclasses for insertion and deletion. The controller keeps commands through the common type and [dynamic dispatch](../../programming-language.md#dynamic-dispatch) chooses each command's actual operation. Alternatively, a specialized document can extend a base document's documented behavior. **An inheritance relationship used for substitution must preserve the superclass contract**; borrowing its code alone does not justify exposing incompatible behavior. Commands exemplify the [Command pattern](../../programming-language.md#command-pattern) without exposing document storage to the controller.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

The constructor stores a reference, not a copy:
```
val d = new Dimension(3, 4)
val f = new Frame(d)
d.width = 10
```
Now **`f.area` is still $12$, but the product of its stored dimension fields is $40$**. Even without retaining `d`, a client can break the same invariant through `f.dimension.height = 9`, because the accessor exposes the same mutable object. This is [representation exposure](../../computer-science.md#representation-exposure) through [reference aliasing](../../computer-memory.md#reference-aliasing). A `val` prevents reassigning the reference; it does not freeze the referenced object.

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

Make defensive copies on both entry and exit, while keeping the supplied `Dimension` class unchanged:
```
class Frame(d: Dimension) {
  require(d != null)
  private val saved = new Dimension(d.width, d.height)
  private val savedArea = saved.width * saved.height

  def area: Int = savedArea
  def dimension: Dimension = new Dimension(saved.width, saved.height)
  def isPortrait: Boolean = saved.height >= saved.width
}
```
The private stored dimensions have no aliases exposed to the caller and are never changed. Mutating the constructor argument affects only the caller's object; mutating a returned `Dimension` affects only a fresh copy. Consequently **the stored area is calculated once and stays equal to the stored dimensions' product**. This [defensive copying](../../computer-science.md#defensive-copying) is sufficient because `Dimension` contains only primitive fields; a more deeply nested mutable structure could require a [deep copy](../../computer-memory.md#deep-copy) or an immutable representation.

The multiplication above deliberately retains the supplied class's `Int` arithmetic and accessor type. If an exact mathematical area outside that range is required, compute once with `saved.width.toLong * saved.height.toLong` and expose `Long` instead; avoiding aliases and avoiding [integer overflow](../../programming-language.md#integer-overflow) are separate concerns.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/i">i</h4>

↑ **Parent:** [C](#7/c)

<h5 id="7/c/i/solution">Solution</h5>

↑ **Parent:** [I](#7/c/i)

Compare areas before and after each completed setter call. Widen before multiplication so all products of two `Int` dimensions are represented exactly:
```
class LoggedResizableFrame(h: Int, w: Int) extends ResizableFrame(h, w) {
  private var increases = BigInt(0)

  private def actualArea: Long = height.toLong * width.toLong

  override def height_=(h: Int): Unit = {
    val before = actualArea
    super.height_=(h)
    if (actualArea > before) increases += 1
  }

  override def width_=(w: Int): Unit = {
    val before = actualArea
    super.width_=(w)
    if (actualArea > before) increases += 1
  }

  def getIncreases: BigInt = increases
}
```
The history [invariant](../../mathematics.md#invariant-mathematics) is that `increases` counts exactly the completed dimension updates whose new area strictly exceeds their immediately preceding area. The constructor's starting area is a baseline, not an increase. Each overriding setter invokes the superclass setter once and increments precisely when its comparison succeeds. Equal-area changes do not count. **The comparison is on area, not merely on which dimension increased**; this also handles zero or signed dimensions without adding an unstated input restriction. An [arbitrary-precision integer](../../arithmetic.md#arbitrary-precision-integer) avoids eventual counter overflow.

<h4 id="7/c/ii">ii</h4>

↑ **Parent:** [C](#7/c)

<h5 id="7/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/c/ii)

One base-class implementation changes the private fields directly:
```
def flip(): Unit = {
  val oldH = _h
  _h = _w
  _w = oldH
}
```
The completed operation leaves the area unchanged. It calls no overriding setters, so the logging subclass's count stays unchanged and **does not need an override**. The invariant is about completed public updates, not transient internal states between the two assignments.

A second implementation uses public setters:
```
def flip(): Unit = {
  val oldH = height
  val oldW = width
  height = oldW
  width = oldH
}
```
These setter calls use [dynamic dispatch](../../programming-language.md#dynamic-dispatch) on a logging receiver. Starting at height two and width three, the first call increases the temporary area from six to nine and wrongly increments the count, while the final area returns to six. **This version needs a subclass override**. With the counter name from part (i), the following override discards the internal setter contributions:
```
override def flip(): Unit = {
  val before = increases
  super.flip()
  increases = before
}
```
For this specified base implementation the two assignments complete normally and the final area equals the initial area, so restoring the saved count is correct. Another design could suppress logging during the compound operation. The difference between the two base implementations illustrates the [fragile base class problem](../../programming-language.md#fragile-base-class-problem): an internal refactoring can change subclass behavior through newly introduced virtual calls.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/solution">Solution</h4>

↑ **Parent:** [D](#7/d)

Use [object composition](../../programming-language.md#object-composition): a logging wrapper owns a private `ResizableFrame` and delegates dimension operations to it, rather than being its subclass. The wrapper takes the before/after area around each public operation. Its own `flip` calls the component's whole `flip` once, compares only the completed states, and therefore records no increase. The component must be exclusively owned or defensively copied, so clients cannot bypass the wrapper's accounting.

**The component's internal calls cannot dynamically dispatch into the separate wrapper.** This prevents the setter-based `flip` implementation change from creating false log entries and reduces dependence on undocumented superclass internals. The wrapper can also choose a smaller interface. Costs include forwarding code and the loss of automatic `ResizableFrame` subtyping: code requiring that concrete superclass cannot necessarily accept the wrapper. A shared abstract frame interface can recover substitutability while keeping implementation reuse based on composition. Composition improves this dependency boundary; it does not remove the need for a clear mutation and ownership contract.

## 8

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

[Test-driven development](../../computer-science.md#test-driven-development) uses a short cycle: write a test for the next behavior and observe its failure, implement enough to pass it, then refactor without changing the tested behavior. In a conventional implementation-then-test workflow, tests primarily assess code after it has been written; in TDD they also guide each small design increment. Tests accumulate into a regression suite, but passing them is not a universal correctness proof.[Definition: interleaved unit tests, implementation and refactoring](../../computer-science-bibliography.md#test-driven-development-in-the-agile-alliance-glossary)

A good candidate is a deterministic [priority queue](../../data-structure.md#priority-queue) operation with a precise contract. Before implementation, test that inserting two equal values permits two minimum deletions and only then leaves an empty queue. The expected result is objective, cheap to check and useful for finding the duplicate-loss bug in a set-based representation.

An exploratory decision about whether an editor's toolbar feels usable is a poor candidate for TDD alone: the desired behavior and human evaluation criteria may not yet be settled, and an executable assertion does not replace user observation. Prototypes and usability evaluation can establish the design before stable behavioral properties are tested automatically. **The distinction is the availability of a useful repeatable test oracle**, not a claim that interface software is inherently untestable.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

A [code smell](../../computer-science.md#code-smell) is an easily noticed feature that suggests a deeper design problem worth investigating. It is neither a proven bug nor an automatic instruction to rewrite the code. Context determines whether the symptom is troublesome.[9 February 2006: surface indication, investigation rather than automatic condemnation; long-method example](../../computer-science-bibliography.md#code-smell-by-martin-fowler)

[Duplicate code](../../computer-science.md#duplicate-code) can indicate that the same knowledge has several maintenance sites: a correction made to one copy may be forgotten in the other. If the copies represent the same responsibility, extract that responsibility into one shared operation or component. Merely looking similar is insufficient; accidentally similar code with independent purposes should not necessarily be coupled.

[Feature envy](../../computer-science.md#feature-envy) occurs when an operation depends mainly on another object's data rather than the responsibilities of its own class. For example, an editor view might implement a text-policy decision by repeatedly inspecting document internals. Move that decision to the document, or extract and move the relevant part, so behavior sits with the data and responsibility it actually uses. **Duplication suggests consolidating repeated knowledge; feature envy suggests moving a responsibility between objects.** These are different design actions, and both can be [refactorings](../../computer-science.md#refactoring) that preserve observable behavior.[Move [Function](../../function.md), called Move Method in the first edition: move behavior to a better-suited context](../../computer-science-bibliography.md#move-function-in-the-refactoring-catalog)

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

The [Observer pattern](../../programming-language.md#observer-pattern) lets interested observers subscribe through a common interface to a subject's events or state changes. The subject notifies registered observers, which perform their own reactions; subscriptions can later be removed. A document model can thereby update multiple editor views without containing explicit knowledge of each view class.

**It avoids tightly coupling the subject to every concrete consumer.** Adding another view does not require adding a new view-specific call inside core model logic. Notifications should expose a coherent updated state, and unused observers should unsubscribe. The pattern does not itself prevent feedback cycles: observers that update each other's sources can still cause repeated or reentrant notifications. The supplied buttons and containing frame use this subscription-and-reaction design through [Scala Swing](../../programming-language.md#scala-swing).

<h3 id="8/d">d</h3>

↑ **Parent:** [8](#8)

<h4 id="8/d/solution">Solution</h4>

↑ **Parent:** [D](#8/d)

Inside the supplied `MainFrame`, after both buttons and the label are defined, add:
```
private var clickCount = BigInt(0)
listenTo(button1, button2)
reactions += {
  case ButtonClicked(source) if (source eq button1) || (source eq button2) =>
    clickCount += 1
    label.text = "Total button clicks: " + clickCount.toString
}
```
The [invariant](../../mathematics.md#invariant-mathematics) is that `clickCount` equals the total number of handled click events from the two buttons. It starts at zero; each matching event increments it exactly once and refreshes the label. The buttons' existing self-listeners can still change their own text independently. **Listening to both publishers is necessary**: their `listenTo(this)` calls subscribe each button to itself, not the frame to both buttons. Updating the label is not another button click, so it does not recursively increment the counter. An [arbitrary-precision integer](../../arithmetic.md#arbitrary-precision-integer) keeps the count exact without a lifetime overflow bound.[Publisher/Reactor subscriptions, listenTo, and reactions; ButtonClicked source event](../../computer-science-bibliography.md#scala-swing-event-system-documentation)

The supplied layout already contains the label, so no additional component is needed. Before any click it retains its initial zero-click message; afterwards it displays the cumulative count across both buttons.

## ↑ Ancestors (9)

1. [2019](../2019.md)
2. [Past exam of the year 1 of the computer science course of the University of Oxford](../../past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Year 1 of the computer science course of the University of Oxford](../../university-of-oxford.md#year-1-of-the-computer-science-course-of-the-university-of-oxford)
4. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../university-of-oxford.md)
8. [List of universities](../../README.md#list-of-universities)
9. [Codex Wiki](../../README.md)
