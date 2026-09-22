# Imperative programming

↑ **Parent:** [2018](../2018.md)

Source paper: [released examination archive, member 2017/T/a10098w1.pdf](https://www.whatdotheyknow.com/request/ba_computer_science_past_papers/response/2577745/attach/2/202402%20183%20CS%20Papers.zip?cookie_passthrough=1). The printed cover dates this examination to Wednesday 13 June 2018, Trinity Term; the archive directory does not determine its year. All eight questions and every printed option are covered. Examples use [Scala](../../programming-language.md#scala) 2 syntax. Arithmetic [loop invariants](../../algorithm.md#loop-invariant) describe exact arithmetic unless a [floating-point arithmetic](../../floating-point-arithmetic.md) qualification is stated.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
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
  - [d](#4/d)
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [i](#5/d/i)
      - [Solution](#5/d/i/solution)
    - [ii](#5/d/ii)
      - [Solution](#5/d/ii/solution)
    - [iii](#5/d/iii)
      - [Solution](#5/d/iii/solution)
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
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
  - [d](#7/d)
    - [Solution](#7/d/solution)
  - [e](#7/e)
    - [Solution](#7/e/solution)
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

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

Keep a running [product](../../arithmetic.md#product-of-numbers) of the fixed base. In particular, `1.0/n` uses [floating-point arithmetic](../../floating-point-arithmetic.md), avoiding the truncation that [integer division](../../arithmetic.md#integer-division) would introduce:
```
def eaLinear(n: Int): Double = {
  require(n > 0)
  val base = 1.0 + 1.0 / n.toDouble
  var k = 0
  var result = 1.0
  while (k < n) {
    result *= base
    k += 1
  }
  result
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $0\leq k\leq n$ and $result=base^k$. Initially the empty [product](../../arithmetic.md#product-of-numbers) is one. Multiplication by `base` and incrementing `k` preserve the [invariant](../../mathematics.md#invariant-mathematics). The [loop variant](../../algorithm.md#loop-variant) $n-k$ decreases by one. On exit $k=n$, so **the result is $e_a(n)$**, with exactly $n$ multiplications and $O(n)$ [time complexity](../../theoretical-computer-science.md#time-complexity). With `Double`, the operational result is the rounded recurrence, rather than an exact real power; this distinction applies to the next two power computations too.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Use [exponentiation by squaring](../../number-theory.md#exponentiation-by-squaring), retaining the unprocessed exponent in `k`:
```
def eaBinary(n: Int): Double = {
  require(n > 0)
  var base = 1.0 + 1.0 / n.toDouble
  var k = n
  var result = 1.0
  while (k > 0) {
    if ((k & 1) != 0) result *= base
    k = k / 2
    if (k > 0) base *= base
  }
  result
}
```
Writing $A=1+1/n$, the [loop invariant](../../algorithm.md#loop-invariant) is $k\geq0$ and $result\,base^k=A^n$. If the old exponent is $2q+b$, $b\in\{0,1\}$, multiplying the accumulator by $base^b$ and replacing the remaining power by $(base^2)^q$ preserves the [invariant](../../mathematics.md#invariant-mathematics). When $q=0$, the unused squaring may be omitted. The nonnegative [integer](../../integer.md) `k` is a [loop variant](../../algorithm.md#loop-variant), since $\lfloor k/2\rfloor<k$ for $k>0$. At exit the remaining power is one, giving **$result=e_a(n)$**. There are $\lfloor\log_2n\rfloor+1$ iterations, at most one accumulator multiplication and one squaring per iteration, hence $O(\log n)$ multiplications and [constant space](../../theoretical-computer-science.md#constant-space).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Generate each reciprocal [factorial](../../combinatorics.md#factorial) from the preceding one, instead of recomputing a [factorial](../../combinatorics.md#factorial) for every summand:
```
def eb(n: Int): Double = {
  require(n >= 0)
  var i = 0
  var term = 1.0
  var sum = 1.0
  while (i < n) {
    i += 1
    term /= i.toDouble
    sum += term
  }
  sum
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $0\leq i\leq n$, $term=1/i!$, and $sum=\sum_{j=0}^{i}1/j!$. Initially $i=0$ and $0!=1$. The division produces $1/(i+1)!$, which is then added to the previous partial [sum](../../arithmetic.md#sum). The [loop variant](../../algorithm.md#loop-variant) is $n-i$. Consequently **the returned value is $e_b(n)$**, using exactly $n$ divisions and $n$ additions, no multiplications, and $O(n)$ [time complexity](../../theoretical-computer-science.md#time-complexity). The slightly weaker [precondition](../../algorithm.md#precondition) also permits the useful zero-term boundary case. For `Double`, small positive terms eventually cease to change `sum` because of [floating-point rounding](../../floating-point-arithmetic.md#floating-point-rounding).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

First rearrange the ratios so that the intermediate powers remain moderate:

$$
e_c(n)=(n+1)\left(1+\frac1n\right)^n-n\left(1+\frac1{n-1}\right)^{n-1}.
$$

This avoids separately forming enormous powers such as $n^n$. Perform the two instances of [exponentiation by squaring](../../number-theory.md#exponentiation-by-squaring) in one [while loop](../../programming-language.md#while-loop), using [coupled binary exponentiation](../../number-theory.md#coupled-binary-exponentiation):
```
def ec(n: Int): Double = {
  require(n > 1)
  val dn = n.toDouble
  var x = 1.0 + 1.0 / dn
  var y = 1.0 + 1.0 / (dn - 1.0)
  var k = n
  var l = n - 1
  var p = 1.0
  var q = 1.0
  while (k > 0 || l > 0) {
    if (k > 0) {
      if ((k & 1) != 0) p *= x
      k /= 2
      if (k > 0) x *= x
    }
    if (l > 0) {
      if ((l & 1) != 0) q *= y
      l /= 2
      if (l > 0) y *= y
    }
  }
  (dn + 1.0) * p - dn * q
}
```
With $A=1+1/n$ and $B=1+1/(n-1)$, the [loop invariant](../../algorithm.md#loop-invariant) is $k,l\geq0$, $p x^k=A^n$, and $q y^l=B^{n-1}$. Each active branch preserves its own power identity by the parity argument in part (a)(ii), and an inactive branch changes nothing. The [loop variant](../../algorithm.md#loop-variant) is the mathematical [integer](../../integer.md) $k+l$, which need not be computed in a fixed-width variable: it decreases whenever either exponent is positive. At exit $p=A^n$, $q=B^{n-1}$, proving **the returned expression is $e_c(n)$**. There are $O(\log n)$ iterations, at most four loop multiplications each, and two final multiplications. Converting `n` before adding one avoids [integer overflow](../../programming-language.md#integer-overflow) at `Int.MaxValue`.

The rearrangement avoids [floating-point overflow](../../floating-point-arithmetic.md#floating-point-overflow) in the original powers, but subtraction still combines two quantities of order $n$ to obtain one of order one. [Catastrophic cancellation](../../floating-point-arithmetic.md#catastrophic-cancellation) can amplify their accumulated [roundoff error](../../numerical-analysis.md#round-off-error). The mathematical $O(n^{-2})$ approximation error therefore does not imply that the `Double` implementation improves indefinitely as `n` grows.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

**Choose the reciprocal-[factorial](../../combinatorics.md#factorial) summation `eb` for asymptotically high accuracy**, counting multiplications and divisions as arithmetic work. For tolerance $\epsilon$, linear powering in part (a)(i) takes $O(\epsilon^{-1})$ multiplications; [binary exponentiation](../../number-theory.md#exponentiation-by-squaring) in part (a)(ii) reduces this to $O(\log(1/\epsilon))$. Part (c) also has $O(\log(1/\epsilon))$ arithmetic work, since its required $n$ grows like $\epsilon^{-1/2}$, though its constants and [cancellation error](../../numerical-analysis.md#cancellation-error) differ.

By the [reciprocal-factorial series remainder bound](../../calculus.md#reciprocal-factorial-series-remainder-bound), the omitted positive tail satisfies

$$
0<e-e_b(n)=\sum_{j=n+1}^{\infty}\frac1{j!}\leq\frac1{(n+1)!}\sum_{r=0}^{\infty}\frac1{(n+2)^r}=\frac{n+2}{(n+1)(n+1)!}.
$$

Thus the [factorial](../../combinatorics.md#factorial) denominator grows much faster than an exponential in the number of iterations. For $d$ decimal places, setting $\epsilon$ of order $10^{-d}$ gives $n=\Theta(d/\log d)$ by [Stirling's approximation](../../real-analysis.md#stirling-formula), rather than $\Theta(d)$ binary-power arithmetic steps. This is a comparison in an exact-arithmetic operation-count model; the stated [Big O notation](../../real-analysis.md#big-o-notation) does not determine the exact winner for every small tolerance. Taken literally, `eb` uses zero multiplications and only divisions. Fixed [double-precision floating-point format](../../floating-point-arithmetic.md#double-precision-floating-point-format) cannot deliver arbitrarily many correct decimal places, and the precision-dependent cost of [arbitrary-precision arithmetic](../../arithmetic.md#arbitrary-precision-arithmetic) is a separate issue.

## 2

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

[Linear search](../../algorithm.md#linear-search) examines successive entries until a match or a stopping condition is reached; in the worst case it inspects $n$ entries. [Binary search](../../algorithm.md#binary-search) uses a [sorted array](../../data-structure.md#sorted-array) to discard about half of the remaining candidates after each comparison, requiring $O(\log(n+1))$ comparisons. Its logarithmic guarantee also requires constant-cost indexed access, as supplied by an [array](../../data-structure.md#array-data-structure); the same index operations on a [linked list](../../data-structure.md#linked-list) would not be constant-cost.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Return the [lower-bound search](../../algorithm.md#lower-bound-search) boundary, permitting both zero and the [array](../../data-structure.md#array-data-structure) length:
```
def lowerBound(a: Array[Int], x: Int): Int = {
  require(a != null) // a is nondecreasing
  var lo = 0
  var hi = a.length
  while (lo < hi) {
    val mid = lo + (hi - lo) / 2
    if (a(mid) < x) lo = mid + 1
    else hi = mid
  }
  lo
}
```
The [precondition](../../algorithm.md#precondition) includes nondecreasing order. The [loop invariant](../../algorithm.md#loop-invariant) is

$$
0\leq lo\leq hi\leq n,\qquad a[0..lo)<x,\qquad x\leq a[hi..n).
$$

Initially both excluded ranges are empty. If $a(mid)<x$, sortedness justifies excluding every position through `mid`; otherwise it justifies excluding every position from `mid` onwards. The [loop variant](../../algorithm.md#loop-variant) $hi-lo$ is a nonnegative [integer](../../integer.md) that strictly decreases. When the old width is positive, `mid` is a valid [array index](../../data-structure.md#array-index). The midpoint expression avoids adding two potentially large indices. At exit $lo=hi$, so **`lo` satisfies the required partition**, including when $n=0$. Each new width is at most half the old width, rounded down; this gives $O(\log(n+1))$ [time complexity](../../theoretical-computer-science.md#time-complexity) and [constant space](../../theoretical-computer-science.md#constant-space), conventionally $O(\log n)$ for nontrivial sizes.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A second [binary search](../../algorithm.md#binary-search) locates the first entry strictly greater than `x`:
```
def upperBound(a: Array[Int], x: Int): Int = {
  require(a != null) // a is nondecreasing
  var lo = 0
  var hi = a.length
  while (lo < hi) {
    val mid = lo + (hi - lo) / 2
    if (a(mid) <= x) lo = mid + 1
    else hi = mid
  }
  lo
}

def equalRange(a: Array[Int], x: Int): (Int, Int) =
  (lowerBound(a, x), upperBound(a, x))
```
For [upper-bound search](../../algorithm.md#upper-bound-search), the [loop invariant](../../algorithm.md#loop-invariant) is $0\leq lo\leq hi\leq n$, $a[0..lo)\leq x$, and $x<a[hi..n)$; its [loop variant](../../algorithm.md#loop-variant) is again $hi-lo$. The same midpoint and sortedness arguments prove preservation, termination and $O(\log(n+1))$ [time complexity](../../theoretical-computer-science.md#time-complexity). The first [binary search](../../algorithm.md#binary-search) in part (b) already has its own [loop invariant](../../algorithm.md#loop-invariant) and [loop variant](../../algorithm.md#loop-variant).

Let the two boundaries be $i,j$. There cannot be a value greater than $x$ before the first value at least $x$, so $i\leq j$. Every entry between them is simultaneously at least and at most $x$, hence equals $x$. Entries before $i$ are smaller and entries at or after $j$ are larger, so the interval cannot be extended at either end. This proves the [equal-range search](../../algorithm.md#equal-range-search) result is maximal. **If `x` is absent, `i == j`, both equal to its insertion position**; this can be zero, $n$, or an interior gap. Two logarithmic searches still have logarithmic total [time complexity](../../theoretical-computer-science.md#time-complexity). Computing an upper boundary as `lowerBound(a, x+1)` would introduce an unnecessary [integer overflow](../../programming-language.md#integer-overflow) bug at the largest [integer](../../integer.md).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

[Black-box testing](../../computer-science.md#black-box-testing) chooses inputs and expected outputs from the public specification without using the implementation's control structure. [Equivalence class testing](../../computer-science.md#equivalence-partitioning) partitions the input space into classes expected to exercise similar specified behavior, then chooses representatives; boundary cases test where that behavior changes. For [equal-range search](../../algorithm.md#equal-range-search), use these concrete representatives:

- Empty [array](../../data-structure.md#array-data-structure): `([], 4)` gives **`(0,0)`**.
- One entry, with the target below, equal, and above it: `([4],3)`, `([4],4)`, `([4],5)` give **`(0,0)`, `(0,1)`, `(1,1)`**.
- An absent interior value: `([1,3,5],4)` gives **`(2,2)`**.
- One interior match: `([1,3,5],3)` gives **`(1,2)`**.
- A repeated interior block: `([1,3,3,3,5],3)` gives **`(1,4)`**.
- A repeated block touching the left or right boundary: `([3,3,5],3)` and `([1,3,3],3)` give **`(0,2)`** and **`(1,3)`**.
- Every entry equal: `([3,3,3],3)` gives **`(0,3)`**; targets two and four give **`(0,0)`** and **`(3,3)`**.
- Extreme keys: `([Int.MinValue,0,Int.MaxValue],Int.MaxValue)` gives **`(2,3)`**, and searching for `Int.MinValue` gives **`(0,1)`**.

For each result independently check $0\leq i\leq j\leq n$, the strict inequalities outside the returned interval, and equality inside it. Unsorted inputs violate the [precondition](../../algorithm.md#precondition); they are not ordinary members of the specified valid-input classes. [Software testing](../../computer-science.md#software-testing) supplies evidence about implementations, while the [loop invariant](../../algorithm.md#loop-invariant) proof explains correctness for every valid input.

## 3

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [list header](../../data-structure.md#list-header) is a permanent dummy [linked list node](../../data-structure.md#linked-list-node), distinct from the ordinary elements. It gives a stable reference to the [linked list](../../data-structure.md#linked-list) and can store metadata such as its length. In a [circular linked list](../../data-structure.md#circular-linked-list), following successor links eventually returns to the starting point; with a [list header](../../data-structure.md#list-header), the last ordinary element links to the header, and the empty structure has the header linked to itself.

A [singly linked list](../../data-structure.md#singly-linked-list) stores a successor reference per [linked list node](../../data-structure.md#linked-list-node). A [doubly linked list](../../data-structure.md#doubly-linked-list) additionally stores a predecessor reference. The latter supports traversal in both directions and deletion of a known [linked list node](../../data-structure.md#linked-list-node) in [constant time](../../theoretical-computer-science.md#constant-time), without first searching for its predecessor. It costs another reference per [linked list node](../../data-structure.md#linked-list-node) and additional updates whose mutual consistency must be maintained. A [list header](../../data-structure.md#list-header) makes insertion and deletion at an endpoint use the same local splicing rules as an interior change; the empty case does not require replacing an external head reference.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Use an immutable index and mutable value and links:
```
class Node(var value: Double, val index: Int,
           var prev: Node = null, var next: Node = null)
```
For the [sparse linked vector representation](../../numerical-analysis.md#sparse-linked-vector-representation), a header `h` has `h.index >= 0`, records that [vector](../../vector-space.md#vector)'s dimension, and lies on a finite [circular linked list](../../data-structure.md#circular-linked-list). Every ordinary [linked list node](../../data-structure.md#linked-list-node) has an index in `[0,h.index)`, a nonzero finite value, and a unique index; indices increase strictly from `h.next` to `h.prev`. For every reachable [linked list node](../../data-structure.md#linked-list-node), including `h`, `p.next.prev eq p` and `p.prev.next eq p`. The [abstraction function](../../computer-science.md#abstraction-function) fills unspecified coordinates with zero. The header's value has no meaning. Finite real coordinates are assumed throughout; infinities and `NaN` are not ordinary [real number](../../arithmetic.md#real-number) coordinates for a mathematical [inner product](../../inner-product.md).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

**Only the [list header](../../data-structure.md#list-header) is present: `h.next eq h`, `h.prev eq h`, and `h.index` is the dimension.** This represents every coordinate as zero, including the unique zero-dimensional [vector](../../vector-space.md#vector) when the dimension is zero. The header is never treated as a nonzero coordinate.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The runtime [precondition](../../algorithm.md#precondition) check rules out negative dimensions:
```
def makeZeroVector(size: Int): Node = {
  require(size >= 0)
  val h = new Node(0.0, size)
  h.prev = h
  h.next = h
  h
}
```
Both links point to the fresh [list header](../../data-structure.md#list-header), so all reciprocal-link conditions hold and there are no ordinary entries to violate ordering or nonzero-value requirements. The [abstraction function](../../computer-science.md#abstraction-function) therefore yields **the zero [vector](../../vector-space.md#vector) of dimension `size`**. Construction uses [constant time](../../theoretical-computer-science.md#constant-time) and [constant space](../../theoretical-computer-science.md#constant-space).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Assume `vector` already satisfies the full [representation invariant](../../computer-science.md#representation-invariant) in part (b). Check the local bounds and value [preconditions](../../algorithm.md#precondition), then find the first index not smaller than the requested one:
```
def setElement(vector: Node, value: Double, index: Int): Unit = {
  require(vector != null)
  require(0 <= index && index < vector.index)
  require(value != 0.0 && !java.lang.Double.isNaN(value) &&
          !java.lang.Double.isInfinite(value))
  var p = vector.next
  while ((p ne vector) && p.index < index) p = p.next
  if ((p ne vector) && p.index == index) p.value = value
  else {
    val left = p.prev
    val fresh = new Node(value, index, left, p)
    left.next = fresh
    p.prev = fresh
  }
}
```
The search [loop invariant](../../algorithm.md#loop-invariant) says that the structure is unchanged and every ordinary [linked list node](../../data-structure.md#linked-list-node) passed has index smaller than `index`; `p` is the next candidate. The number of unpassed ordinary entries is a [loop variant](../../algorithm.md#loop-variant). The [short-circuit evaluation](../../programming-language.md#short-circuit-evaluation) prevents testing the header index as an ordinary entry. If an equal index exists, changing only its nonzero value preserves the [representation invariant](../../computer-science.md#representation-invariant). Otherwise `left` and `p` delimit the unique insertion position: initializing both new links before redirecting their neighbors preserves reciprocal links and strict index order. **Exactly the requested coordinate changes.** With $k$ stored entries, the search costs $O(k+1)$ and the splice costs [constant time](../../theoretical-computer-science.md#constant-time); checking the whole input structure is a caller obligation, rather than an unmentioned scan inside each call.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

An already-zero entry needs no new [linked list node](../../data-structure.md#linked-list-node):
```
def zeroElement(vector: Node, index: Int): Unit = {
  require(vector != null)
  require(0 <= index && index < vector.index)
  var p = vector.next
  while ((p ne vector) && p.index < index) p = p.next
  if ((p ne vector) && p.index == index) {
    val left = p.prev
    val right = p.next
    left.next = right
    right.prev = left
  }
}
```
The full input [representation invariant](../../computer-science.md#representation-invariant) is a [precondition](../../algorithm.md#precondition). The search has the same [loop invariant](../../algorithm.md#loop-invariant) and [loop variant](../../algorithm.md#loop-variant) as in part (d). At exit, either `p` is the only stored entry with that index or none exists. In the first case, bypassing it in both directions removes exactly that coordinate and preserves the order of all remaining entries. This also works when its two neighbors are the same [list header](../../data-structure.md#list-header), leaving a self-linked empty structure. The header itself is never removed. **The requested coordinate is zero and all others are unchanged**, in $O(k+1)$ [time complexity](../../theoretical-computer-science.md#time-complexity).

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Append entries in increasing index order, keeping a tail reference so that repeated searches do not make construction quadratic:
```
def makeVector(elems: Array[Double]): Node = {
  require(elems != null)
  val h = makeZeroVector(elems.length)
  var tail = h
  var i = 0
  while (i < elems.length) {
    val v = elems(i)
    require(!java.lang.Double.isNaN(v) &&
            !java.lang.Double.isInfinite(v))
    if (v != 0.0) {
      val fresh = new Node(v, i, tail, h)
      tail.next = fresh
      h.prev = fresh
      tail = fresh
    }
    i += 1
  }
  h
}
```
The [loop invariant](../../algorithm.md#loop-invariant) is $0\leq i\leq elems.length$, a valid circular representation of the nonzero entries in `elems[0..i)`, a fixed header dimension `elems.length`, and `tail eq h.prev`. The next nonzero index is greater than every stored index; appending the fresh [linked list node](../../data-structure.md#linked-list-node) preserves reciprocal links, including `tail.next eq h`. The [loop variant](../../algorithm.md#loop-variant) is `elems.length-i`. At exit **the [abstraction function](../../computer-science.md#abstraction-function) yields exactly the input [array](../../data-structure.md#array-data-structure) as a [vector](../../vector-space.md#vector)**. There is one pass and constant work per entry: $\Theta(n)$ [time complexity](../../theoretical-computer-science.md#time-complexity) for $n>0$, $O(n+1)$ including emptiness, and $O(k+1)$ output storage for $k$ nonzero entries. Both signs of floating-point zero are represented by absence.

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

Use the [sorted sparse dot product](../../numerical-analysis.md#sorted-sparse-dot-product) merge, processing a coordinate only when it appears in both [supports of a vector](../../numerical-analysis.md#support-of-a-vector):
```
def dotProduct(vec1: Node, vec2: Node): Double = {
  require(vec1 != null && vec2 != null)
  require(vec1.index == vec2.index)
  var p = vec1.next
  var q = vec2.next
  var result = 0.0
  while ((p ne vec1) && (q ne vec2)) {
    if (p.index < q.index) p = p.next
    else if (q.index < p.index) q = q.next
    else {
      result += p.value * q.value
      p = p.next
      q = q.next
    }
  }
  result
}
```
Both structures must satisfy the [representation invariant](../../computer-science.md#representation-invariant); equal dimension is checked explicitly. The [loop invariant](../../algorithm.md#loop-invariant) says that `result` contains exactly the products for all matching indices already passed, and that every skipped unequal index has zero in the other [vector](../../vector-space.md#vector). The latter follows from sortedness: if `p.index < q.index`, that index cannot appear at `q` or later, and all earlier entries of the other [vector](../../vector-space.md#vector) have already been settled. Equality contributes its product exactly once. The total number of remaining ordinary entries is a [loop variant](../../algorithm.md#loop-variant); every iteration advances at least one cursor. Once either cursor reaches its header, all remaining entries pair with zeros. Thus **the exact-arithmetic result is $\sum_i vec1_i vec2_i$**. With $k_1,k_2$ stored entries, [time complexity](../../theoretical-computer-science.md#time-complexity) is $O(k_1+k_2+1)$ and [auxiliary space](../../algorithm.md#auxiliary-space) is constant. Floating-point products and additions may round or overflow even when input coordinates are finite; no exact real-arithmetic accuracy claim is made for `Double`.

## 4

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Take the abstract state to be a finite [sequence](../../sequence-and-series.md#sequence) $s$ of [integers](../../integer.md), initially empty. Let $s_0$ denote the entry state, $\epsilon$ the empty [sequence](../../sequence-and-series.md#sequence), and $\mathbin{+\!+}$ concatenation. A [Scala](../../programming-language.md#scala) [trait](../../programming-language.md#trait) presents the interface; its comments give the mathematical [preconditions](../../algorithm.md#precondition) and [postconditions](../../algorithm.md#postcondition):
```
trait DoubleEndedQueue {
  // Pre: true. Post: result == s0.isEmpty and s == s0.
  def isEmpty: Boolean
  // Pre: true. Post: s == [x] ++ s0.
  def addLeft(x: Int): Unit
  // Pre: s0.nonEmpty. Post: result == s0.head, s == s0.tail.
  def getLeft(): Int
  // Pre: true. Post: s == s0 ++ [x].
  def addRight(x: Int): Unit
  // Pre: s0.nonEmpty. Post: result == s0.last, s == s0.init.
  def getRight(): Int
}
```
The [double-ended queue](../../data-structure.md#double-ended-queue) has no abstract capacity limit in this first specification. Both removals require nonemptiness; the query leaves the state unchanged, an instance of [command-query separation](../../programming-language.md#command-query-separation).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A fixed-size [array](../../data-structure.md#array-data-structure) cannot implement unbounded successful insertion. **Either specify a bounded [double-ended queue](../../data-structure.md#double-ended-queue) with an extra not-full insertion [precondition](../../algorithm.md#precondition), or retain the unbounded interface and specify a possible full-capacity failure.** Silently overwriting an endpoint would change the stated behavior. Here use the bounded contract, with a fixed positive capacity `MAX` and abstract state $|s|\leq MAX$. Both additions require $|s|<MAX$; the other [postconditions](../../algorithm.md#postcondition) remain unchanged. The class declaration in part (c) is interpreted as implementing this explicitly revised contract, rather than as a behavioral subtype of the unrestricted contract in part (a).

The concrete state is an [array](../../data-structure.md#array-data-structure) `a` of length `MAX`, a first-position index `head`, and an occupied-entry count `size`. Its [representation invariant](../../computer-science.md#representation-invariant) is

$$
MAX>0,\qquad a.length=MAX,\qquad 0\leq head<MAX,\qquad0\leq size\leq MAX.
$$

The [abstraction function](../../computer-science.md#abstraction-function) is $s(k)=a((head+k)\bmod MAX)$ for $0\leq k<size$. Unoccupied slots are unconstrained. Storing `size` distinguishes empty and full states even though their two circular endpoint positions coincide. `MAX=1` is valid. Using a [circular buffer](../../data-structure.md#circular-buffer) avoids shifting entries and makes every endpoint operation [constant time](../../theoretical-computer-science.md#constant-time).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The following class uses the bounded insertion contract from part (b). `slot` performs mathematical circular indexing with a wider intermediate, so even large legal indices do not overflow before reduction:
```
class ArrayDoubleEndedQueue(val MAX: Int) extends DoubleEndedQueue {
  require(MAX > 0)
  private val a = new Array[Int](MAX)
  private var head = 0
  private var size = 0

  private def slot(offset: Int): Int =
    ((head.toLong + offset.toLong) % MAX.toLong).toInt

  private def before(i: Int): Int = if (i == 0) MAX - 1 else i - 1
  private def after(i: Int): Int = if (i == MAX - 1) 0 else i + 1

  def isEmpty: Boolean = size == 0

  def addLeft(x: Int): Unit = {
    require(size < MAX)
    head = before(head)
    a(head) = x
    size += 1
  }

  def addRight(x: Int): Unit = {
    require(size < MAX)
    a(slot(size)) = x
    size += 1
  }

  def getLeft(): Int = {
    require(size > 0)
    val x = a(head)
    head = after(head)
    size -= 1
    x
  }

  def getRight(): Int = {
    require(size > 0)
    val x = a(slot(size - 1))
    size -= 1
    x
  }
}
```
For `addLeft`, moving the first position back one slot makes the old position the new logical index one; inserting at the new position prepends `x`. For `addRight`, the old `size` is the first unoccupied logical index, so writing there appends `x`. The removals read the appropriate endpoint and exclude that slot from the occupied interval. Every operation preserves the [representation invariant](../../computer-science.md#representation-invariant) and realizes the [abstraction function](../../computer-science.md#abstraction-function) postcondition. Old contents in unused slots cannot be observed through this interface. Each operation performs a fixed number of accesses and arithmetic operations, hence has [constant time](../../theoretical-computer-science.md#constant-time) and [constant space](../../theoretical-computer-science.md#constant-space) per call, apart from the class's $O(MAX)$ backing storage.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

Place this [object method](../../programming-language.md#object-method) inside the concrete class. Its [precondition](../../algorithm.md#precondition) is the [representation invariant](../../computer-science.md#representation-invariant); its [postcondition](../../algorithm.md#postcondition) is that the [abstract data type](../../computer-science.md#abstract-data-type) state is unchanged and its left-to-right contents have been printed in bracket notation followed by a newline:
```
def display: Unit = {
  print("[")
  var i = 0
  while (i < size) {
    if (i > 0) print(", ")
    print(a(slot(i)))
    i += 1
  }
  println("]")
}
```
Assume ordinary sequential execution and successful output. The [loop invariant](../../algorithm.md#loop-invariant) is $0\leq i\leq size$, unchanged representation, and output consisting of `[` followed by precisely the first $i$ abstract values, separated by commas and spaces. The [loop variant](../../algorithm.md#loop-variant) $size-i$ decreases. At exit the closing bracket completes the required display, including `[]` for emptiness. This takes $O(size+1)$ output operations and [constant space](../../theoretical-computer-science.md#constant-space).

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

The successive abstract [sequences](../../sequence-and-series.md#sequence) are $[10]$, $[20,10]$, $[20,10,30]$, $[10,30]$, $[10,30,40]$, $[10,30,40,10]$, $[10,30,40]$, $[10,30,40,15]$, and finally $[30,40,15]$. The three removals return $20$, $10$, and $10$, respectively. With the display convention in part (i), **the output is**
```
20
10
10
Queue status: [30, 40, 15]
```
The capacity-four bound is never exceeded. The abstract trace is independent of which physical [array](../../data-structure.md#array-data-structure) slots wrap around.

## 5

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Each [binary tree](../../data-structure.md#binary-tree) entry stores its word, positive frequency, and two child references:
```
class Tree(val word: String, var count: Int,
           var left: Tree = null, var right: Tree = null)
```
A `null` reference denotes an empty [subtree](../../data-structure.md#subtree). A word is a non-null [string data type](../../programming-language.md#string-data-type) value; its order below is the fixed lexicographic order used by `String.compareTo`.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The [representation invariant](../../computer-science.md#representation-invariant) says that `root` is either `null` or the root of a finite, acyclic [binary search tree](../../data-structure.md#binary-search-tree), with no [software object](../../programming-language.md#software-object) shared between different child [subtrees](../../data-structure.md#subtree). Every reachable entry has a non-null word and a strictly positive frequency. For each entry $t$, **every word in its entire left [subtree](../../data-structure.md#subtree) is strictly less than `t.word`, and every word in its entire right [subtree](../../data-structure.md#subtree) is strictly greater**. This is an inherited ordering condition on all descendants, rather than merely a comparison with immediate children. It implies that each distinct word has exactly one entry. The empty initial state satisfies it.

The [abstraction function](../../computer-science.md#abstraction-function) is the finite [multiset](../../set.md#multiset) assigning each stored word its positive count and assigning all other words zero. Frequencies and their increments must fit in `Int`; the implementation below explicitly rejects an increment at its representational limit instead of silently violating positivity through [integer overflow](../../programming-language.md#integer-overflow).

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Return the new root of the affected [subtree](../../data-structure.md#subtree), assigning that result back to the parent's child reference:
```
def addToTree(word: String, t: Tree): Tree = {
  require(word != null)
  if (t == null) new Tree(word, 1)
  else {
    val c = word.compareTo(t.word)
    if (c < 0) t.left = addToTree(word, t.left)
    else if (c > 0) t.right = addToTree(word, t.right)
    else {
      require(t.count < Int.MaxValue)
      t.count += 1
    }
    t
  }
}
// Updating the whole structure uses: root = addToTree(word, root)
```
Assume the input [binary search tree](../../data-structure.md#binary-search-tree) satisfies part (b)'s [representation invariant](../../computer-science.md#representation-invariant) and, if the key already occurs, its count can be incremented. [Structural induction](../../foundations-of-mathematics.md#structural-induction) proves the [postcondition](../../algorithm.md#postcondition). For an empty [subtree](../../data-structure.md#subtree), the fresh entry represents one occurrence. Otherwise the word comparison identifies the only possible child [subtree](../../data-structure.md#subtree) containing the word. The [recursive call](../../algorithm.md#recursive-call) adds exactly one occurrence there, preserving the inherited strict bounds; in the equal case only the count changes. The number of entries in the current [subtree](../../data-structure.md#subtree) strictly decreases in each [recursive call](../../algorithm.md#recursive-call), proving [algorithm termination](../../algorithm.md#algorithm-termination). **The returned [binary search tree](../../data-structure.md#binary-search-tree) represents the old [multiset](../../set.md#multiset) plus one occurrence of `word`.** With height $h$, at most $h+1$ comparisons are made; without balancing this can be linear in the number of words. Actual comparison work also depends on the compared [string data type](../../programming-language.md#string-data-type) lengths.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/i">i</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/i/solution">Solution</h5>

↑ **Parent:** [I](#5/d/i)

**`start == null` if and only if `end == null`.** Otherwise there is a finite list of distinct [software objects](../../programming-language.md#software-object) $v_0,\ldots,v_{m-1}$, with `start eq v0`, `end eq v(m-1)`, `v0.left == null`, and `v(m-1).right == null`. For every valid adjacent pair, `v(i).right eq v(i+1)` and `v(i+1).left eq v(i)`. These are exactly the entries reachable through the list links, so there is no extra cycle or branch. All counts are positive, all words are non-null, and words strictly increase from `start` to `end`.

This is the [representation invariant](../../computer-science.md#representation-invariant) for a null-terminated [doubly linked list](../../data-structure.md#doubly-linked-list) without a [list header](../../data-structure.md#list-header). The [abstraction function](../../computer-science.md#abstraction-function) reads the ordered word-count pairs from left to right. Conversion additionally requires the output entries, counts and words to be precisely those of the input [binary search tree](../../data-structure.md#binary-search-tree); that preservation property is an operation [postcondition](../../algorithm.md#postcondition), rather than an invariant of an arbitrary list by itself.

<h4 id="5/d/ii">ii</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/d/ii)

Perform a [destructive binary search tree flattening](../../data-structure.md#destructive-binary-search-tree-flattening) by converting both child [subtrees](../../data-structure.md#subtree) and splicing their endpoints around the original root:
```
def flatten(t: Tree): (Tree, Tree) = {
  if (t == null) (null, null)
  else {
    val oldLeft = t.left
    val oldRight = t.right
    val (ls, le) = flatten(oldLeft)
    val (rs, re) = flatten(oldRight)
    t.left = le
    if (le != null) le.right = t
    t.right = rs
    if (rs != null) rs.left = t
    val start = if (ls == null) t else ls
    val end = if (re == null) t else re
    (start, end)
  }
}
```
Save the child references before changing their interpretation. The input is a finite [binary search tree](../../data-structure.md#binary-search-tree) satisfying part (b), and no external client may simultaneously rely on the old tree links. By [structural induction](../../foundations-of-mathematics.md#structural-induction), the two [recursive calls](../../algorithm.md#recursive-call) return disjoint, ordered [doubly linked lists](../../data-structure.md#doubly-linked-list) containing exactly their original entries. The [binary search tree](../../data-structure.md#binary-search-tree) bounds place every left word before `t.word` and every right word after it. Splicing the left end, `t`, and the right start therefore preserves strict order and reciprocal links. A missing left list makes `t.left` null and `t` the start; a missing right list similarly makes `t` the end. The resulting outside links are null as required by part (i).

The recursive [loop variant](../../algorithm.md#loop-variant) analogue is the strictly smaller number of entries in each child [subtree](../../data-structure.md#subtree). Every entry is processed once and incurs a constant number of link writes, so [time complexity](../../theoretical-computer-science.md#time-complexity) is $O(n+1)$ and recursion uses $O(h+1)$ [auxiliary space](../../algorithm.md#auxiliary-space). **No new `Tree` entry is created**; returning endpoint [tuples](../../set-theory.md#finite-tuple) and using a call [stack](../../data-structure.md#stack-data-structure) are permitted auxiliary storage. The old [binary search tree](../../data-structure.md#binary-search-tree) representation is consumed by this operation.

<h4 id="5/d/iii">iii</h4>

↑ **Parent:** [D](#5/d)

<h5 id="5/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/d/iii)

Replace suspended [recursive calls](../../algorithm.md#recursive-call) by an explicit [stack](../../data-structure.md#stack-data-structure) for an [inorder traversal](../../data-structure.md#inorder-traversal). Save each original right child before overwriting that link:
```
def flattenIterative(): (Tree, Tree) = {
  val pending = new scala.collection.mutable.Stack[Tree]
  var current = root
  var start: Tree = null
  var end: Tree = null
  while (current != null || pending.nonEmpty) {
    while (current != null) {
      pending.push(current)
      current = current.left
    }
    val t = pending.pop()
    val nextSubtree = t.right
    t.left = end
    if (end == null) start = t else end.right = t
    t.right = null
    end = t
    current = nextSubtree
  }
  root = null
  (start, end)
}
```
The method belongs to the concrete class owning `root`. Clearing `root` records that ownership has transferred to the returned [doubly linked list](../../data-structure.md#doubly-linked-list); callers retain both returned endpoints. The inner [loop invariant](../../algorithm.md#loop-invariant) says that the current [subtree](../../data-structure.md#subtree) lies before all its pending ancestors in [inorder traversal](../../data-structure.md#inorder-traversal); pushing and descending left preserves this fact. Its [loop variant](../../algorithm.md#loop-variant) is the number of entries along the remaining left-child path, a finite decreasing quantity.

The outer [loop invariant](../../algorithm.md#loop-invariant) says that `start` through `end` is precisely the already emitted sorted prefix, with reciprocal links and null outside endpoints. `current` and the pending ancestors describe exactly the remaining traversal in order; original links that are still needed have been retained. A pending ancestor has not yet had its right child overwritten. The next popped entry is therefore the next sorted entry. Saving `nextSubtree` preserves its future work before assigning `t.right = null`; linking it to `end` extends the prefix by exactly one entry. The number of original entries not yet emitted is an outer [loop variant](../../algorithm.md#loop-variant), since each full outer iteration emits one. At exit nothing remains, proving the same preservation and ordering [postconditions](../../algorithm.md#postcondition) as the recursive version.

Each entry is pushed and popped once, giving $O(n+1)$ [time complexity](../../theoretical-computer-science.md#time-complexity) and $O(h+1)$ [auxiliary space](../../algorithm.md#auxiliary-space). No new `Tree` entries are allocated. The historical mutable [stack](../../data-structure.md#stack-data-structure) interface provides the `push` and `pop` operations used here; its later deprecation does not change their meaning.[Scala 2.12.6, constructors, push(elem), pop(), nonEmpty](../../computer-science-bibliography.md#scala-2-12-mutable-stack-api-documentation)

## 6

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Use an inverse edit record with a common undo/redo interface. Positions are zero-based. For `move(i,j)`, **`j` is the song's final index after the move**, so it is also the insertion index in the shortened [sequence](../../sequence-and-series.md#sequence). For an original length $m$, require $0\leq i,j<m$; insertion permits $0\leq i\leq m$ and deletion requires $0\leq i<m$. As allowed, the caller guarantees validity.
```
trait Change {
  def undo(): Unit
  def redo(): Unit
}

class SongSuite(initial: Sequence[Song]) {
  private var songs = initial
  def length: Int = songs.length
  def elementAt(i: Int): Song = songs.elementAt(i)

  private def rawInsert(i: Int, x: Song): Unit = {
    songs = songs.insert(i, x)
  }
  private def rawDelete(i: Int): Unit = {
    songs = songs.delete(i)
  }
  private def rawMove(i: Int, j: Int): Unit = {
    val x = songs.elementAt(i)
    songs = songs.delete(i)
    songs = songs.insert(j, x)
  }
  private def perform(forward: () => Unit,
                      backward: () => Unit): Change = {
    forward()
    new Change {
      def undo(): Unit = backward()
      def redo(): Unit = forward()
    }
  }
  def insert(i: Int, x: Song): Change =
    perform(() => rawInsert(i, x), () => rawDelete(i))

  def delete(i: Int): Change = {
    val x = songs.elementAt(i)
    perform(() => rawDelete(i), () => rawInsert(i, x))
  }
  def move(i: Int, j: Int): Change =
    perform(() => rawMove(i, j), () => rawMove(j, i))
}
```
`Song` denotes the application's song type, whose internal fields are irrelevant to these operations. `Sequence` denotes the supplied interface; each returned [sequence](../../sequence-and-series.md#sequence) is assigned back, so the code does not discard the result of a functional implementation. `SongSuite` owns its current [sequence](../../sequence-and-series.md#sequence); independent mutations through outside aliases are excluded. Atomic successful edits and an ordinary sequential history are assumed.

For [inverse command correctness](../../programming-language.md#inverse-command-correctness), inserting at $i$ is reversed by deleting at $i$; deleting at $i$ is reversed by reinserting the saved song there. After moving from $i$ to $j$, removing the moved song at $j$ recovers the original [sequence](../../sequence-and-series.md#sequence) with that one entry missing, and reinserting it at $i$ restores the original. This also covers $i=j$. Store the actual deleted song reference, rather than identifying it by title, since duplicate songs may occur.

The edits have already executed when returned. A history manager can enforce the chronological protocol with two [stacks](../../data-structure.md#stack-data-structure):
```
class History {
  private var done: List[Change] = Nil
  private var undone: List[Change] = Nil
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
For example, `history.record(suite.move(i,j))` records an applied move. The history [invariant](../../mathematics.md#invariant-mathematics) says that the current playlist results from the applied prefix, the top of `done` is its last edit, and the top of `undone` is the first next edit available for redo. Each transfer preserves this [invariant](../../mathematics.md#invariant-mathematics). A fresh edit clears the redo branch. Calling an arbitrary old inverse after unrelated edits is outside this protocol and need not be correct.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The [Command pattern](../../programming-language.md#command-pattern) separates a request into a common command interface, concrete commands carrying arguments and execution behavior, a receiver doing the application work, an invoker requesting execution or retaining history, and a client assembling these [software objects](../../programming-language.md#software-object). A menu item, toolbar button or keyboard shortcut can invoke the same command without duplicating the playlist manipulation.

**`SongSuite` is the receiver.** The application/controller invokes its operations, and the returned `Change` [software objects](../../programming-language.md#software-object) hold the concrete inverse/forward behavior. A command wrapper can expose an initial `execute` that calls the appropriate `SongSuite` operation and then delegates later undo/redo to its returned record. `History` is the history-managing part of the invoker. Separating these roles avoids making a graphical control know how the playlist representation is edited; requests can be retained and reversed through a common [object interface](../../programming-language.md#object-interface).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/i">i</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/i/solution">Solution</h5>

↑ **Parent:** [I](#6/c/i)

If [sequence](../../sequence-and-series.md#sequence) versions are immutable, replace `perform` by the following method; the insert, delete and move entry points can stay as written:
```
private def perform(forward: () => Unit,
                    backward: () => Unit): Change = {
  val before = songs
  forward()
  val after = songs
  new Change {
    def undo(): Unit = { songs = before }
    def redo(): Unit = { songs = after }
  }
}
```
The unused inverse argument can subsequently be removed from `perform` and its callers. Each history record now captures two complete versions. Undo and redo restore the respective roots without replaying an operation, an instance of the [Memento pattern](../../programming-language.md#memento-pattern). The same chronological history discipline still applies.

**The supplied method signatures alone do not establish immutability or persistence.** If `insert` or `delete` changes a shared mutable [software object](../../programming-language.md#software-object), merely storing its reference fails to freeze the earlier state. Then independent copies of the relevant state are needed, including any mutable song state intended to be undoable, or the implementation must provide immutable [persistent data structure](../../data-structure.md#persistent-data-structure) versions. This is a representation requirement, not a reason to invent a particular unavailable copying API.

<h4 id="6/c/ii">ii</h4>

↑ **Parent:** [C](#6/c)

<h5 id="6/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/c/ii)

Version snapshots simplify correctness: a complicated command restores the complete prior state, so a bespoke inverse cannot accidentally omit an auxiliary field. Redo restores the recorded result without re-executing behavior that might depend on time, randomness or external input. Restoring an immutable root takes [constant time](../../theoretical-computer-science.md#constant-time), though refreshing the display can cost more.

The storage comparison depends on the representation. A change-specific record for these elementary edits retains only a few indices and song references. Copying a length-$m$ [array](../../data-structure.md#array-data-structure) for each of $h$ edits can require $\Theta(hm)$ storage and $\Theta(m)$ copying per edit. A [persistent data structure](../../data-structure.md#persistent-data-structure) with [structural sharing](../../data-structure.md#structural-sharing) can preserve many versions much more cheaply; balanced path copying can make small edits allocate $O(\log m)$ new entries. Retaining versions also keeps their reachable data alive. Snapshot references are only constant-sized roots, not a guarantee of constant total retained memory. Neither scheme automatically reverses external effects such as playing audio or writing files. The desired undo boundary must be specified.

## 7

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

[Programming language polymorphism](../../programming-language.md#programming-language-polymorphism) means that one interface or program definition can be used with values of multiple types. In [object-oriented programming](../../programming-language.md#object-oriented-programming), [subtype polymorphism](../../programming-language.md#subtype-polymorphism) allows references with a common [static type](../../programming-language.md#static-type) to denote instances of different concrete subclasses or implementers of a [trait](../../programming-language.md#trait). An [object method](../../programming-language.md#object-method) call uses [dynamic dispatch](../../programming-language.md#dynamic-dispatch) to select the overriding implementation belonging to the receiver's [runtime type](../../programming-language.md#runtime-type). For example, different implementations of a playlist interface can respond to the same `insert` call without the client testing their concrete classes.

[Parametric polymorphism](../../programming-language.md#parametric-polymorphism) uses [type parameters](../../programming-language.md#type-parameter), as in `Sequence[A]`, so the same definition works uniformly for songs, [integers](../../integer.md), or other elements. [Ad hoc polymorphism](../../programming-language.md#ad-hoc-polymorphism) includes [method overloading](../../programming-language.md#method-overloading), where different parameter signatures share a name and the [static types](../../programming-language.md#static-type) determine overload selection. These mechanisms are distinct: selecting an overloaded signature is not the same step as dispatching an override of that selected signature. [Class inheritance](../../programming-language.md#class-inheritance) can supply implementations, but the reusable interface and legal [subtyping](../../programming-language.md#subtyping) relationship determine what a polymorphic client may do.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Use [pattern matching](../../programming-language.md#pattern-matching) and an [optional value](../../data-structure.md#optional-value) to distinguish absence from a present result:
```
class PartialFn[T, U](val data: List[(T, U)]) {
  def get(x: T): Option[U] =
    data.find { case (key, _) => key == x }.map(_._2)

  def remove(x: T): PartialFn[T, U] =
    new PartialFn[T, U](data.filterNot { case (key, _) => key == x })

  def add(x: T, y: U): PartialFn[T, U] =
    new PartialFn[T, U]((x, y) ::
      data.filterNot { case (key, _) => key == x })
}
```
The representation [precondition](../../algorithm.md#precondition) is that equal keys always have equal associated values, with a stable equality relation on keys. This permits harmless repeated identical pairs; it excludes conflicting outputs for one input. `get` therefore returns `Some(y)` exactly when the represented [partial function](../../function.md#partial-function) is defined at `x`. Removing filters out every occurrence of the key and leaves all other pairs unchanged. Adding first removes every old occurrence and prepends exactly the new pair, proving the [partial function](../../function.md#partial-function) update [postcondition](../../algorithm.md#postcondition) even if the input contains duplicate identical pairs. The immutable [linked list](../../data-structure.md#linked-list) representation leaves the original mapping unchanged. Each operation has $O(m+1)$ worst-case [time complexity](../../theoretical-computer-science.md#time-complexity) for $m$ pairs under constant-cost key equality.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

The second [partial function](../../function.md#partial-function) accepts this one's outputs. Put this method inside the invariant class in part (b):
```
def compose[V](that: PartialFn[U, V]): PartialFn[T, V] = {
  val pairs: List[(T, V)] = data.flatMap {
    case (x, y) => that.get(y).map(z => (x, z)).toList
  }
  new PartialFn[T, V](pairs)
}
```
**The represented mapping is $that\circ this$**, since the paper explicitly applies `that` second despite the method name. A pair is emitted exactly when this mapping supplies a `y` and `that.get(y)` supplies a `z`. Hence its [domain of a partial function](../../function.md#domain-of-a-partial-function) is $\{x\in\operatorname{dom}(this):this(x)\in\operatorname{dom}(that)\}$ and its value there is $that(this(x))$. This is strict [composition of partial functions](../../function.md#composition-of-partial-functions): either missing stage makes the composite undefined. Repeated equal input pairs still produce the same output, preserving the representation [invariant](../../mathematics.md#invariant-mathematics). With $m$ and $k$ pairs, direct association-list lookup gives $O(m(k+1)+1)$ worst-case [time complexity](../../theoretical-computer-science.md#time-complexity), not a hidden constant-cost dictionary lookup.

<h3 id="7/d">d</h3>

↑ **Parent:** [7](#7)

<h4 id="7/d/solution">Solution</h4>

↑ **Parent:** [D](#7/d)

A [covariant type parameter](../../programming-language.md#covariant-type-parameter) preserves [subtyping](../../programming-language.md#subtyping): **if $A<:B$, then `PartialFn[T,A] <: PartialFn[T,B]`** when its second parameter is covariant. In [Scala](../../programming-language.md#scala) the class annotation is `+U`. A mapping that produces a narrower output can be used where a broader output is expected. Covariance describes a type relationship; it does not convert stored values or make mutation through a widened reference safe.[Relations between types: conformance of parameterized types and variance](../../computer-science-bibliography.md#scala-2-12-types-specification)

<h3 id="7/e">e</h3>

↑ **Parent:** [7](#7)

<h4 id="7/e/solution">Solution</h4>

↑ **Parent:** [E](#7/e)

Declare `+U`, keep its stored [linked list](../../data-structure.md#linked-list) immutable, and generalize operations that need to accept output values by a fresh [lower type bound](../../programming-language.md#lower-type-bound):
```
class PartialFn[T, +U](val data: List[(T, U)]) {
  def get(x: T): Option[U] =
    data.find { case (key, _) => key == x }.map(_._2)

  def remove(x: T): PartialFn[T, U] =
    new PartialFn[T, U](data.filterNot { case (key, _) => key == x })

  def add[V >: U](x: T, y: V): PartialFn[T, V] =
    new PartialFn[T, V]((x, y) ::
      data.filterNot { case (key, _) => key == x })

  def compose[V >: U, W](that: PartialFn[V, W]): PartialFn[T, W] = {
    val pairs: List[(T, W)] = data.flatMap {
      case (x, y) => that.get(y).map(z => (x, z)).toList
    }
    new PartialFn[T, W](pairs)
  }
}
```
`get`, `remove`, and the immutable `val data` expose `U` in covariant result positions: [Scala](../../programming-language.md#scala)'s immutable `List`, `Tuple2` and `Option` preserve that position. The old `add(x:T,y:U)` consumed `U` directly, violating the [variance-position rule](../../programming-language.md#variance-position-rule). The new `add` accepts a value of a chosen supertype `V` and returns a new mapping with that widened output type; it never inserts the wider value into the old narrower mapping.

The original `compose` also mentions `U` as the first, invariant parameter of `PartialFn[U,V]`. Changing only `add` is therefore insufficient. Its new first [type parameter](../../programming-language.md#type-parameter) `V >: U` is independent of the class's covariant parameter except for the allowed lower bound. Any stored `y:U` is acceptable to `that.get` as a `V`, while the result has output type `W`. This [lower type bound](../../programming-language.md#lower-type-bound) solution avoids unchecked variance annotations or casts. The official variance rules illustrate the same lower-bound widening technique for an immutable collection's consuming method; the later 2.13 text corroborates the rule, without identifying an installed 2018 compiler version.[Variance Annotations: method-parameter positions, invariant type arguments, and the lower-bound widening example for Sequence.append](../../computer-science-bibliography.md#scala-2-13-variance-annotations-specification)

## 8

↑ **Parent:** [Imperative programming](imperative-programming.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/solution">Solution</h4>

↑ **Parent:** [A](#8/a)

In the [Observer pattern](../../programming-language.md#observer-pattern), an observable subject maintains subscriptions and sends notifications through a common observer interface when a relevant change occurs. Observers can then react to the event or query the subject's coherent new state. Registration and removal allow multiple dependants to change independently of the subject's application logic.

It is useful when one [software object](../../programming-language.md#software-object) has several changing dependants, for example a document model with several views or a text field with an event handler. **It avoids hard-coding every concrete dependant into the subject**, reducing direct coupling and duplicated synchronization logic. Clients need not poll repeatedly to detect a change. This separation does not automatically prevent notification cycles, stale subscriptions, or inconsistent intermediate states: notification should occur after a coherent update, and observers should unregister when no longer needed. A [reentrant event handler](../../programming-language.md#reentrant-event-handler) can otherwise commit recursively while refreshing a display.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/solution">Solution</h4>

↑ **Parent:** [B](#8/b)

A [Scala Swing](../../programming-language.md#scala-swing) `Publisher` is the subject-side event source. Calling `publish(e)` notifies its subscribed reactors. A `Reactor` is the observer-side participant: `listenTo(p1,p2)` registers it with the specified sources, `deafTo` ends those subscriptions, and `reactions` contains the event-handling cases.
```
listenTo(pounds, euros, rate)
reactions += {
  case EditDone(source) => handleCommittedEdit(source)
}
```
Here the containing frame supplies the reactor behavior, and each text field supplies publication. Defining `reactions` without `listenTo` is insufficient to establish the subscription. The pattern-matching cases can handle only events of interest while other events are ignored. This is the [Observer pattern](../../programming-language.md#observer-pattern) expressed through event publication rather than a separate hand-written `update` method for every subject.[Archived Reactor API: listenTo, deafTo and reactions; official library README: Publisher/Reactor event-system overview](../../computer-science-bibliography.md#scala-swing-event-system-documentation)

<h3 id="8/c">c</h3>

↑ **Parent:** [8](#8)

<h4 id="8/c/solution">Solution</h4>

↑ **Parent:** [C](#8/c)

Choose a deterministic editing policy: editing pounds or the exchange rate preserves the pounds amount and recalculates euros; editing euros preserves the rate and recalculates pounds. A valid rate must be finite and positive; amounts may be any finite signed number. Keep an unrounded numeric model, so repeatedly refreshing a two-decimal display does not feed rounded text back into the computation. Place the following members inside the supplied `MainFrame`, after its fields are created:
```
private var poundsValue = 10.0
private var eurosValue = 11.5
private var rateValue = 1.15
private var refreshing = false

private def finite(x: Double): Boolean =
  !java.lang.Double.isNaN(x) && !java.lang.Double.isInfinite(x)

private def number(s: String): Option[Double] =
  scala.util.Try(s.trim.toDouble).toOption.filter(finite)

private def money(x: Double): String =
  java.lang.String.format(java.util.Locale.ROOT, "%.2f",
                          java.lang.Double.valueOf(x))

private def refresh(): Unit = {
  refreshing = true
  try {
    pounds.text = money(poundsValue)
    euros.text = money(eurosValue)
    rate.text = money(rateValue)
  } finally {
    refreshing = false
  }
}

private def commit(p: Double, e: Double, r: Double): Unit = {
  if (finite(p) && finite(e) && finite(r) && r > 0.0) {
    poundsValue = p
    eurosValue = e
    rateValue = r
    refresh()
  }
}

listenTo(pounds, euros, rate)
reactions += {
  case EditDone(source) if !refreshing =>
    number(source.text).foreach { value =>
      if (source eq pounds)
        commit(value, value * rateValue, rateValue)
      else if (source eq euros)
        commit(value / rateValue, value, rateValue)
      else if ((source eq rate) && value > 0.0)
        commit(poundsValue, poundsValue * value, value)
    }
}
```
The mathematical model [invariant](../../mathematics.md#invariant-mathematics) is $eurosValue=poundsValue\,rateValue$ with a positive rate. In [floating-point arithmetic](../../floating-point-arithmetic.md), each update establishes the corresponding rounded multiplication or division; a division followed by multiplication need not recover bitwise identical values. Pounds and rate edits calculate a matching euro amount, while euro edits calculate its matching pound amount. An invalid parse, a nonpositive rate, or a nonfinite calculated result leaves the last valid numeric model unchanged. An invalid text entry may remain visible until corrected or a subsequent valid refresh; a production interface could add a validation message.

Every accepted edit refreshes the fields from that model. `Locale.ROOT` makes the decimal separator match the `toDouble` parser, independently of the machine's locale. The guard prevents a synchronous [reentrant event handler](../../programming-language.md#reentrant-event-handler) from interpreting a refresh as another user commit. The displayed values are rounded to two decimal places, including the rate, while the stored values retain full `Double` precision. Very small positive rates can therefore display as `0.00`; using more rate digits is a reasonable presentation refinement. **Pounds, euros and rate edits all propagate by the stated policy**, with no parsing exception or division by zero.

`EditDone` handles completion of an edit, such as an action or focus-change notification, using the event type supplied in the paper. It is not a promise of recalculation after every keystroke. A character-by-character interface would subscribe to the corresponding text-change event instead. The publisher/reactor interaction follows the supplied contract and official [Scala Swing](../../programming-language.md#scala-swing) documentation; no exact course library build or native graphical execution is presumed.[Publisher/Reactor subscriptions and reactions; the paper supplies the EditDone event contract](../../computer-science-bibliography.md#scala-swing-event-system-documentation)

<h3 id="8/d">d</h3>

↑ **Parent:** [8](#8)

<h4 id="8/d/solution">Solution</h4>

↑ **Parent:** [D](#8/d)

[Model-view-controller](../../computer-science.md#model-view-controller) divides an interactive application into a model containing application state and domain rules, a view rendering that state, and a controller interpreting user actions and requesting model operations. In the converter, the numeric amounts and exchange relation belong to the model, the text fields and labels form the view, and the edit handler parses input and chooses which quantity to preserve. A playlist model similarly owns song order independently of the controls used to change it.

A user acts through the view, the controller interprets that input, the model validates and commits a change, and the view then renders the resulting state. The exact packaging varies: a widget can combine view and controller responsibilities while still separating domain logic. Keeping the model independent of particular controls supports [separation of concerns](../../computer-science.md#separation-of-concerns), [encapsulation](../../computer-science.md#encapsulation-computer-programming), reuse of the same model in several views, and [unit testing](../../computer-science.md#unit-testing) of domain behavior without a graphical interface.

The [Observer pattern](../../programming-language.md#observer-pattern) often supplies the model-to-view notification path: views subscribe to model changes, so the model need not directly know every concrete view. It can also carry view input events to a controller, as in [Scala Swing](../../programming-language.md#scala-swing). **[Model-view-controller](../../computer-science.md#model-view-controller) is an architectural separation of responsibilities; the [Observer pattern](../../programming-language.md#observer-pattern) is one mechanism for their communication.** They are related without being identical, and small applications can implement the separation with direct calls where event subscriptions add no benefit.

## ↑ Ancestors (9)

1. [2018](../2018.md)
2. [Past exam of the year 1 of the computer science course of the University of Oxford](../../past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
3. [Year 1 of the computer science course of the University of Oxford](../../university-of-oxford.md#year-1-of-the-computer-science-course-of-the-university-of-oxford)
4. [Computer science course of the University of Oxford](../../university-of-oxford.md#computer-science-course-of-the-university-of-oxford)
5. [Undergraduate course of the University of Oxford](../../university-of-oxford.md#undergraduate-course-of-the-university-of-oxford)
6. [Course of the University of Oxford](../../university-of-oxford.md#course-of-the-university-of-oxford)
7. [University of Oxford](../../university-of-oxford.md)
8. [List of universities](../../README.md#list-of-universities)
9. [Codex Wiki](../../README.md)
