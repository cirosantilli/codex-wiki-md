# Imperative programming resit

↑ **Parent:** [2019](../2019.md)

Source paper: [released examination archive, member 2018/L/a10098w1.pdf](https://www.whatdotheyknow.com/request/ba_computer_science_past_papers/response/2577745/attach/2/202402%20183%20CS%20Papers.zip?cookie_passthrough=1). The cover identifies the Long Vacation sitting of Thursday 5 September 2019. That printed identity takes precedence over the archive member's directory name.

The implementations use [Scala](../../programming-language.md#scala) 2 syntax. Fixed-width results are checked when [arbitrary-precision arithmetic](../../arithmetic.md#arbitrary-precision-arithmetic) is needed internally; the mathematical contracts do not make [integer overflow](../../programming-language.md#integer-overflow) harmless. All eight questions are covered.

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
  - [g](#3/g)
    - [Solution](#3/g/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [i](#6/c/i)
      - [Solution](#6/c/i/solution)
    - [ii](#6/c/ii)
      - [Solution](#6/c/ii/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [i](#7/b/i)
      - [Solution](#7/b/i/solution)
    - [ii](#7/b/ii)
      - [Solution](#7/b/ii/solution)
    - [iii](#7/b/iii)
      - [Solution](#7/b/iii/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
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

↑ **Parent:** [Imperative programming resit](imperative-programming-resit.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the remainder form of the [Euclidean algorithm](../../number-theory.md#euclidean-algorithm) to compute the [greatest common divisor](../../divisibility.md#greatest-common-divisor), then divide both components of the [fraction](../../number-theory.md#fraction) by it:
```
def Reduce(num: Int, den: Int): (Int, Int) = {
  require(0 <= num && num < den)
  var a = den
  var b = num
  while (b != 0) {
    val r = a % b
    a = b
    b = r
  }
  (num / a, den / a)
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $a>0$, $b\geq0$, and $\gcd(a,b)=\gcd(den,num)$. Initially it holds by symmetry of the [greatest common divisor](../../divisibility.md#greatest-common-divisor). For $b>0$, the [integer division](../../arithmetic.md#integer-division) identity $a=qb+r$, with $0\leq r<b$, shows that $a,b$ and $b,r$ have exactly the same common [integer divisors](../../divisibility.md#divisor). Thus the update preserves the [loop invariant](../../algorithm.md#loop-invariant). The [loop variant](../../algorithm.md#loop-variant) is the nonnegative [integer](../../integer.md) $b$, which strictly decreases on each iteration. At exit $b=0$, so $a=\gcd(den,num)>0$. Dividing by $a$ preserves the [rational number](../../number-theory.md#rational-number) and makes the returned components [coprime](../../divisibility.md#coprime-integers). In particular, **zero is returned as $(0,1)$**. No multiplication is needed, and all remainders remain within the original nonnegative `Int` range.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a positive remaining [fraction](../../number-theory.md#fraction) $n/d$, the condition $1/q\leq n/d$ is equivalent to $q\geq d/n$. Since $1/q$ decreases as the positive [integer](../../integer.md) $q$ increases, **choose $q=\lceil d/n\rceil$**. The zero [fraction](../../number-theory.md#fraction) needs no term. This is the [greedy Egyptian fraction expansion](../../number-theory.md#greedy-egyptian-fraction-expansion).

The remaining [fraction](../../number-theory.md#fraction) is

$$
\frac nd-\frac1q=\frac{nq-d}{dq}.
$$

The defining inequalities $q-1<d/n\leq q$ give $0\leq nq-d<n$. Therefore the unreduced new numerator is a nonnegative [integer](../../integer.md) strictly smaller than the old positive numerator. Passing to a [reduced fraction](../../number-theory.md#reduced-fraction) can only reduce it further. That numerator is a [loop variant](../../algorithm.md#loop-variant), so the process terminates. The increasing denominators are not the termination argument; their size need not be bounded in advance.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Maintain an accumulated [array](../../data-structure.md#array-data-structure) of denominators and an exact remaining [fraction](../../number-theory.md#fraction). The usual [greedy algorithm](../../algorithm.md#greedy-algorithm) can require a denominator larger than `Int.MaxValue`, even for an input with `Int` components. The following implementation uses [arbitrary-precision integers](../../arithmetic.md#arbitrary-precision-integer) internally. If that representational limit is reached, it returns the always-valid alternative consisting of `num` copies of $1/den$. Repeated denominators are permitted by the given [Egyptian fraction](../../number-theory.md#egyptian-fraction) representation.
```
def fromRat(num: Int, den: Int): Array[Int] = {
  require(0 <= num && num < den)
  val start = Reduce(num, den)
  var n = BigInt(start._1)
  var d = BigInt(start._2)
  var e = Array.empty[Int]
  while (n > 0) {
    val q = (d + n - 1) / n
    if (!q.isValidInt) return Array.fill(num)(den)
    e = e :+ q.toInt
    val nextN = n * q - d
    val nextD = d * q
    val g = nextN.gcd(nextD)
    n = nextN / g
    d = nextD / g
  }
  e
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $d>0$, $0\leq n<d$, all entries of `e` are positive, and

$$
\sum_{0\leq j<e.length}\frac1{e(j)}+\frac nd=\frac{num}{den}.
$$

Appending $q$ and replacing the residual by $(nq-d)/(dq)$ preserves this equality; division by the [greatest common divisor](../../divisibility.md#greatest-common-divisor) preserves the residual's value. The [loop variant](../../algorithm.md#loop-variant) is $n$, by the proof in part (b). If `nextN` is zero, its [greatest common divisor](../../divisibility.md#greatest-common-divisor) with `nextD` is `nextD`, giving residual $0/1$. On normal exit the residual is zero and **the returned [array](../../data-structure.md#array-data-structure) has exactly the required value**. On the early-return branch, `num` copies of $1/den$ have that same value directly; the partial [greedy Egyptian fraction expansion](../../number-theory.md#greedy-egyptian-fraction-expansion) is discarded. `num=0` returns an empty [array](../../data-structure.md#array-data-structure).

The fallback is a correctness provision for the fixed result type, not an efficiency claim: a large repeated-term [array](../../data-structure.md#array-data-structure) can be impractical. An [array](../../data-structure.md#array-data-structure) of [arbitrary-precision integers](../../arithmetic.md#arbitrary-precision-integer) would retain the [greedy Egyptian fraction expansion](../../number-theory.md#greedy-egyptian-fraction-expansion) without this fallback. Allocation, as with any output-producing program, requires enough available memory. The `BigInt` remainder, [greatest common divisor](../../divisibility.md#greatest-common-divisor) and checked conversion operations are documented in [Methods gcd, isValidInt and toInt](../../computer-science-bibliography.md#scala-2-12-bigint-api-documentation).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

An [Egyptian fraction](../../number-theory.md#egyptian-fraction) need not be proper: several positive [unit fractions](../../number-theory.md#unit-fraction) may sum to at least one. Accordingly, accumulate a general nonnegative [reduced fraction](../../number-theory.md#reduced-fraction), rather than calling the proper-input-only `Reduce` on every intermediate value. First define an exact helper:
```
def toRatExact(e: Array[Int]): (BigInt, BigInt) = {
  var n = BigInt(0)
  var d = BigInt(1)
  var i = 0
  while (i < e.length) {
    require(e(i) > 0)
    val x = BigInt(e(i))
    val g = d.gcd(x)
    val nextN = n * (x / g) + d / g
    val nextD = d * (x / g)
    val h = nextN.gcd(nextD)
    n = nextN / h
    d = nextD / h
    i += 1
  }
  (n, d)
}

def toRat(e: Array[Int]): (Int, Int) = {
  val result = toRatExact(e)
  require(result._1.isValidInt && result._2.isValidInt,
          "Reduced result does not fit (Int, Int)")
  (result._1.toInt, result._2.toInt)
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $0\leq i\leq e.length$, $n\geq0$, $d>0$, $\gcd(n,d)=1$, and

$$
\frac nd=\sum_{0\leq j<i}\frac1{e(j)}.
$$

Writing $g=\gcd(d,x)$, the [fraction](../../number-theory.md#fraction) for the extended prefix has numerator $n(x/g)+d/g$ and denominator $d(x/g)$. These are the `nextN` and `nextD` in the code. Reducing them preserves the value and restores [coprimality](../../divisibility.md#coprime-integers). The [loop variant](../../algorithm.md#loop-variant) is $e.length-i$. At exit **the helper returns the exact sum in lowest terms**, including $(0,1)$ for the empty [array](../../data-structure.md#array-data-structure).

There are three distinct ways to control [integer overflow](../../programming-language.md#integer-overflow): cancel the common denominator factor before multiplication, reduce after each addition, and use [arbitrary-precision arithmetic](../../arithmetic.md#arbitrary-precision-arithmetic) when the remaining values still exceed fixed-width bounds. Cancellation reduces intermediate size but cannot guarantee that an exact answer fits `(Int, Int)`. For example, the sum $1/46337+1/46349$ is $92686/2147673613$ in lowest terms, whose denominator exceeds `Int.MaxValue`. No implementation returning that fixed type can represent every permitted input exactly. The wrapper therefore checks this unavoidable result-type limitation instead of silently truncating; `toRatExact` supplies the unrestricted mathematical result.[Checked representability with isValidInt before the potentially truncating toInt conversion](../../computer-science-bibliography.md#scala-2-12-bigint-api-documentation)

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Print separators before all but the first term, so there is neither a leading nor a trailing plus sign:
```
def printRat(num: Int, den: Int): Unit = {
  print(num.toString + "/" + den.toString)
}

def printEgypt(e: Array[Int]): Unit = {
  if (e.isEmpty) print("0")
  var i = 0
  while (i < e.length) {
    if (i > 0) print(" + ")
    print("1/" + e(i).toString)
    i += 1
  }
}
```
The [loop invariant](../../algorithm.md#loop-invariant) says that exactly the first $i$ [unit fractions](../../number-theory.md#unit-fraction) have been printed in order, separated by ` + `, with no trailing separator. The [loop variant](../../algorithm.md#loop-variant) is $e.length-i$. The empty [array](../../data-structure.md#array-data-structure) is displayed as zero. Since $5/7-1/2=3/14$ and $3/14-1/5=1/70$, **the output is `5/7 = 1/2 + 1/5 + 1/70`**. The source's earlier example with middle denominator $4$ and final denominator $70$ contains the arithmetic typo; its final printing example is correct. Indeed $1/2+1/4>5/7$, so no positive final term could repair that particular prefix. The printing routine reports the generated terms rather than imposing a particular expansion.

## 2

↑ **Parent:** [Imperative programming resit](imperative-programming-resit.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let `a` be the given enclosing [array](../../data-structure.md#array-data-structure). A [two-way array partition](../../algorithm.md#two-way-array-partition) needs only one scan, and does not require the pivot to occur in the [array](../../data-structure.md#array-data-structure):
```
def partition(l: Int, r: Int, p: Int): Int = {
  require(0 <= l && l <= r && r <= a.length)
  var k = l
  var j = l
  while (j < r) {
    if (a(j) < p) {
      val t = a(k)
      a(k) = a(j)
      a(j) = t
      k += 1
    }
    j += 1
  }
  k
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $l\leq k\leq j\leq r$, every entry of $a[l,k)$ is less than $p$, every entry of $a[k,j)$ is at least $p$, and the segment's [multiset](../../set.md#multiset) is unchanged. Entries outside $[l,r)$ are unchanged. When `a(j)<p`, swapping it into position `k` extends the low part; if `k<j`, the displaced entry was in the high part and remains there after `j` advances. If `k==j`, the self-swap is harmless. The other branch simply extends the high part. The [loop variant](../../algorithm.md#loop-variant) is $r-j$. At exit $j=r$, so **the returned $k$ has the required separation property**, including empty segments and arbitrarily many duplicate entries. The [time complexity](../../theoretical-computer-science.md#time-complexity) is $\Theta(r-l+1)$ and auxiliary [space complexity](../../theoretical-computer-science.md#space-complexity) is $O(1)$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

For an integer pivot $0\leq p\leq N+1$, exactly $k$ entries lie in $[0,p)$. That interval contains $p$ possible [integers](../../integer.md). If $k<p$, the [pigeonhole principle](../../combinatorics.md#pigeonhole-principle) implies that **some value in $[0,p)$ is missing**. Counting occurrences rather than distinct entries only strengthens this argument: $k$ occurrences cannot cover more than $k$ distinct values.

For completeness, if $p>N+1$ the lower side contains the entire permitted value range, which already has a missing value. If $p\leq0$, the condition $k<p$ is impossible. Thus the general conclusion is a missing permitted value below $p$; an internal pivot gives useful localization.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

There are $N-k$ entries in $[p,N+1)$, which contains $N+1-p$ possible [integers](../../integer.md). If $k\geq p$, then $N-k\leq N-p<N+1-p$. Therefore **some value in $[p,N+1)$ is missing**, again by the [pigeonhole principle](../../combinatorics.md#pigeonhole-principle). This is an existence conclusion in the chosen interval, not a claim that all missing values lie there; both sides can contain missing values when duplicates occur.

If $p\leq0$, the upper side contains the whole permitted range and hence a missing value. If $p>N+1$, the condition $k\geq p$ is impossible. Outside the internal-pivot range this conclusion therefore supplies no improved localization.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Keep a deficient interval of possible values and only the [array](../../data-structure.md#array-data-structure) segment containing occurrences from that interval. This is [missing-value search by deficient value intervals](../../algorithm.md#missing-value-search-by-deficient-value-intervals):
```
def missing(): Int = {
  val n = a.length
  var lo = 0L
  var hi = n.toLong + 1L
  var l = 0
  var r = n
  while (hi - lo > 1L) {
    val p = lo + (hi - lo) / 2L
    val k = partition(l, r, p.toInt)
    if ((k - l).toLong < p - lo) {
      hi = p
      r = k
    } else {
      lo = p
      l = k
    }
  }
  lo.toInt
}
```
The [precondition](../../algorithm.md#precondition) is that every original entry lies in $[0,N+1)$. The [loop invariant](../../algorithm.md#loop-invariant) is

$$
0\leq lo<hi\leq N+1,\qquad 0\leq l\leq r\leq N,\qquad r-l<hi-lo,
$$

together with: every active entry lies in $[lo,hi)$, and every original occurrence with a value in that interval is in the active segment. The whole [array](../../data-structure.md#array-data-structure) remains a [permutation](../../combinatorics.md#permutation) of its initial contents. Initially these assertions follow from the [precondition](../../algorithm.md#precondition) and $N<N+1$.

After [array partitioning](../../algorithm.md#two-way-array-partition), the low subinterval has $k-l$ occurrences and $p-lo$ possible values. If it is deficient, retaining it preserves the [loop invariant](../../algorithm.md#loop-invariant). Otherwise $k-l\geq p-lo$, while the original active count is strictly less than $hi-lo$; subtraction gives

$$
r-k<(hi-lo)-(p-lo)=hi-p.
$$

Thus the high subinterval is deficient and retaining it also preserves the [loop invariant](../../algorithm.md#loop-invariant). Discarded occurrences lie outside the new candidate interval. The [loop variant](../../algorithm.md#loop-variant) is the positive [integer](../../integer.md) $hi-lo$, which strictly decreases because the midpoint is strictly internal. At exit the interval has one possible value and fewer than one occurrence, so **`lo` is absent from the entire original [array](../../data-structure.md#array-data-structure)**. For $N=0$ the loop is skipped and zero is returned. The `Long` value bounds avoid overflowing $N+1$; every internal pivot is at most $N$, so its checked mathematical range fits `Int`.

For the [time complexity](../../theoretical-computer-science.md#time-complexity), let $W_i$ be the interval width and $m_i$ its active occurrence count before iteration $i$. The [loop invariant](../../algorithm.md#loop-invariant) gives $m_i<W_i$, and [binary search](../../algorithm.md#binary-search) gives $W_{i+1}\leq\lceil W_i/2\rceil$. Each [two-way array partition](../../algorithm.md#two-way-array-partition) costs $O(m_i+1)$. Until the width reaches one, the widths are bounded by $(N+1)/2^i+1$, so the total scan work is bounded by a [geometric series](../../sequence-and-series.md#geometric-series) plus $O(\log(N+1))$ loop overhead: **$O(N+1)$ overall, hence $O(N)$ for positive $N$**. Partitioning the full [array](../../data-structure.md#array-data-structure) again at every iteration would instead lose this bound. Auxiliary [space complexity](../../theoretical-computer-science.md#space-complexity) is $O(1)$.

## 3

↑ **Parent:** [Imperative programming resit](imperative-programming-resit.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The abstract state is a finite [partial function](../../function.md#partial-function) $B$ from [strings](../../foundations-of-mathematics.md#string) to [strings](../../foundations-of-mathematics.md#string), initially empty. Names and numbers below are non-null mathematical [strings](../../foundations-of-mathematics.md#string). `store` replaces an old binding if present; `delete` reports whether a binding existed.
```
trait Book {
  // Abstract state B: finite partial map String -> String; initially empty.

  // Pre: name != null && number != null.
  // Post: B' = B updated at name with number.
  def store(name: String, number: String): Unit

  // Pre: name != null && name is in dom(B).
  // Post: result = B(name), and B' = B.
  def recall(name: String): String

  // Pre: name != null.
  // Post: result iff name is in dom(B), and B' = B.
  def isInBook(name: String): Boolean

  // Pre: name != null.
  // Post: result iff name was in dom(B); B' = B with name removed.
  def delete(name: String): Boolean
}
```
These [preconditions](../../algorithm.md#precondition) and [postconditions](../../algorithm.md#postcondition) specify an [abstract data type](../../computer-science.md#abstract-data-type), independently of any [linked list](../../data-structure.md#linked-list). In particular, a failed deletion leaves the abstract state unchanged, and recalling a missing name is outside the operation's specified domain.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [linked list node](../../data-structure.md#linked-list-node) needs mutable fields for changing a stored number and rearranging links:
```
class Node(var name: String, var number: String, var next: Node)
```
The implementation will keep its real [linked list nodes](../../data-structure.md#linked-list-node) private to the `Book` object and will not return [linked list node](../../data-structure.md#linked-list-node) references to clients.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A permanent [dummy header node](../../data-structure.md#sentinel-node) gives even the first real [linked list node](../../data-structure.md#linked-list-node) a predecessor. Insertion into an empty [linked list](../../data-structure.md#linked-list) and deletion or movement of its first real [linked list node](../../data-structure.md#linked-list-node) then use the same link updates as internal cases. The header itself represents no contact, so it also removes the need to use a real name as a special end marker. A search still needs a null-end check.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Start with a private permanent header whose `next` is null. Its two [string](../../foundations-of-mathematics.md#string) fields are ignored. For a concrete state satisfying the [representation invariant](../../computer-science.md#representation-invariant), define the [abstraction function](../../computer-science.md#abstraction-function)

$$
\alpha(header)=\{v.name\mapsto v.number:\ v\text{ is a real node reachable from }header.next\}.
$$

The [representation invariant](../../computer-science.md#representation-invariant) says that the header exists, the reachable real [linked list](../../data-structure.md#linked-list) is finite and acyclic, the header is not a real reachable [linked list node](../../data-structure.md#linked-list-node), all real name/number fields are non-null [strings](../../foundations-of-mathematics.md#string), and real names are pairwise distinct. The real [linked list nodes](../../data-structure.md#linked-list-node) are owned by the book, so clients cannot mutate their fields through exposed references. Distinct names ensure that the displayed relation is a [partial function](../../function.md#partial-function). The initial empty [linked list](../../data-structure.md#linked-list) has abstraction $\varnothing$. Reordering real [linked list nodes](../../data-structure.md#linked-list-node) changes the representation but not the abstract book.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Search for the predecessor of the matching [linked list node](../../data-structure.md#linked-list-node), or for the last [linked list node](../../data-structure.md#linked-list-node) if there is no match. This helper makes deletion uniform:
```
class LinkedBook extends Book {
  private val header = new Node("", "", null)

  // Pre: name != null.
  // Post: result is header or a real node.
  // All real nodes through result have names different from name.
  // result.next is null or has name equal to name.
  // No state is changed.
  private def findPrev(name: String): Node = {
    require(name != null)
    var p = header
    while (p.next != null && p.next.name != name) {
      p = p.next
    }
    p
  }

  def store(name: String, number: String): Unit = {
    require(name != null && number != null)
    val p = findPrev(name)
    if (p.next == null)
      p.next = new Node(name, number, null)
    else
      p.next.number = number
  }

  def recall(name: String): String = {
    require(name != null)
    val p = findPrev(name)
    require(p.next != null, "Name is not in the book")
    p.next.number
  }

  def isInBook(name: String): Boolean = {
    require(name != null)
    findPrev(name).next != null
  }

  def delete(name: String): Boolean = {
    require(name != null)
    val p = findPrev(name)
    if (p.next == null) false
    else {
      p.next = p.next.next
      true
    }
  }
}
```
The search [loop invariant](../../algorithm.md#loop-invariant) says that `p` is the header or a reachable real [linked list node](../../data-structure.md#linked-list-node), and every real [linked list node](../../data-structure.md#linked-list-node) from the start through `p` has a name different from the requested name. The [linked list](../../data-structure.md#linked-list) has not been changed. [Short-circuit evaluation](../../programming-language.md#short-circuit-evaluation) protects `p.next.name` when the end is reached. The [loop variant](../../algorithm.md#loop-variant) is the number of real [linked list nodes](../../data-structure.md#linked-list-node) strictly after `p`; finiteness and acyclicity make it a nonnegative decreasing [integer](../../integer.md). Consequently the helper's stated [postcondition](../../algorithm.md#postcondition) holds.

For `store`, a found name changes only its number; an absent name adds exactly one fresh binding at the end, maintaining uniqueness. For `delete`, unlinking the found [linked list node](../../data-structure.md#linked-list-node) removes exactly the requested binding; absence returns false without mutation. Both query operations preserve the [abstraction function](../../computer-science.md#abstraction-function). Non-null [preconditions](../../algorithm.md#precondition) are checked at entry; **`recall` additionally checks membership using the one completed search**, avoiding a redundant whole-list membership scan. The helper is the only additional operation and its complete behavioral contract is stated above.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Let $m\geq1$ be the number of real contacts, and suppose the requested name is at position $j$, counting from one. The implementation above makes exactly $j$ name-equality comparisons, including the successful comparison; null checks are not [string](../../foundations-of-mathematics.md#string) comparisons. Thus **the minimum is one, when the first real contact is requested, and the maximum is $m$, when the last is requested**. The [precondition](../../algorithm.md#precondition) excludes unsuccessful recalls and recalls on an empty book. This counts calls to [string](../../foundations-of-mathematics.md#string) equality, not individual character inspections within each call.

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

Use the [move-to-front heuristic](../../data-structure.md#move-to-front-heuristic). Replace only `recall` in `LinkedBook` by:
```
def recall(name: String): String = {
  require(name != null)
  val p = findPrev(name)
  require(p.next != null, "Name is not in the book")
  val found = p.next
  if (p ne header) {
    p.next = found.next
    found.next = header.next
    header.next = found
  }
  found.number
}
```
The search has the same [loop invariant](../../algorithm.md#loop-invariant) and [loop variant](../../algorithm.md#loop-variant) as before. Detach the existing [linked list node](../../data-structure.md#linked-list-node) before inserting it immediately after the [dummy header node](../../data-structure.md#sentinel-node). The branch for an already-first [linked list node](../../data-structure.md#linked-list-node) avoids linking it to itself. Every real contact still occurs exactly once with the same name/number binding, so the [representation invariant](../../computer-science.md#representation-invariant) and [abstraction function](../../computer-science.md#abstraction-function) are preserved at return. **No new [linked list node](../../data-structure.md#linked-list-node) is allocated, and an immediate repeated recall needs one name comparison.** The present recall still pays its original search cost; the gain is for later repeated access.

## 4

↑ **Parent:** [Imperative programming resit](imperative-programming-resit.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Treat a null reference as the empty [binary tree](../../data-structure.md#binary-tree) and perform the visit before descending:
```
def preorderRecursive(t: Tree): Unit = {
  if (t != null) {
    println(t.datum)
    preorderRecursive(t.left)
    preorderRecursive(t.right)
  }
}
```
By [structural induction](../../foundations-of-mathematics.md#structural-induction), the empty [binary tree](../../data-structure.md#binary-tree) produces the empty output. A nonempty [binary tree](../../data-structure.md#binary-tree) prints its root label, then the complete [preorder traversal](../../tree-graph-theory.md#preorder-traversal) of the left [subtree](../../data-structure.md#subtree), then that of the right [subtree](../../data-structure.md#subtree). These are exactly the required output positions. The [recursion](../../algorithm.md#recursion-computer-science) terminates on a finite [binary tree](../../data-structure.md#binary-tree) because each recursive call has strictly fewer [vertices](../../graph.md#vertex-graph-theory). For the three-node example, **the output order is $2,1,3$**. The [time complexity](../../theoretical-computer-science.md#time-complexity) is linear in the number of [vertices](../../graph.md#vertex-graph-theory), with [call stack](../../data-structure.md#call-stack) depth bounded by the [height of a binary tree](../../data-structure.md#height-of-a-binary-tree) plus a constant.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Store the bottom of the [stack](../../data-structure.md#stack-data-structure) at index zero and the top at the last occupied index:
```
class Stack {
  private val MAX = 1000
  private val data = new Array[Tree](MAX)
  private var used = 0

  // Pre: used < MAX.
  def push(t: Tree): Unit = {
    require(used < MAX, "Stack full")
    data(used) = t
    used += 1
  }

  // Pre: used > 0.
  def pop: Tree = {
    require(used > 0, "Stack empty")
    used -= 1
    val result = data(used)
    data(used) = null
    result
  }

  // Pre: true.
  def isEmpty: Boolean = used == 0
}
```
The [representation invariant](../../computer-science.md#representation-invariant) is that `data.length==MAX`, $0\leq used\leq MAX$, and unused slots from `used` onwards contain null references. Occupied slots contain the stored `Tree` references; the [stack](../../data-structure.md#stack-data-structure) itself need not forbid null values. The [abstraction function](../../computer-science.md#abstraction-function), written with the first [sequence](../../sequence-and-series.md#sequence) element at the top, is

$$
\alpha(data,used)=[data(used-1),data(used-2),\ldots,data(0)].
$$

Initially this is the empty [sequence](../../sequence-and-series.md#sequence). `push` prepends its argument, `pop` removes and returns the first abstract element, and `isEmpty` reports whether the abstract [sequence](../../sequence-and-series.md#sequence) is empty. These [postconditions](../../algorithm.md#postcondition) follow directly from the index changes. Clearing a popped slot avoids retaining an otherwise unused [tree](../../tree-graph-theory.md) reference. All three operations take **$O(1)$ time**. No loops are needed.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Push the right child before the left child so that the [LIFO stack](../../data-structure.md#stack-data-structure) exposes the left child first:
```
def preorderIterative(t: Tree): Unit = {
  val pending = new Stack
  if (t != null) pending.push(t)
  while (!pending.isEmpty) {
    val u = pending.pop
    println(u.datum)
    if (u.right != null) pending.push(u.right)
    if (u.left != null) pending.push(u.left)
  }
}
```
Let $P(u)$ be the [sequence](../../sequence-and-series.md#sequence) of labels in the [preorder traversal](../../tree-graph-theory.md#preorder-traversal) of $u$. If the abstract pending [stack](../../data-structure.md#stack-data-structure), top first, is $[u_1,\ldots,u_k]$, the [loop invariant](../../algorithm.md#loop-invariant) is that the output already printed, followed by $P(u_1)\mathbin{+\!+}\cdots\mathbin{+\!+}P(u_k)$, is the required full output. Each pending root is non-null, and its [subtree](../../data-structure.md#subtree) is still unvisited. This is the pending-work form of [explicit-stack depth-first tree traversal](../../algorithm.md#explicit-stack-depth-first-tree-traversal).

One iteration discharges the first root's own label and replaces its remaining obligation by the left [subtree](../../data-structure.md#subtree) followed by the right [subtree](../../data-structure.md#subtree). The push order makes that precisely the new top-first pending order. Thus the [loop invariant](../../algorithm.md#loop-invariant) is preserved. The [loop variant](../../algorithm.md#loop-variant) is the sum of the numbers of [vertices](../../graph.md#vertex-graph-theory) in all pending [subtrees](../../data-structure.md#subtree); it decreases by exactly one per iteration, even if the number of [stack](../../data-structure.md#stack-data-structure) entries increases. When the [stack](../../data-structure.md#stack-data-structure) is empty there is no remaining output obligation, proving correctness and termination. This assumes a finite genuine [binary tree](../../data-structure.md#binary-tree) and, as permitted, sufficient [stack](../../data-structure.md#stack-data-structure) capacity. Each [vertex](../../graph.md#vertex-graph-theory) is pushed and popped once, giving **$\Theta(n)$ time** and $O(h+1)$ pending references for [binary tree](../../data-structure.md#binary-tree) height $h$.

## 5

↑ **Parent:** [Imperative programming resit](imperative-programming-resit.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

For [Chomp](../../game-theory.md#chomp), one representation is a Boolean [array](../../data-structure.md#array-data-structure) `occupied(y)(x)` with one entry per cell. The initial board has every entry true. For the noninitial board in the figure, the sets of occupied column indices in successive rows $y=0,1,\ldots,5$ are $\{0,1,2,3,4,5\}$, $\{0,1,2,3\}$, $\{0,1,2,3\}$, $\{0,1\}$, $\varnothing$, $\varnothing$; all other entries are false.

A more compact representation is the [monotone boundary representation of a grid order ideal](../../set.md#monotone-boundary-representation-of-a-grid-order-ideal): an [array](../../data-structure.md#array-data-structure) `row(y)` giving the number of occupied cells in row $y$. Occupied cells in a row always form a left prefix. The initial representation is $[6,6,6,6,6,6]$, and **the illustrated noninitial representation is $[6,4,4,2,0,0]$**, indexed upwards from row zero. Its total is $16$. These descriptions use the same coordinate orientation as the original figure; no source image is needed in the solution.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

Let the abstract state be the [set](../../set.md) $B$ of occupied coordinate pairs. For the Boolean [array](../../data-structure.md#array-data-structure), the [abstraction function](../../computer-science.md#abstraction-function) is $\alpha(occupied)=\{(x,y):occupied(y)(x)\}$. Its [representation invariant](../../computer-science.md#representation-invariant) requires an $N\times N$ Boolean [array](../../data-structure.md#array-data-structure) and the downward-closure property

$$
(x,y)\in B\ \Longrightarrow\ (i,j)\in B
\quad\text{whenever }0\leq i\leq x,\ 0\leq j\leq y.
$$

Thus $B$ is an [order ideal](../../set.md#order-ideal) for the coordinatewise [partial order](../../set.md#partially-ordered-set). Removing an upper-right rectangle preserves this property. The empty [set](../../set.md) is allowed after the losing move.

For the row-boundary [array](../../data-structure.md#array-data-structure), the [abstraction function](../../computer-science.md#abstraction-function) and [representation invariant](../../computer-science.md#representation-invariant) are

$$
\alpha(row)=\{(x,y):0\leq y<N,\ 0\leq x<row(y)\},
\qquad N\geq row(0)\geq\cdots\geq row(N-1)\geq0.
$$

The [array](../../data-structure.md#array-data-structure) has length $N$. Removing at $(x,y)$ replaces each `row(j)` for $j\geq y$ by $\min(row(j),x)$. Earlier rows are unchanged. This both implements the abstract removal and preserves the nonincreasing boundary.

Without a cached count, the Boolean representation takes $\Theta(N^2)$ for `Count`, $O(1)$ for `Legal`, $O(N^2)$ worst-case for `Move`, and $\Theta(N^2)$ for a full-grid `Display`. The boundary representation takes $\Theta(N)$ for `Count`, $O(1)$ for `Legal`, $O(N)$ worst-case for `Move`, and $\Theta(N^2)$ for the same full-grid `Display`. Their [space complexities](../../theoretical-computer-science.md#space-complexity) are respectively $\Theta(N^2)$ and $\Theta(N)$. A scalar cached total makes `Count` $O(1)$ in either representation if each move updates it consistently. The implementation below uses that cache with the boundary [array](../../data-structure.md#array-data-structure), so it achieves **constant-time `Count` and `Legal`, linear worst-case `Move`, and linear storage**. Full-grid output still takes quadratic time because it emits quadratic many cell positions.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Use the row boundary and cache its sum. The restriction on the initial total makes the fixed `Int` return type of `Count` meaningful; `Display` separately checks the requested single-digit coordinate range.
```
class Chomps(N: Int) {
  require(N > 0 && N.toLong * N.toLong <= Int.MaxValue.toLong)
  private val row = Array.fill(N)(N)
  private var remaining = N * N

  def Count(): Int = remaining

  def Legal(x: Int, y: Int): Boolean =
    0 <= x && x < N && 0 <= y && y < N && x < row(y)

  def Move(x: Int, y: Int): Unit = {
    require(Legal(x, y))
    var j = y
    while (j < N) {
      val next = math.min(row(j), x)
      remaining -= row(j) - next
      row(j) = next
      j += 1
    }
  }

  def Display(): Unit = {
    require(N < 10)
    var y = N - 1
    while (y >= 0) {
      print(y.toString + " ")
      var x = 0
      while (x < N) {
        print(if (x < row(y)) "* " else "  ")
        x += 1
      }
      println()
      y -= 1
    }
    print("  ")
    var x = 0
    while (x < N) {
      print(x.toString + " ")
      x += 1
    }
    println()
  }
}
```
The additional [representation invariant](../../computer-science.md#representation-invariant) is $remaining=\sum_{j=0}^{N-1}row(j)$. It initially holds. For `Move`, write $row_0$ for the boundary at entry. The [loop invariant](../../algorithm.md#loop-invariant) says that rows before $y$ are unchanged, rows from $y$ through $j-1$ equal $\min(row_0(i),x)$, rows from $j$ onwards still equal $row_0(i)$, and `remaining` equals the sum of the current entries. The [loop variant](../../algorithm.md#loop-variant) is $N-j$. Each iteration subtracts exactly the newly removed number of cells from the cache. At exit all affected rows are truncated as required, and the nonincreasing boundary is restored. During a partially completed update it need not be nonincreasing; only the stated [loop invariant](../../algorithm.md#loop-invariant), not the full externally visible [representation invariant](../../computer-science.md#representation-invariant), is required internally.

For `Display`, the outer [loop invariant](../../algorithm.md#loop-invariant) says that exactly the rows with indices greater than $y$ have been printed correctly; its [loop variant](../../algorithm.md#loop-variant) is $y+1$. The inner [loop invariant](../../algorithm.md#loop-invariant) says that the current row's first $x$ cells have been emitted correctly; its [loop variant](../../algorithm.md#loop-variant) is $N-x$. The final labels loop has the same decreasing [loop variant](../../algorithm.md#loop-variant), and prints exactly the first $x$ column labels before each iteration. [Short-circuit evaluation](../../programming-language.md#short-circuit-evaluation) in `Legal` checks both coordinates before indexing. **An illegal `Move` fails before changing the board.**

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Keep the same player until an occupied, in-range cell is supplied:
```
val board = new Chomps(6)
var player = 1
while (board.Count() > 0) {
  board.Display()
  var x = -1
  var y = -1
  while (!board.Legal(x, y)) {
    println("Player " + player + ": enter x, then y")
    try {
      x = scala.io.StdIn.readInt()
      y = scala.io.StdIn.readInt()
    } catch {
      case _: NumberFormatException =>
        x = -1
        y = -1
    }
    if (!board.Legal(x, y)) println("Choose an occupied cell")
  }
  board.Move(x, y)
  if (board.Count() == 0)
    println("Player " + player + " loses; player " + (3 - player) + " wins")
  else player = 3 - player
}
```
The outer [loop invariant](../../algorithm.md#loop-invariant) is that `player` is the next player's number, either one or two, and the board is the result of the accepted moves. The inner [loop invariant](../../algorithm.md#loop-invariant) says that the board and player have not changed; rejected inputs do not consume a turn. Assuming the input source continues and eventually supplies a legal coordinate pair, the inner loop finishes. No program can guarantee that a user stops entering illegal moves, so that interaction assumption is necessary.

Every accepted move removes at least its selected token, so the outer [loop variant](../../algorithm.md#loop-variant) is `Count()`, a decreasing nonnegative [integer](../../integer.md). In a nonempty [order ideal](../../set.md#order-ideal), $(0,0)$ is occupied. Removing it removes the entire board, whereas a move at any other cell leaves it. Therefore **the player making the final move is exactly the loser**; the code reports that player before changing the turn. At most $36$ legal moves occur.

## 6

↑ **Parent:** [Imperative programming resit](imperative-programming-resit.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The return types suggest an **immutable [sequence](../../sequence-and-series.md#sequence) implementation**: insertion and deletion return a new `Sequence[A]`, while the receiver can remain unchanged. A mutable implementation would more naturally return `Unit` for in-place edits, though it could return itself. Thus the signatures are evidence of an intended [immutable object](../../programming-language.md#immutable-object) implementation, not a logical guarantee. For the snapshot solution below, require that returned and retained `Sequence` values really are immutable. The owning `SlideSuite` can still have a mutable variable referring to its current immutable [sequence](../../sequence-and-series.md#sequence).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Represent an applied edit by a [command pattern](../../programming-language.md#command-pattern) object with `undo` and `redo`. Use zero-based positions. For `move(from,to)`, define `to` as the slide's index in the resulting [sequence](../../sequence-and-series.md#sequence); it is in $[0,n)$ for a presentation of length $n$. Removing the slide first and then inserting at that index implements this convention in either direction.
```
trait Change {
  // Pre: this is the most recent applied change not yet undone.
  def undo(): Unit
  // Pre: this is the next change on the redo history.
  def redo(): Unit
}

class SlideSuite(initial: Sequence[Slide]) {
  private var slides = initial

  private def insertRaw(i: Int, x: Slide): Unit = {
    slides = slides.insert(i, x)
  }

  private def deleteRaw(i: Int): Unit = {
    slides = slides.delete(i)
  }

  private def moveRaw(from: Int, to: Int): Unit = {
    val x = slides.elementAt(from)
    slides = slides.delete(from).insert(to, x)
  }

  def insert(i: Int, x: Slide): Change = {
    insertRaw(i, x)
    new Change {
      def undo(): Unit = deleteRaw(i)
      def redo(): Unit = insertRaw(i, x)
    }
  }

  def delete(i: Int): Change = {
    val x = slides.elementAt(i)
    deleteRaw(i)
    new Change {
      def undo(): Unit = insertRaw(i, x)
      def redo(): Unit = deleteRaw(i)
    }
  }

  def move(from: Int, to: Int): Change = {
    moveRaw(from, to)
    new Change {
      def undo(): Unit = moveRaw(to, from)
      def redo(): Unit = moveRaw(from, to)
    }
  }
}
```
`Sequence` and `Slide` are the supplied external types. Valid insertion positions are $0\leq i\leq n$, deletion positions are $0\leq i<n$, and both move positions are valid indices of the original length. These are the permitted unchecked argument [preconditions](../../algorithm.md#precondition). The private raw operations perform exactly their named state transformation and do not create history entries. A move to the same index is a legitimate no-op.

The deleted slide must be saved because its index alone cannot reconstruct it. By contrast, insertion already receives the slide to retain. For a move, the inverse of moving the slide from `from` to its final index `to` is to remove it at `to` and reinsert it at `from`; all other slides retain their relative order. Thus each returned object satisfies **`undo` restores the state immediately before the edit, and `redo` restores the state immediately after it**, under the stated history protocol.

A controller can enforce the protocol with two [stacks](../../data-structure.md#stack-data-structure). This code records changes that have already been executed:
```
class History {
  private var done = List.empty[Change]
  private var undone = List.empty[Change]

  // Pre: c is a fresh, already-applied change of this history's suite.
  def record(c: Change): Unit = {
    done = c :: done
    undone = Nil
  }

  def undo(): Unit = {
    require(done.nonEmpty)
    val c = done.head
    c.undo()
    done = done.tail
    undone = c :: undone
  }

  def redo(): Unit = {
    require(undone.nonEmpty)
    val c = undone.head
    c.redo()
    undone = undone.tail
    done = c :: done
  }
}
```
For example, `history.record(suite.move(i,j))` executes and records one move. The [representation invariant](../../computer-science.md#representation-invariant) says that `done` contains applied changes in reverse application order, while `undone` contains undone changes in the next-redo order, all belonging to the same suite. A fresh edit clears the redo branch. Undo and redo transfer one command between the two heads, so they neither skip intervening edits nor generate new history records. Unrecorded external edits and out-of-order use of old command objects are excluded by this protocol.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/i">i</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6/c/i)

Replace edit-specific inverse information by before/after snapshots implementing the [Memento pattern](../../programming-language.md#memento-pattern). The same `Change` and `History` interfaces still work. A complete alternative suite is:
```
class SnapshotSlideSuite(initial: Sequence[Slide]) {
  private var slides = initial

  private def changeTo(after: Sequence[Slide]): Change = {
    val before = slides
    slides = after
    new Change {
      def undo(): Unit = { slides = before }
      def redo(): Unit = { slides = after }
    }
  }

  def insert(i: Int, x: Slide): Change =
    changeTo(slides.insert(i, x))

  def delete(i: Int): Change =
    changeTo(slides.delete(i))

  def move(from: Int, to: Int): Change = {
    val x = slides.elementAt(from)
    changeTo(slides.delete(from).insert(to, x))
  }
}
```
By-value evaluation computes `after` without changing `slides`, then `changeTo` captures the still-current `before` and installs the new value. The `val` bindings inside each call are stable snapshots, rather than later reads of a mutable variable. Under the same chronological history [preconditions](../../algorithm.md#precondition), **undo and redo are constant-time reference assignments**. This is the [Memento pattern](../../programming-language.md#memento-pattern) applied to an immutable [sequence](../../sequence-and-series.md#sequence). Retaining a reference to an in-place-mutated [sequence](../../sequence-and-series.md#sequence) would not save its old state. The snapshot covers slide order and membership; it does not promise to undo unrelated mutations inside a `Slide` object.

<h4 id="6/c/ii">ii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/c/ii)

**Not necessarily: [structural sharing](../../data-structure.md#structural-sharing) can make snapshots cheap, but the trait alone gives no storage guarantee.** With a [persistent data structure](../../data-structure.md#persistent-data-structure), unchanged portions of old and new [sequences](../../sequence-and-series.md#sequence) can be shared safely. Saving two root references costs $O(1)$ additional space per edit, and adjacent history entries commonly refer to the same intermediate version. With an appropriate balanced persistent [tree](../../tree-graph-theory.md), each positional edit may add only $O(\log n)$ new [vertices](../../graph.md#vertex-graph-theory), giving approximately $O(n+h\log n)$ storage for $h$ retained edits of comparable presentation size, plus references to slides.

There are important qualifications. A fully copied immutable [array](../../data-structure.md#array-data-structure) may allocate $\Theta(n)$ per edit and use $\Theta(hn)$ across its history. A persistent [linked list](../../data-structure.md#linked-list) shares suffixes but may copy a long prefix for a late positional edit. Moreover, snapshot history keeps old versions alive that an edit-specific inverse representation might otherwise release. Consequently a significant increase is possible with some implementations or workloads; it is not forced by saving `Sequence` references, and it cannot be ruled out from the interface alone.

## 7

↑ **Parent:** [Imperative programming resit](imperative-programming-resit.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

[Programming language polymorphism](../../programming-language.md#programming-language-polymorphism) lets one expression or operation work with values of different types or concrete representations. In [object-oriented programming](../../programming-language.md#object-oriented-programming), [subtype polymorphism](../../programming-language.md#subtype-polymorphism) lets a reference of an interface or superclass type designate instances of different implementing [software classes](../../programming-language.md#class-programming). A call through that reference uses [dynamic dispatch](../../programming-language.md#dynamic-dispatch) to select the receiver's overriding [object method](../../programming-language.md#object-method). For example, a routine taking `Book` can invoke `recall` on a linked-list or an array-based implementation while depending only on the common abstract contract.

[Parametric polymorphism](../../programming-language.md#parametric-polymorphism) is another form: the type parameter in `FiniteDist[T]` lets the same interface describe distributions over [Booleans](../../programming-language.md#boolean-data-type), [integers](../../integer.md) or characters. A generic method introduces a further type parameter when its output type differs. [Method overloading](../../programming-language.md#method-overloading), in contrast, supplies several statically selected signatures with one name; it should not be confused with receiver-dependent [dynamic dispatch](../../programming-language.md#dynamic-dispatch). Correct substitutability also requires implementations to respect the common behavioral contract, not merely to share method names.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/i">i</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/i/solution">Solution</h5>

↑ **Parent:** [I](#7/b/i)

Implement the [Bernoulli distribution](../../discrete-probability-distribution.md#bernoulli-distribution), taking special care that a zero-mass outcome is excluded from the [support of a probability distribution](../../probability-distribution.md#support-of-a-probability-distribution):
```
class Flip(p: Double) extends FiniteDist[Boolean] {
  require(!p.isNaN && 0.0 <= p && p <= 1.0)

  def getDom: List[Boolean] =
    if (p == 0.0) List(false)
    else if (p == 1.0) List(true)
    else List(true, false)

  def getProb(x: Boolean): Double =
    if (x) p else 1.0 - p
}
```
The [precondition](../../algorithm.md#precondition) excludes NaN and all values outside $[0,1]$, including infinities. The two masses are nonnegative and sum mathematically to one. **Endpoint domains are singleton lists**, while an interior parameter lists both outcomes exactly once. Treating `getDom` as always containing both [Booleans](../../programming-language.md#boolean-data-type) would violate its positive-support contract at the endpoints.

<h4 id="7/b/ii">ii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/b/ii)

The inclusive interval is nonempty exactly when **$l\leq u$**. Reject $l>u$ with a failed [precondition](../../algorithm.md#precondition), rather than assigning a nonexistent normalization to an empty interval. Compute its width in `Long` before taking a reciprocal:
```
class Uniform(l: Int, u: Int) extends FiniteDist[Int] {
  require(l <= u, "Empty uniform interval")
  private val width = u.toLong - l.toLong + 1L
  private val mass = 1.0 / width.toDouble

  def getProb(x: Int): Double =
    if (l <= x && x <= u) mass else 0.0

  def getDom: List[Int] = {
    var x = l.toLong
    var rev = List.empty[Int]
    while (x <= u.toLong) {
      rev = x.toInt :: rev
      x += 1L
    }
    rev.reverse
  }
}
```
The [loop invariant](../../algorithm.md#loop-invariant) says that $l\leq x\leq u+1$ and `rev` contains exactly the [integers](../../integer.md) $l,\ldots,x-1$ in reverse order. The [loop variant](../../algorithm.md#loop-variant) is $u-x+1$ while the guard is true. `Long` handles both the full interval width $2^{32}$ and the increment past `Int.MaxValue`. At exit, reversing yields each support value once. All support values have mass $1/(u-l+1)$, so their exact sum is one; `Double` approximates that [rational number](../../number-theory.md#rational-number). Very large valid domains require correspondingly large lists and sufficient memory; that resource issue does not make the mathematical endpoint values invalid.

<h4 id="7/b/iii">iii</h4>

↑ **Parent:** [B](#7/b)

<h5 id="7/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/b/iii)

Use relative character frequencies, an [empirical distribution](../../information-theory.md#type-information-theory). A nonempty [string](../../foundations-of-mathematics.md#string) is required because an empty sample has no normalized frequency distribution:
```
class DistFromString(s: String) extends FiniteDist[Char] {
  require(s != null && s.nonEmpty, "A nonempty string is required")
  private val chars = s.toList
  private val domain = chars.distinct

  def getDom: List[Char] = domain

  def getProb(c: Char): Double =
    chars.count(_ == c).toDouble / s.length.toDouble
}
```
`distinct` removes repeated support entries without changing which characters occur. Every returned domain element has positive frequency, and every absent character has frequency zero. The occurrence counts partition the [string](../../foundations-of-mathematics.md#string)'s character positions, so their total is `s.length`, establishing normalization. **For `Scala`, the masses are $2/5$ for `a` and $1/5$ each for `S`, `c` and `l`.** The character units here are exactly the `Char` values supplied by `s.toList`; the interface does not specify a different notion of displayed text characters. The code has no explicit loop beyond the specified library traversals.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

Add the following concrete method inside `FiniteDist[T]`. It forms a [pushforward of a finite probability distribution](../../probability-distribution.md#pushforward-of-a-finite-probability-distribution), adding the masses of outcomes that map to the same result:
```
def map[U](f: T => U): FiniteDist[U] = {
  val source = getDom
  val weighted = source.map(x => (f(x), getProb(x)))
  val target = weighted.map(_._1).distinct
  new FiniteDist[U] {
    def getDom: List[U] = target
    def getProb(y: U): Double =
      weighted.filter(pair => pair._1 == y).map(_._2).sum
  }
}
```
The input [finite probability distribution](../../probability-distribution.md#finite-probability-distribution) is assumed to satisfy its interface, with stable masses during construction, and `f` must be a total deterministic [pure function](../../programming-language.md#pure-function) on its finite support. Output values need stable equality consistent with the mathematical equality being modeled; mutating equality-relevant fields afterwards would undermine any finite-support implementation. Computing `weighted` once also prevents later queries from re-evaluating `f` inconsistently.

Every source support element appears once in `weighted`. The `distinct` operation lists each image value once; every such image has a positive mathematical mass because it has a positive-mass preimage. For each $y$, filtering selects exactly those $x$ with $f(x)=y$, so `getProb(y)` is the required sum, with an empty sum of zero off the image. The fibers form a [set partition](../../combinatorics.md#set-partition) of the original support, giving

$$
\sum_y p_2(y)=\sum_y\sum_{x:f(x)=y}p_1(x)=\sum_xp_1(x)=1.
$$

Thus **colliding images have their probabilities added, not overwritten**. For a concrete check, mapping a uniform distribution on $\{0,1,2,3\}$ by parity gives probability $1/2$ to each of $0,1$; mapping every source value to one constant gives a singleton domain with total mass one. [Floating-point rounding](../../floating-point-arithmetic.md#floating-point-rounding) can make a computed total differ slightly from one; the proof is for exact mathematical masses, and the representation uses `Double` approximations.

## 8

↑ **Parent:** [Imperative programming resit](imperative-programming-resit.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

[Test-driven development](../../computer-science.md#test-driven-development) interleaves three small steps: write a test expressing the next required behavior and observe that it fails, implement enough behavior to make it pass, then improve the code's structure while keeping the tests passing. The retained tests become a regression suite. For example, before implementing a book deletion, test that deleting an existing contact removes it and returns true; later add the absent-name case. Each test guides a small implementation step rather than waiting for a finished component.[What is TDD?: interleaving unit tests, implementation and refactoring in a short cycle](../../computer-science-bibliography.md#test-driven-development-in-the-agile-alliance-glossary)

Compared with a traditional write-the-component-then-test workflow, **tests guide the design before each increment is implemented**. This does not imply that all non-TDD testing is postponed until a whole product is finished, or that TDD eliminates broader integration testing.

The test-first behavioral core is naturally [black-box testing](../../computer-science.md#black-box-testing): expected outcomes come from the operation's contract. Later tests can use internal control flow or representation cases, becoming [white-box testing](../../computer-science.md#white-box-testing). Thus a complete practice can use **a mixture, with mainly contract-based black-box tests driving the next behavior**. The classification depends on how test cases are chosen, not on whether the programmer personally knows the implementation. Passing a finite suite is not a proof of universal correctness.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

In the [Observer pattern](../../programming-language.md#observer-pattern), a subject maintains subscriptions through a common observation interface. Interested observers register and unregister; when a relevant state change occurs, the subject sends a notification, and each observer runs its own reaction. Notifications can carry the new information directly or prompt the observer to query the subject's coherent updated state.

This fits an [event-driven programming](../../programming-language.md#event-driven-programming) interface in which one model can have several independently changing views: a displayed conversion, a chart or a status indicator can react to the same model change. It avoids hard-coding calls to every concrete view inside the subject, which would couple domain logic to presentation details and require editing the subject whenever another view is added. **The subject depends on the observer interface rather than every concrete observer class.**

The design still needs subscription cleanup and an update policy. Mutual notifications can create a feedback loop or a [reentrant event handler](../../programming-language.md#reentrant-event-handler), while an observer that reacts halfway through a state change can see inconsistent data. Publishing only coherent changes and controlling derived display updates address those problems; the pattern alone does not automatically solve them.

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

In [Scala Swing](../../programming-language.md#scala-swing), a `Publisher` is the observable subject and a `Reactor` supplies an observer's reactions. A reactor calls `listenTo(pounds, euros, rate)` to subscribe to the relevant publishing components. It adds a [partial function](../../function.md#partial-function) from events to actions with `reactions += { case ... => ... }`; unmatched event types need no action. When a publisher calls `publish(e)`, subscribed reactions that handle that event are notified. Calling `deafTo` removes subscriptions that are no longer wanted.[README, About scala-swing: Publisher/Reactor, listenTo and reactions; archived Reactor API: deafTo](../../computer-science-bibliography.md#scala-swing-event-system-documentation)

The publisher does not need to know the concrete frame or its currency-conversion code. A `TextField` supplies the relevant editing events, and the frame's reaction distinguishes the source field using `EditDone(source)`. **Both registration and a matching reaction are needed**: installing a case handler without subscribing does not establish the notification path. The observer logic should update the conversion model once and then refresh the other fields from that coherent state.

<h3 id="8/d">d</h3>

↑ **Parent:** [8](#8)

<h4 id="8/d/solution">Solution</h4>

↑ **Parent:** [D](#8/d)

Let the committed model be amounts $p,e$ and an exchange rate $r$, with [invariant](../../mathematics.md#invariant-mathematics) $e=pr$. Editing pounds keeps the rate and computes euros; editing euros keeps the rate and computes pounds; editing the rate keeps pounds and computes euros. A usable rate must be strictly positive, and every accepted [floating-point number](../../floating-point-arithmetic.md#floating-point-number) and derived result must be finite. Negative amounts are allowed. Rejecting invalid text preserves the last committed model.

Insert the following members inside the supplied `MainFrame`, after the three fields have been initialized. Its existing layout can remain as written:
```
private var p = 10.0
private var e = 11.5
private var r = 1.15
private var refreshing = false

private def finite(x: Double): Boolean = !x.isNaN && !x.isInfinity

private def showModel(): Unit = {
  refreshing = true
  try {
    pounds.text = java.lang.String.format(java.util.Locale.ROOT, "%.2f", Double.box(p))
    euros.text = java.lang.String.format(java.util.Locale.ROOT, "%.2f", Double.box(e))
    rate.text = r.toString
  } finally {
    refreshing = false
  }
}

private def edit(source: TextField): Unit = {
  try {
    val v = source.text.trim.toDouble
    if (finite(v)) {
      var nextP = p
      var nextE = e
      var nextR = r
      if (source eq pounds) {
        nextP = v
        nextE = v * r
      } else if (source eq euros) {
        nextE = v
        nextP = v / r
      } else if (source eq rate) {
        nextR = v
        nextE = p * v
      }
      if (nextR > 0.0 && finite(nextP) && finite(nextE) && finite(nextR)) {
        p = nextP
        e = nextE
        r = nextR
      }
    }
  } catch {
    case _: NumberFormatException => ()
  }
  showModel()
}

listenTo(pounds, euros, rate)
reactions += {
  case EditDone(source) if !refreshing => edit(source)
}
```
The [invariant](../../mathematics.md#invariant-mathematics) is interpreted with the usual [floating-point rounding](../../floating-point-arithmetic.md#floating-point-rounding) in multiplication and division. All candidate values are calculated before committing any of them, so invalid text, zero/negative rates, NaN, infinity and [floating-point overflow](../../floating-point-arithmetic.md#floating-point-overflow) leave the old model intact. The committed `r` remains positive, so euro-to-pound division is defined. Using a fixed formatting locale keeps the decimal separator compatible with `toDouble`. The displayed amounts are rounded to two decimal places, while the model retains their full available precision. The rate is not forcibly rounded to two places, which could otherwise turn a valid small positive rate into displayed zero.

The `refreshing` guard prevents synchronous derived-field notifications from recursively committing another edit. `EditDone` is an edit-completion event, not a request to react to every partial keystroke; pressing the field's completion action is enough to trigger the conversion. If a particular UI additionally needs live updates, it can subscribe to the appropriate text-change events with the same validation and authoritative-source policy. The supplied API and archived [Scala Swing](../../programming-language.md#scala-swing) documentation suffice for the requested completion-event implementation; no unidentified practical library is required.[Publisher/Reactor subscription design; archived Swing event API: EditDone carries its source TextField](../../computer-science-bibliography.md#scala-swing-event-system-documentation)

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
