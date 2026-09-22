# Paper 5

↑ **Parent:** [Ia](../ia.md)

[https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2006/PaperIA_5.pdf](https://www.maths.cam.ac.uk/undergrad/pastpapers/files/2006/PaperIA_5.pdf)

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
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
    - [iii](#5/a/iii)
      - [Solution](#5/a/iii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [a](#7/a)
    - [i](#7/a/i)
      - [Solution](#7/a/i/solution)
    - [ii](#7/a/ii)
      - [Solution](#7/a/ii/solution)
    - [iii](#7/a/iii)
      - [Solution](#7/a/iii/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)
  - [c](#7/c)
    - [Solution](#7/c/solution)
- [8](#8)
  - [a](#8/a)
    - [i](#8/a/i)
      - [Solution](#8/a/i/solution)
    - [ii](#8/a/ii)
      - [Solution](#8/a/ii/solution)
    - [iii](#8/a/iii)
      - [Solution](#8/a/iii/solution)
    - [iv](#8/a/iv)
      - [Solution](#8/a/iv/solution)
  - [b](#8/b)
    - [i](#8/b/i)
      - [Solution](#8/b/i/solution)
    - [ii](#8/b/ii)
      - [Solution](#8/b/ii/solution)
- [9](#9)
  - [a](#9/a)
    - [Solution](#9/a/solution)
  - [b](#9/b)
    - [Solution](#9/b/solution)
  - [c](#9/c)
    - [Solution](#9/c/solution)
  - [d](#9/d)
    - [Solution](#9/d/solution)
  - [e](#9/e)
    - [Solution](#9/e/solution)
- [10](#10)
  - [a](#10/a)
    - [Solution](#10/a/solution)
  - [b](#10/b)
    - [Solution](#10/b/solution)
  - [c](#10/c)
    - [Solution](#10/c/solution)
  - [d](#10/d)
    - [Solution](#10/d/solution)
  - [e](#10/e)
    - [Solution](#10/e/solution)
- [11](#11)
  - [Solution](#11/solution)
  - [i](#11/i)
    - [Solution](#11/i/solution)
  - [ii](#11/ii)
    - [Solution](#11/ii/solution)
  - [iii](#11/iii)
    - [Solution](#11/iii/solution)
  - [iv](#11/iv)
    - [Solution](#11/iv/solution)
- [12](#12)
  - [Solution](#12/solution)

## 1

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the usual unit-cost model for [Standard ML](../../../computer-science.md#standard-ml) list constructors and fixed-size arithmetic. The input size $n$ in the list examples is the number of list elements, rather than the size of the integer entries. Inspecting only the first constructor has constant [time complexity](../../../computer-science.md#time-complexity):
```
sml
fun firstOrZero [] = 0
  | firstOrZero (x :: _) = x;
```
No tail is traversed. **The running time is $\Theta(1)$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [Standard ML](../../../computer-science.md#standard-ml) length function visits each list constructor once:
```
sml
fun length [] = 0
  | length (_ :: xs) = 1 + length xs;
```
Writing $T(n)$ for its [time complexity](../../../computer-science.md#time-complexity), $T(n)=T(n-1)+\Theta(1)$ and $T(0)=\Theta(1)$. Thus **$T(n)=\Theta(n)$**. Arithmetic is treated as unit cost; the example concerns list traversal rather than arbitrary-precision arithmetic.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use [merge sort](../../../computer-science.md#merge-sort) on a list of integers:
```
sml
fun sort xs = mergeSort (op <=) xs;
```
Here `mergeSort` denotes the standard [merge sort](../../../computer-science.md#merge-sort) implementation: split into two almost equal lists, recursively sort them, and combine them using the [merge algorithm](../../../computer-science.md#merge-algorithm). Splitting and merging take linear time, and each recursion level has total input length $n$. There are $\Theta(\log n)$ levels, so the worst-case [time complexity](../../../computer-science.md#time-complexity) is **$\Theta(n\log n)$**. Equivalently, $T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+\Theta(n)$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Traverse the whole original list once for each of its elements:
```
sml
fun scan [] = ()
  | scan (_ :: xs) = scan xs;

fun scanForEach [] whole = ()
  | scanForEach (_ :: rest) whole =
      (scan whole; scanForEach rest whole);

fun quadratic xs = scanForEach xs xs;
```
The outer [structural recursion](../../../computer-science.md#structural-recursion) runs $n$ times, and each `scan whole` visits $n$ constructors. In the ordinary source-evaluation cost model, **the [time complexity](../../../computer-science.md#time-complexity) is $\Theta(n^2)$**. This example counts executed traversals, without assuming an optimizing compiler that removes deliberately unused computations.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

For a nonnegative integer parameter $n$, make both branches of a [structural recursion](../../../computer-science.md#structural-recursion) execute:
```
sml
fun binaryWalk 0 = ()
  | binaryWalk n = (binaryWalk (n - 1); binaryWalk (n - 1));
```
The semicolon sequences two calls, so this is not a conditional choosing just one branch. The recursion tree has $2^n$ leaves and $2^{n+1}-1$ calls. Its [time complexity](../../../computer-science.md#time-complexity) satisfies $T(n)=2T(n-1)+\Theta(1)$, giving **$\Theta(2^n)$**. Here $n$ is the parameter specified by the question, not its binary encoding length; only $\Theta(n)$ calls are simultaneously on the stack.

## 2

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

**False.** The [Windows XP](../../../computer-science.md#windows-xp) Executive implements core object management, memory management, process management and input-output services in privileged mode, as part of the kernel image. User applications and environment subsystems invoke these services through controlled entry points; they do not turn the Executive into user-mode code. This distinction is explicit in Microsoft's [description of the Executive layer](https://learn.microsoft.com/en-us/windows-hardware/drivers/kernel/windows-kernel-mode-executive-support-library).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

**False.** An [access matrix](../../../computer-science.md#access-matrix) is an authorization table, not a numerical matrix representing a linear transformation. Its entries are sets of rights, such as permission to read or write an object. “Inverting” its organization means obtaining subject-oriented capability lists from object-oriented [access control lists](../../../computer-science.md#access-control-list), or conversely, by enumerating and regrouping entries. Numerical floating-point matrix inversion has neither the relevant operations nor the relevant semantics, and many access tables are not even square.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

**True.** In [polled input-output](../../../computer-science.md#polled-input-output), a processor reads device status and handles ready work without [interrupt](../../../computer-science.md#interrupt) entry and return overhead. If an operation completes very quickly, or requests arrive continuously at a high rate, a short poll or a batch of polls can cost less than an [interrupt](../../../computer-science.md#interrupt) for every event. [Interrupt-driven input-output](../../../computer-science.md#interrupt-driven-input-output) is usually better for long or infrequent waits because the processor can do unrelated work or sleep instead of busy waiting. The useful choice depends on the event rate and latency requirement.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

**False as a general performance claim.** A [microkernel](../../../computer-science.md#microkernel) moves services into separate protection domains, which can require extra messages, scheduling and address-space transitions. A [monolithic kernel](../../../computer-science.md#monolithic-kernel) can often call a service directly within its own privileged address space. The [microkernel](../../../computer-science.md#microkernel) gains isolation and modularity, but these do not imply greater speed. Efficient implementations and particular workloads can change the comparison; the architecture alone gives no universal ordering.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

**True in the intended comparison with traditional Unix protection mechanisms.** [Windows XP](../../../computer-science.md#windows-xp) provides object-specific [access control lists](../../../computer-science.md#access-control-list), subject tokens containing identities and privileges, and a security reference monitor. Rights can distinguish operations on files, registry keys, processes and other protected objects. Traditional [Unix](../../../computer-science.md#unix) file permissions distinguish read, write and execute for owner, group and everyone else; unrestricted root authority also makes privilege separation coarse. The richer [Windows XP](../../../computer-science.md#windows-xp) mechanisms can express finer least-privilege policies. Cambridge's [access-control notes](https://www.cl.cam.ac.uk/teaching/0809/IntroSec/slides-2up.pdf) describe this architectural contrast.

This is an architectural capability comparison, not a claim that every [Windows XP](../../../computer-science.md#windows-xp) installation resists attacks better than every [Unix](../../../computer-science.md#unix) installation. More complex authorization is not itself a proof of security; configuration and implementation matter, and [Unix](../../../computer-science.md#unix) variants can add [access control lists](../../../computer-science.md#access-control-list) and other protection mechanisms. Without specifying that traditional model, the blanket comparison is underspecified.

## 3

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Extract one four-bit digit at a time, beginning at the most significant end of the [Java](../../../computer-science.md#java-programming-language) `int`. A lookup string supplies characters, but no library performs the conversion:
```
java
static String toHex(int value) {
    String digits = "0123456789abcdef";
    String answer = "";
    boolean started = false;
    for (int shift = 28; shift >= 0; shift -= 4) {
        int digit = (value >>> shift) & 15;
        if (started || digit != 0 || shift == 0) {
            answer = answer + digits.charAt(digit);
            started = true;
        }
    }
    return answer;
}
```
The logical right [bit shift](../../../computer-science.md#bit-shift) `>>>` inserts zeros, and the [bit mask](../../../computer-science.md#bit-mask) `15` retains exactly the low four bits of the shifted word. Each emitted character is therefore the corresponding [hexadecimal](../../../computer-science.md#hexadecimal) digit. The `started` flag suppresses leading zero digits; the `shift == 0` exception makes zero produce **`"0"`**, rather than an empty string.

A negative [Java](../../../computer-science.md#java-programming-language) integer uses [two's complement](../../../computer-science.md#two-s-complement). Its top bit is set, so the first extracted digit is between eight and fifteen and all eight digits are emitted. We interpret its original 32-bit pattern, without taking an absolute value or negating a potentially unnegatable minimum integer. In particular, **`toHex(19)` returns `"13"`, `toHex(-1)` returns `"ffffffff"`, and `toHex(Integer.MIN_VALUE)` returns `"80000000"`.** There are exactly eight iterations, so for this fixed word size the [time complexity](../../../computer-science.md#time-complexity) is constant.

## 4

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

A [prime number](../../../number-theory.md#prime-number) is an integer greater than one whose only positive divisors are one and itself. In particular, one is not a [prime number](../../../number-theory.md#prime-number). Every integer greater than one has a [prime number](../../../number-theory.md#prime-number) divisor, by taking its smallest divisor greater than one.

Suppose there were only finitely many [prime numbers](../../../number-theory.md#prime-number) congruent to $-1$ modulo six, and let their product be $P$, with empty product one. The integer $N=6P-1>1$ has no divisor two or three and is divisible by none of the listed [prime numbers](../../../number-theory.md#prime-number), since $N\equiv-1\pmod{p_j}$. Every [prime number](../../../number-theory.md#prime-number) divisor of $N$ is therefore $1$ or $-1$ modulo six. If all these divisors were $1$ modulo six, their product, with multiplicities, would also be $1$ modulo six. But $N\equiv-1\pmod6$. Hence at least one divisor is an unlisted [prime number](../../../number-theory.md#prime-number) congruent to $-1$ modulo six, a contradiction. **There are infinitely many primes of the form $6k-1$.**

For the other class, suppose its [prime numbers](../../../number-theory.md#prime-number) were a finite list with product $P$. None is divisible by three. The integer $M=4P^2+3$ is odd and is $1$ modulo three, since $P^2\equiv1\pmod3$. Thus a [prime number](../../../number-theory.md#prime-number) divisor $q$ of $M$ satisfies $q>3$. The residue $x=2P$ solves $x^2\equiv-3\pmod q$, so the allowed quadratic-congruence fact gives $q\equiv1\pmod6$. However, for every listed divisor $p_j$, $M\equiv3\pmod{p_j}$, and $p_j>3$, so none divides $M$. We have again found an unlisted [prime number](../../../number-theory.md#prime-number) in the supposedly complete list. **There are infinitely many primes of the form $6k+1$.** Both arguments remain valid for an empty starting list.

## 5

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

A [FIFO queue](../../../computer-science.md#fifo-queue) provides an empty queue, an emptiness test, insertion at the rear, inspection of the front item, and removal of the front item. It preserves insertion order: after enqueuing $x$ and then $y$, removing an item returns $x$ first. Inspection and removal on an empty [FIFO queue](../../../computer-science.md#fifo-queue) must have a specified outcome, such as an [exception handling](../../../computer-science.md#exception-handling) case or an option-valued result. In a functional interface, insertion and removal return the new [FIFO queue](../../../computer-science.md#fifo-queue) rather than updating their argument.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

Use a [two-list functional queue](../../../computer-science.md#two-list-functional-queue). Its representation `(front, rear)` denotes the abstract sequence `front @ rev rear`; the front is nonempty unless the whole [FIFO queue](../../../computer-science.md#fifo-queue) is empty. Normalize only when the front runs out:
```
sml
datatype 'a queue = Q of 'a list * 'a list;
exception EmptyQueue;

fun check ([], rear) = Q (rev rear, [])
  | check (front, rear) = Q (front, rear);

fun empty () = Q ([], []);
fun isEmpty (Q (front, _)) = null front;
fun enqueue x (Q (front, rear)) = check (front, x :: rear);

fun peek (Q ([], _)) = raise EmptyQueue
  | peek (Q (x :: _, _)) = x;

fun dequeue (Q ([], _)) = raise EmptyQueue
  | dequeue (Q (x :: front, rear)) = (x, check (front, rear));
```
Enqueue prepends to the reversed rear list. Removing the head either leaves a nonempty front or reverses the accumulated rear to restore the invariant. The result pair from `dequeue` contains the removed element and the new [FIFO queue](../../../computer-science.md#fifo-queue). The constructor should be hidden behind an abstract interface so clients cannot construct an unnormalized representation that invalidates `isEmpty`.

<h4 id="5/a/iii">iii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/a/iii)

The [two-list functional queue](../../../computer-science.md#two-list-functional-queue) has constant-time `peek` and `isEmpty`, but an individual insertion or removal can cost linear time when it reverses a rear list of length $k$. Its useful guarantee is **constant amortized time per operation along a single history starting from empty**.

For the [amortized analysis](../../../computer-science.md#amortized-analysis), each item is consed into the rear once, transferred into the front at most once, and removed at most once. Charge its future reversal to the earlier insertion. Thus $m$ operations perform only $O(m)$ total list-cell work. More formally, use potential $\Phi=C\lvert\texttt{rear}\rvert$, with $C$ sufficient to pay the per-cell reversal cost. An insertion into a nonempty front increases $\Phi$ by $C$ and has constant actual cost; a reversal of $k$ cells decreases $\Phi$ by $Ck$, paying its actual cost. With $\Phi_0=0$ and $\Phi_m\geq0$,

$$
\sum_{i=1}^m c_i=\sum_{i=1}^m\bigl(c_i+\Phi_i-\Phi_{i-1}\bigr)-\Phi_m=O(m).
$$

This [amortized analysis](../../../computer-science.md#amortized-analysis) is deterministic, not an average over a random workload. It assumes subsequent operations use the successive returned versions. If a persistent old version with a long rear is reused repeatedly, each independent dequeue can redo the same reversal. The simple potential accounting does not give constant amortized cost across such a branching history without further [memoization](../../../computer-science.md#memoization) or a stronger persistent [FIFO queue](../../../computer-science.md#fifo-queue) implementation.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Generate every [permutation](../../../combinatorics.md#permutation) of the tail, then insert its missing head at every possible position. The helper preserves order among the elements already present:
```
sml
fun insertEverywhere x [] = [[x]]
  | insertEverywhere x (y :: ys) =
      (x :: y :: ys) ::
      List.map (fn zs => y :: zs) (insertEverywhere x ys);

fun permutations [] = [[]]
  | permutations (x :: xs) =
      List.concat
        (List.map (insertEverywhere x) (permutations xs));
```
The first helper result inserts $x$ before $y$; the mapped recursive results put $y$ back at the front and insert $x$ farther along. For a list of length $k$, it yields exactly $k+1$ positions. The empty list has one [permutation](../../../combinatorics.md#permutation), itself, so the base result is `[[]]`, not `[]`.

For correctness, use [structural induction](../../../foundations-of-mathematics.md#structural-induction). Any [permutation](../../../combinatorics.md#permutation) of `x :: xs` has a unique position containing $x$. Removing that position leaves a [permutation](../../../combinatorics.md#permutation) of `xs`, supplied by the induction hypothesis; reinserting $x$ at its unique position reconstructs the required output. With distinct input elements, neither the tail [permutation](../../../combinatorics.md#permutation) nor the insertion position can be duplicated, so each output occurs once. Consequently **a length-$n$ input yields exactly $n!$ permutations**, in an unrestricted order. The explicit output is large; this is not a polynomial-time enumeration with respect to $n$ alone.

## 6

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

These [Standard ML](../../../computer-science.md#standard-ml) declarations separate the three evaluation and mutation models:
```
sml
datatype 'a olist = ONil | OCons of 'a * 'a olist;

datatype 'a lnode = LNil | LCons of 'a * (unit -> 'a lnode);
type 'a llist = unit -> 'a lnode;

datatype 'a mnode = MNil | MCons of 'a * 'a mnode ref;
type 'a mlist = 'a mnode ref;
```
The ordinary [linked list](../../../computer-science.md#linked-list) is immutable and its spine is built eagerly. A [lazy list](../../../computer-science.md#lazy-list) is a delayed function producing the next constructor, with another delayed function for its tail; it can describe an infinite stream without constructing it in advance. A [mutable list](../../../computer-science.md#mutable-list) uses an [ML reference type](../../../computer-science.md#ml-reference-type) cell for both the root link and every tail link. Updating those cells can remove nodes, including the original head. This [lazy list](../../../computer-science.md#lazy-list) representation delays evaluation but does not automatically implement [memoization](../../../computer-science.md#memoization); repeated forcing can repeat work or effects.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

For a pure predicate `p`, the ordinary [linked list](../../../computer-science.md#linked-list) version copies only the surviving spine:
```
sml
fun filterO p ONil = ONil
  | filterO p (OCons (x, xs)) =
      if p x then OCons (x, filterO p xs)
      else filterO p xs;
```
For a [lazy list](../../../computer-science.md#lazy-list), return a delayed computation. Searching for the next retained element begins only when this computation is forced:
```
sml
fun filterL p stream () =
    case stream () of
        LNil => LNil
      | LCons (x, rest) =>
          if p x then LCons (x, filterL p rest)
          else filterL p rest ();
```
A retained element has a delayed filtered tail, so the whole input is not forced at once. A long run of rejected elements must still be traversed to find the next match. If an infinite [lazy list](../../../computer-science.md#lazy-list) has no matching element beyond the current position, forcing the next result does not terminate; laziness does not promise productivity for every predicate.

The destructive [mutable list](../../../computer-science.md#mutable-list) version operates on the link reaching the current node:
```
sml
fun filterM p link =
    case !link of
        MNil => ()
      | MCons (x, tail) =>
          if p x then filterM p tail
          else (link := !tail; filterM p link);
```
When a node survives, recurse on its tail link. When it fails, bypass it by copying its successor into the same link and inspect that link again, which correctly handles several consecutive rejected nodes. **No new list nodes are allocated.** In particular, changing the root [ML reference type](../../../computer-science.md#ml-reference-type) cell handles deletion of the head. These arguments assume finite acyclic input for the eager and destructive versions and a predicate that does not itself mutate the list. Aliases observe the mutations; a detached node is not promised to disappear from all external references.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Represent a [binary search tree](../../../computer-science.md#binary-search-tree) by:
```
sml
datatype ('k, 'v) dict = Empty
    | Branch of ('k, 'v) dict * 'k * 'v * ('k, 'v) dict;
```
Assume the provided `lookup d key` returns `NONE` or `SOME value`, and `update d (key, value)` returns the updated [binary search tree](../../../computer-science.md#binary-search-tree). Traverse the first dictionary, retaining only a key with the same value in the second:
```
sml
fun intersection equal d1 d2 =
    let
        fun visit Empty result = result
          | visit (Branch (left, key, value, right)) result =
              let
                  val r1 = visit left result
                  val r2 =
                      case lookup d2 key of
                          NONE => r1
                        | SOME other =>
                            if equal (value, other)
                            then update r1 (key, value)
                            else r1
              in
                  visit right r2
              end
    in
        visit d1 Empty
    end;
```
For equality-type values, call `intersection (op =) d1 d2`. An explicit value comparison parameter also handles values for which [Standard ML](../../../computer-science.md#standard-ml) does not define built-in equality. This distinguishes absent keys from defined values without reserving a sentinel value.

Every inserted entry belongs to both input dictionaries with the same value, so the result agrees with each. Conversely, each common equal-valued entry is visited in `d1`, found in `d2`, and inserted. Any dictionary agreeing with both can contain only those entries. Thus **the result is exactly the largest common dictionary**, not merely an intersection of key sets. If `d1` has $m$ entries, lookup height is $h_2$, and maximum result-tree height during insertion is $h_r$, the [time complexity](../../../computer-science.md#time-complexity) is $O(m(1+h_2+h_r))$ for constant-cost comparisons. Logarithmic heights require a balancing assumption; an ordinary unbalanced [binary search tree](../../../computer-science.md#binary-search-tree) can have linear height.

## 7

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/i">i</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/i/solution">Solution</h5>

↑ **Parent:** [I](#7/a/i)

[FIFO page replacement](../../../computer-science.md#fifo-page-replacement) orders resident pages by when they were loaded and evicts the oldest arrival. An access to a resident page does not change this order, so an old but heavily used page can be the next victim.

[LRU replacement](../../../computer-science.md#lru-replacement) records the recency of every page access and evicts the page whose most recent access is oldest. It makes use of [temporal locality](../../../computer-science.md#temporal-locality), but exact reference tracking can require expensive per-access hardware or software bookkeeping.

[CLOCK page replacement](../../../computer-science.md#clock-page-replacement) arranges frames in a circle with a scanning hand and one reference flag per frame. A use sets the flag. During replacement, the hand clears a set flag and moves on, giving that page another chance; it selects an eligible frame with a clear flag. Recent pages tend to survive a scan. [CLOCK page replacement](../../../computer-science.md#clock-page-replacement) approximates recency rather than preserving the exact [LRU replacement](../../../computer-science.md#lru-replacement) ordering. A dirty victim must be written back before its frame is reused, and pinned frames must be skipped.

<h4 id="7/a/ii">ii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#7/a/ii)

Emulate reference observations using [page table](../../../computer-science.md#page-table) protection and [page faults](../../../computer-science.md#page-fault). When resetting a page's reference state, temporarily revoke access to its resident mapping and invalidate any corresponding [translation lookaside buffer](../../../computer-science.md#translation-lookaside-buffer) entry. The first subsequent access traps. The handler recognizes an intentionally protected resident page, sets a software reference flag and restores the mapping without performing a disk read. A later [CLOCK page replacement](../../../computer-science.md#clock-page-replacement) scan can use and clear this software flag.

**One protection fault records the first access after each reset**, rather than trapping on every access. All mappings that can access the frame must be considered. The method requires ordinary memory-protection traps, even though hardware reference bits are absent, and adds a fault cost that native reference flags avoid.

<h4 id="7/a/iii">iii</h4>

↑ **Parent:** [A](#7/a)

<h5 id="7/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#7/a/iii)

**Choose CLOCK for page replacement in a conventional operating system.** Good [temporal locality](../../../computer-science.md#temporal-locality) makes recency valuable, and [CLOCK page replacement](../../../computer-science.md#clock-page-replacement) captures it reasonably well using cheap reference flags. [FIFO page replacement](../../../computer-science.md#fifo-page-replacement) ignores accesses after a page arrives, so it can evict a hot page. Exact [LRU replacement](../../../computer-science.md#lru-replacement) has a stronger recency rule but recording and maintaining the order on every ordinary memory access is usually too costly. This is a practical cost-versus-hit-rate choice, not a theorem that [CLOCK page replacement](../../../computer-science.md#clock-page-replacement) minimizes faults on every reference sequence.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

A [buffer cache](../../../computer-science.md#buffer-cache) keeps copies of device blocks in main memory, indexed by device identity and block number. It reduces expensive repeated device reads and can combine several modifications into one write. It also gives software a controlled place to hold data while requests are in progress.

On a read, the [operating system](../../../computer-science.md#operating-system) looks up the block. A valid cached copy gives a hit and supplies the data; a miss reserves an eligible buffer, writes its old contents first if dirty, issues the device read, and marks the new contents valid when the transfer completes. A write modifies the buffer and marks it dirty. Under a write-back policy, a later flush or eviction sends it to the device; under write-through, completion also waits for the required device write. Dirty state differs from “currently in use”: a pinned or locked buffer cannot simply be reused while a request depends on it.

A [buffer cache](../../../computer-science.md#buffer-cache) needs synchronization for concurrent readers, writers and in-flight transfers, and should avoid inconsistent independent copies of the same block. Explicit flushes and ordering are needed when durable storage is required; caching alone does not guarantee that an acknowledged in-memory update survives a crash. Replacement chooses among eligible buffers, preserving dirty data before reuse.

<h3 id="7/c">c</h3>

↑ **Parent:** [7](#7)

<h4 id="7/c/solution">Solution</h4>

↑ **Parent:** [C](#7/c)

**Use LRU replacement, or a modest recency-based approximation, for eligible buffer-cache entries.** Unlike individual memory accesses, [buffer cache](../../../computer-science.md#buffer-cache) lookups already pass through [operating system](../../../computer-science.md#operating-system) code. Updating an [LRU replacement](../../../computer-science.md#lru-replacement) list on each lookup is therefore practical: remove the accessed entry from its old position and put it at the most-recent end; choose the oldest unpinned entry as victim. A hash lookup plus a doubly linked recency list makes this bookkeeping constant time.

Good [temporal locality](../../../computer-science.md#temporal-locality) favors retaining recently used blocks. [FIFO page replacement](../../../computer-science.md#fifo-page-replacement)'s arrival-only criterion can evict a block used moments ago. [CLOCK page replacement](../../../computer-science.md#clock-page-replacement) can save bookkeeping, but the difficulty of observing arbitrary memory references that motivates it is absent for software-mediated block accesses. Dirty victims require write-back, so a policy can favor an old clean buffer or arrange background cleaning without discarding recent hot data. A long one-pass scan can pollute pure [LRU replacement](../../../computer-science.md#lru-replacement); scan-resistant variants are useful refinements rather than a reason to ignore recency altogether.

## 8

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="8/a">a</h3>

↑ **Parent:** [8](#8)

<h4 id="8/a/i">i</h4>

↑ **Parent:** [A](#8/a)

<h5 id="8/a/i/solution">Solution</h5>

↑ **Parent:** [I](#8/a/i)

A [computer bus](../../../computer-science.md#computer-bus) conventionally has **address, data and control components**. Address information selects a memory location or device register; data carries the value being transferred; control identifies operations and coordinates timing, direction, completion and arbitration. A clock, request/grant and acknowledge signals are examples of control information. These are logical roles, not a requirement for three physically separate wire groups: implementations may multiplex address and data on the same wires.

<h4 id="8/a/ii">ii</h4>

↑ **Parent:** [A](#8/a)

<h5 id="8/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/a/ii)

The processor selects the device's data or control register by presenting its address, either in memory-mapped input-output space or in a distinct port-address space. For a write, it places data on the [computer bus](../../../computer-science.md#computer-bus) and asserts the appropriate write control. For a read, it asserts read control and samples the data supplied by the addressed device. The device recognizes the address and uses the bus timing or acknowledge protocol to indicate completion, including wait states if needed.

The processor uses status registers to determine readiness and control registers to request operations. This register-level communication can be arranged using [polled input-output](../../../computer-science.md#polled-input-output) or [interrupt-driven input-output](../../../computer-science.md#interrupt-driven-input-output); the bus transaction itself and the policy for waiting on a device are separate issues.

<h4 id="8/a/iii">iii</h4>

↑ **Parent:** [A](#8/a)

<h5 id="8/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#8/a/iii)

With [direct memory access](../../../computer-science.md#direct-memory-access), a device can initiate memory transfers, so the processor is no longer the only [computer bus](../../../computer-science.md#computer-bus) master. Requests must be arbitrated to prevent conflicting transfers, and the processor may have to wait while the device owns a shared bus. The [operating system](../../../computer-science.md#operating-system) must supply valid stable buffers and arrange safe completion before reusing them. On a noncoherent system, cached processor copies must be flushed or invalidated as appropriate so processor and device agree on data. These extra initiators also need suitable address and protection controls.

<h4 id="8/a/iv">iv</h4>

↑ **Parent:** [A](#8/a)

<h5 id="8/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#8/a/iv)

**Separate buses match different bandwidth, latency and electrical requirements.** Processor-memory traffic needs high bandwidth and short delays, whereas many peripheral devices are slower or use different signaling protocols. Bridges let them communicate without making every memory transfer obey the slowest peripheral's timing. Separating traffic also reduces contention and electrical loading, and permits expansion or compatibility with older device interfaces. Thus a hierarchical [computer bus](../../../computer-science.md#computer-bus) organization is useful even though all devices are ultimately reachable from the processor.

<h3 id="8/b">b</h3>

↑ **Parent:** [8](#8)

<h4 id="8/b/i">i</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/i/solution">Solution</h5>

↑ **Parent:** [I](#8/b/i)

Add profiling to the timer-[interrupt](../../../computer-science.md#interrupt) handler. When the target [operating-system process](../../../computer-science.md#process-computing) is interrupted while running, record its saved [instruction pointer](../../../computer-science.md#instruction-pointer), map that address to a code region in the executable, and increment an address histogram. Addresses with many samples identify regions consuming a large fraction of execution time. The executable's code can then be disassembled around these addresses even when source and symbolic names are absent.

This is [statistical program profiling](../../../computer-science.md#statistical-program-profiling): uniform samples of running time estimate time spent in code, not exact execution counts. Restrict samples to the desired process and distinguish application execution from unrelated kernel work. A sufficiently fine address histogram and many samples reveal hot loops; varying the sample interval reduces synchronization bias. If exact visit counts rather than time hotspots are needed, arrange breakpoint or single-step traps, or rewrite the binary to add counters, accepting their much larger overhead. **Source code is not required to associate sampled execution with instruction addresses.**

<h4 id="8/b/ii">ii</h4>

↑ **Parent:** [B](#8/b)

<h5 id="8/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#8/b/ii)

Use [strength reduction](../../../computer-science.md#strength-reduction) on the disassembled hot instructions. In a fixed-width wrapping integer model,

$$
\boxed{8x=x\ll3,\qquad 15x=(x\ll4)-x\pmod{2^w}.}
$$

The first replacement is a single left [bit shift](../../../computer-science.md#bit-shift). For the second, preserve the original operand in a register, shift a copy left by four and subtract the original:
```
text
rOriginal = x
rResult = rOriginal << 4
rResult = rResult - rOriginal
```
This avoids a general multiplication if shifts and subtraction are cheaper on the target processor. The two identities hold for positive and negative [two's complement](../../../computer-science.md#two-s-complement) operands when only the low $w$ result bits are required.

Because only a binary is available, patch the machine instructions and adjust displaced branches or use a jump to a replacement code block if the new sequence does not fit. Preserve live registers and the calling convention. If later instructions consume overflow or other condition flags, or the original multiplication produces a double-width result or traps on overflow, matching only the low-word arithmetic is insufficient: those effects must be reproduced or the transformation rejected. Finally, measure the modified program; a fast hardware multiply need not be slower than several replacement instructions.

## 9

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="9/a">a</h3>

↑ **Parent:** [9](#9)

<h4 id="9/a/solution">Solution</h4>

↑ **Parent:** [A](#9/a)

A graphical-component library can provide `protected void paintComponent(Graphics g)` as a subclass customization hook, as in `javax.swing.JComponent`. A subclass overrides it to draw its own contents while the library retains responsibility for the surrounding painting protocol. A [protected method in Java](../../../computer-science.md#protected-method-in-java) is accessible to code in the declaring package and to subclasses in other packages subject to the receiver restriction; it is not simply a public method and not exclusively subclass-visible.

**The benefit is controlled extensibility without exposing an ordinary client operation.** If the method were private, external subclasses could not override and reuse it as the intended hook. If it were public, arbitrary clients could call it outside the normal painting lifecycle and the library would have a wider public contract to maintain. Protected hooks still require documented invariants because subclass code participates in the implementation.

<h3 id="9/b">b</h3>

↑ **Parent:** [9](#9)

<h4 id="9/b/solution">Solution</h4>

↑ **Parent:** [B](#9/b)

An immutable library value such as `java.lang.String` can be a [final class in Java](../../../computer-science.md#final-class-in-java). No class can extend it, so a client receiving a `String` cannot secretly receive a subclass that changes the behavior of its methods. This protects assumptions about value semantics in code using strings as keys or trusted identifiers.

**The benefit is a closed implementation contract.** Without `final`, subclasses might override methods inconsistently or introduce behavior incompatible with the library's intended guarantees. Making a class final does not by itself make its fields immutable; a correct immutable implementation also controls its state. The cost is that clients cannot customize it by inheritance and must instead use composition or a different abstraction.

<h3 id="9/c">c</h3>

↑ **Parent:** [9](#9)

<h4 id="9/c/solution">Solution</h4>

↑ **Parent:** [C](#9/c)

A collections library can supply a genuinely [generic method in Java](../../../computer-science.md#generic-method-in-java) whose own type parameter connects the input element and the result element type:
```
java
static <T> java.util.List<T> oneElement(T item) {
    java.util.List<T> result = new java.util.ArrayList<T>();
    result.add(item);
    return result;
}
```
For example, `List<String> xs = oneElement("sample");` is type-checked without a cast. The method can also construct a `List<Integer>` from an integer object. The standard library's `Collections.singletonList` is another example of this type relationship, though its returned list is unmodifiable.

**The benefit is one reusable implementation with compile-time argument/result consistency.** A raw `List` result would lose element-type information, invite unchecked calls and require casts that may fail later. Separate methods for every element type would duplicate code. Merely enclosing a concrete type in angle brackets, such as returning `List<String>`, does not make a method generic; the method here declares `<T>`. [Type erasure](../../../computer-science.md#type-erasure) means the guarantee is primarily a source-level type check, not a distinct runtime class for each type argument.

<h3 id="9/d">d</h3>

↑ **Parent:** [9](#9)

<h4 id="9/d/solution">Solution</h4>

↑ **Parent:** [D](#9/d)

A growable-array library should store its backing [Java array](../../../computer-science.md#java-array) and logical size in [private fields in Java](../../../computer-science.md#private-field-in-java). Public methods such as `add`, `get` and `remove` can enforce bounds and keep the size consistent with the stored elements. The representation can later change without requiring clients to modify direct field accesses.

**The benefit is preserving invariants through encapsulation.** If clients could assign the size or replace the backing [Java array](../../../computer-science.md#java-array) directly, they could create negative sizes, report elements that do not exist, or modify entries without the library's checks. Accessor methods should not expose a mutable backing object indiscriminately, since a private field alone does not prevent that indirect route. Private fields also do not provide a general security boundary against privileged reflection or native code; the point here is ordinary library access discipline.

<h3 id="9/e">e</h3>

↑ **Parent:** [9](#9)

<h4 id="9/e/solution">Solution</h4>

↑ **Parent:** [E](#9/e)

A collections library can specify a `List<E>` [Java interface](../../../computer-science.md#java-interface), with different implementations such as `ArrayList<E>` and `LinkedList<E>`. A method accepting `List<E>` can iterate or access elements according to the documented list contract without requiring one particular storage representation. Each implementation may also extend its own appropriate class superclass.

**The benefit is separating a usable contract from its implementation.** A parameter restricted to a concrete `ArrayList<E>` would exclude a [linked list](../../../computer-science.md#linked-list) implementation and unnecessarily expose the storage choice. Requiring all providers to extend one concrete class would couple them to its implementation and consume [Java](../../../computer-science.md#java-programming-language)'s single class-inheritance relationship. Interfaces permit multiple implemented contracts, though clients must rely on the stated contract rather than assuming every optional operation is supported or has the same [time complexity](../../../computer-science.md#time-complexity).

## 10

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="10/a">a</h3>

↑ **Parent:** [10](#10)

<h4 id="10/a/solution">Solution</h4>

↑ **Parent:** [A](#10/a)

Allocate a rectangular [Java array](../../../computer-science.md#java-array):
```
java
boolean[][] board = new boolean[1000][1000];
```
[Java](../../../computer-science.md#java-programming-language) initializes every new boolean array element to `false`, so **all cells are initially dead without a filling loop**. This allocates a top-level array of row references and a distinct boolean array for every row.

<h3 id="10/b">b</h3>

↑ **Parent:** [10](#10)

<h4 id="10/b/solution">Solution</h4>

↑ **Parent:** [B](#10/b)

Count only the existing neighbours, excluding the center, then apply the [Conway Game of Life](../../../computer-science.md#conway-game-of-life) transition:
```
java
static boolean nextCell(boolean[][] old, int i, int j) {
    int height = old.length;
    int width = old[0].length;
    int neighbours = 0;
    for (int di = -1; di <= 1; di++) {
        for (int dj = -1; dj <= 1; dj++) {
            if (di == 0 && dj == 0) continue;
            int r = i + di;
            int c = j + dj;
            if (r >= 0 && r < height && c >= 0 && c < width
                    && old[r][c]) {
                neighbours++;
            }
        }
    }
    return neighbours == 3 || (old[i][j] && neighbours == 2);
}
```
The short-circuit bounds test occurs before indexing a neighbour. Out-of-range cells therefore contribute zero, including at corners, and no opposite-edge wrapping occurs. The center is explicitly excluded. **Birth requires three neighbours; survival requires two or three.** The method accepts a nonempty rectangular board and a valid cell index and does not change the old [Java array](../../../computer-science.md#java-array).

<h3 id="10/c">c</h3>

↑ **Parent:** [10](#10)

<h4 id="10/c/solution">Solution</h4>

↑ **Parent:** [C](#10/c)

Use disjoint [Java arrays](../../../computer-science.md#java-array) for the old and new generations:
```
java
static void step(boolean[][] old, boolean[][] next) {
    for (int i = 0; i < old.length; i++) {
        for (int j = 0; j < old[i].length; j++) {
            next[i][j] = nextCell(old, i, j);
        }
    }
}
```
Every decision reads only `old`, so all cells undergo the simultaneous [Conway Game of Life](../../../computer-science.md#conway-game-of-life) transition. The second board must have the same dimensions and share no row arrays with the first. Afterwards swap their references for the following step.

Writing each new cell immediately into the input board would expose a mixture of old and new states to later neighbour counts. The result would depend on the traversal order and would no longer be the specified simultaneous automaton. For example, put the three live cells at $(2,1),(2,2),(2,3)$ on an otherwise dead $5\times5$ board. The simultaneous result is the vertical triple $(1,2),(2,2),(3,2)$. During a naive row-major overwrite, $(1,2)$ becomes live first. The next cell $(1,3)$ now sees that new cell as well as the old cells $(2,2),(2,3)$, so it is incorrectly born with three counted neighbours. This explicitly exhibits the mixture of generations. **A second generation array, or explicit preservation of overwritten old information, is essential.**

<h3 id="10/d">d</h3>

↑ **Parent:** [10](#10)

<h4 id="10/d/solution">Solution</h4>

↑ **Parent:** [D](#10/d)

A [one-row in-place Life update](../../../computer-science.md#one-row-in-place-life-update) needs only one saved row plus a few running sums. Before processing row $i$, `above[j]` stores the old row $i-1$, and all rows $i$ and below are still old. Let a column sum be the number of old live cells in that column in rows $i-1,i,i+1$. The three adjacent column sums, minus the center, give the required neighbour count.
```
java
static int columnSum(boolean[][] board, boolean[] above,
                     int i, int j) {
    int total = above[j] ? 1 : 0;
    if (board[i][j]) total++;
    if (i + 1 < board.length && board[i + 1][j]) total++;
    return total;
}

static void stepInPlace(boolean[][] board) {
    int width = board[0].length;
    boolean[] above = new boolean[width];
    for (int i = 0; i < board.length; i++) {
        int left = 0;
        int middle = columnSum(board, above, i, 0);
        for (int j = 0; j < width; j++) {
            int right = j + 1 < width
                ? columnSum(board, above, i, j + 1) : 0;
            boolean oldCenter = board[i][j];
            int neighbours = left + middle + right
                - (oldCenter ? 1 : 0);
            boolean newCenter = neighbours == 3
                || (oldCenter && neighbours == 2);
            above[j] = oldCenter;
            board[i][j] = newCenter;
            left = middle;
            middle = right;
        }
    }
}
```
When column $j$ is processed, `left` and `middle` were computed before their cells were overwritten. `right` is computed now from untouched column $j+1$, including its untouched `above[j+1]` entry. Thus all three sums describe old cells. Saving `oldCenter` into `above[j]` preserves the old current row for the next row's processing; no later computation in the current row rereads that changed entry, because its old contribution is already in the running sums. This proves the inner-loop invariant and then the row invariant by induction.

Initially `above` is all false, representing the dead exterior above the board. The missing left and right columns contribute zero; the bottom row omits any row below it. Hence all four boundaries follow the required convention. **The update takes $O(HW)$ time and one $W$-element auxiliary boolean vector**, which is exactly a 1000-element vector for the requested board. It uses one board array throughout and does not silently keep a second board or two auxiliary rows.

<h3 id="10/e">e</h3>

↑ **Parent:** [10](#10)

<h4 id="10/e/solution">Solution</h4>

↑ **Parent:** [E](#10/e)

Choose bit zero of each integer to represent the leftmost cell in its group of 32 columns. Then use a quotient to choose the word and a remainder to choose the bit:
```
java
static boolean getBit(int[][] board, int i, int j) {
    return ((board[i][j >>> 5] >>> (j & 31)) & 1) != 0;
}
```
For valid $0\leq i,j<1024$, `j >>> 5` is $\lfloor j/32\rfloor$ and ranges from zero to 31. The [bit mask](../../../computer-science.md#bit-mask) `j & 31` is the offset $j\bmod32$. The logical right [bit shift](../../../computer-science.md#bit-shift) brings the desired bit to position zero; the final mask selects only that bit. **Even bit 31 of a negative stored word is extracted correctly**, because `>>>` inserts zeros. A different convention, with the leftmost cell in the most significant bit, would instead shift by `31 - (j & 31)` and must be used consistently.

## 11

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="11/solution">Solution</h3>

↑ **Parent:** [11](#11)

An [equivalence relation](../../../set-theory.md#equivalence-relation) on a [set](../../../set.md) $A$ is a [binary relation](../../../set-theory.md#binary-relation) that is [reflexive](../../../set-theory.md#reflexive-relation), [symmetric](../../../set-theory.md#symmetric-relation) and [transitive](../../../set-theory.md#transitive-relation): every element is related to itself, related pairs may be reversed, and two consecutive related pairs imply the pair of endpoints is related.

Write $T=R\circ S$, using the printed left-to-right [composition of relations](../../../set-theory.md#composition-of-relations) convention. [Reflexivity](../../../set-theory.md#reflexive-relation) implies $R\subseteq T$ and $S\subseteq T$, and hence $T$ is [reflexive](../../../set-theory.md#reflexive-relation). Reversing a two-step chain gives

$$
T^{-1}=S^{-1}\circ R^{-1}=S\circ R,
$$

since $R,S$ are [symmetric](../../../set-theory.md#symmetric-relation). Also $R\circ R=R$ and $S\circ S=S$: one inclusion is [transitivity](../../../set-theory.md#transitive-relation), and the reverse follows by inserting a reflexive step. These elementary identities supply the equivalences below, without presuming that a composite of [equivalence relations](../../../set-theory.md#equivalence-relation) is automatically an [equivalence relation](../../../set-theory.md#equivalence-relation).

<h3 id="11/i">i</h3>

↑ **Parent:** [11](#11)

<h4 id="11/i/solution">Solution</h4>

↑ **Parent:** [I](#11/i)

A [binary relation](../../../set-theory.md#binary-relation) $T$ is [symmetric](../../../set-theory.md#symmetric-relation) exactly when $T=T^{-1}$. By the reversed-chain identity, condition (i) therefore gives $R\circ S=S\circ R$, in particular condition (iii). Conversely, if $S\circ R\subseteq R\circ S$, reversing both sides gives $R\circ S\subseteq S\circ R$. Thus condition (iii) gives equality and therefore [symmetry](../../../physics.md#symmetry-physics). **Conditions (i) and (iii) are equivalent.**

<h3 id="11/ii">ii</h3>

↑ **Parent:** [11](#11)

<h4 id="11/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#11/ii)

If $T$ is [transitive](../../../set-theory.md#transitive-relation), then $T\circ T\subseteq T$. Since $S,R\subseteq T$, monotonicity of [composition of relations](../../../set-theory.md#composition-of-relations) gives

$$
S\circ R\subseteq T\circ T\subseteq T,
$$

which is condition (iii).

Conversely, condition (iii), associativity of [composition of relations](../../../set-theory.md#composition-of-relations), and the identities $R\circ R=R$, $S\circ S=S$ give

$$
\begin{aligned}
T\circ T&=R\circ S\circ R\circ S\\
&\subseteq R\circ R\circ S\circ S
=R\circ S=T.
\end{aligned}
$$

For a direct chain description, start with $xRaSbRcSz$. Replace its middle $aSbRc$ by $aRdSc$ using condition (iii), then use [transitivity](../../../set-theory.md#transitive-relation) inside $R$ and $S$ to obtain $xRdSz$. Hence $T$ is [transitive](../../../set-theory.md#transitive-relation). **Conditions (ii) and (iii) are equivalent.**

<h3 id="11/iii">iii</h3>

↑ **Parent:** [11](#11)

<h4 id="11/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#11/iii)

The preceding proofs show that this inclusion forces both [symmetry](../../../physics.md#symmetry-physics) and [transitivity](../../../set-theory.md#transitive-relation) of $T$; its [reflexivity](../../../set-theory.md#reflexive-relation) already follows from that of $R,S$. It actually forces equality of the composites, not just a one-way inclusion:

$$
\boxed{S\circ R\subseteq R\circ S\quad\Longleftrightarrow\quad S\circ R=R\circ S.}
$$

This is the [composition of commuting equivalence relations](../../../set-theory.md#composition-of-commuting-equivalence-relations) criterion. It remains to establish the asserted smallest-extension characterization, rather than merely to identify an [equivalence relation](../../../set-theory.md#equivalence-relation).

<h3 id="11/iv">iv</h3>

↑ **Parent:** [11](#11)

<h4 id="11/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#11/iv)

Assume any of conditions (i)–(iii). The established [reflexivity](../../../set-theory.md#reflexive-relation), [symmetry](../../../physics.md#symmetry-physics) and [transitivity](../../../set-theory.md#transitive-relation) make $T$ an [equivalence relation](../../../set-theory.md#equivalence-relation), and it contains both $R,S$. If $E$ is any [equivalence relation](../../../set-theory.md#equivalence-relation) containing $R,S$ and $xRaSz$, then $xEaEz$, so [transitivity](../../../set-theory.md#transitive-relation) of $E$ gives $xEz$. Thus $T\subseteq E$. This proves that **$T$ is the unique smallest equivalence relation containing $R$ and $S$**. Conversely, condition (iv) explicitly makes $T$ an [equivalence relation](../../../set-theory.md#equivalence-relation), so it has properties (i) and (ii). Together these implications prove all four conditions equivalent.

For the final integer example, let $g=\gcd(m,n)$. If $x\equiv y\pmod m$ and $y\equiv z\pmod n$, then $z-x$ is a sum of a multiple of $m$ and a multiple of $n$, so $x\equiv z\pmod g$. Conversely, if $g$ divides $z-x$, [Bezout identity](../../../algebra.md#bezout-identity) provides integers $a,b$ with $z-x=am+bn$. Set $y=x+am$. Then $y-x$ is divisible by $m$ and $z-y$ by $n$, so $xRySz$. Therefore

$$
\boxed{R_m\circ R_n=R_{\gcd(m,n)}=R_n\circ R_m.}
$$

Interchanging $m,n$ gives the other equality. The composite is thus exactly congruence modulo the [greatest common divisor](../../../number-theory.md#greatest-common-divisor), an [equivalence relation](../../../set-theory.md#equivalence-relation), and all four equivalent conditions hold.

## 12

↑ **Parent:** [Paper 5](paper-5.md)

<h3 id="12/solution">Solution</h3>

↑ **Parent:** [12](#12)

For [finite sets](../../../set.md#finite-set) $A_1,\ldots,A_n$, the [inclusion-exclusion principle](../../../combinatorics.md#inclusion-exclusion-principle) states

$$
\boxed{\left|\bigcup_{i=1}^n A_i\right|
=\sum_{\varnothing\ne J\subseteq\{1,\ldots,n\}}
(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.}
$$

To prove it, fix an element in exactly $r$ of the [sets](../../../set.md). If $r=0$, it contributes to neither side. If $r\geq1$, its contribution to the right side is

$$
\sum_{k=1}^r(-1)^{k+1}\binom rk
=1-(1-1)^r=1,
$$

using the [binomial theorem](../../../combinatorics.md#binomial-theorem). This is exactly its contribution to the union. Summing over the finite ambient union proves the formula. Equivalently, the proof is an identity of elementwise membership indicators, so no unproved rule for overlapping sets is being assumed.

Now let the ambient [set](../../../set.md) be all $n!$ [permutations](../../../combinatorics.md#permutation), and let $E_i$ be those fixing element $i$. A [set intersection](../../../set.md#set-intersection) of $k$ specified events $E_i$ has $(n-k)!$ elements: the specified elements are fixed and the others may be permuted freely. Apply [inclusion-exclusion](../../../combinatorics.md#inclusion-exclusion-principle) to the complement of the union of these events. There are $\binom nk$ possible choices of the fixed positions, hence the [derangement](../../../combinatorics.md#derangement-of-a-permutation) count is

$$
\begin{aligned}
f(n)&=\sum_{k=0}^n(-1)^k\binom nk(n-k)!\\
&=\boxed{n!\sum_{k=0}^n\frac{(-1)^k}{k!}}.
\end{aligned}
$$

The $k=0$ term counts the whole ambient [set](../../../set.md) before subtraction; it is not an omitted empty intersection. The formula also gives $f(0)=1$ and $f(1)=0$.

Dividing by the [factorial](../../../combinatorics.md#factorial) and using the convergent power series for the [exponential function](../../../calculus.md#exponential-function) at $-1$ gives

$$
\boxed{\lim_{n\to\infty}\frac{f(n)}{n!}=\sum_{k=0}^\infty\frac{(-1)^k}{k!}=e^{-1}.}
$$

The alternating-series estimate supplies the explicit error bound $|f(n)/n!-e^{-1}|\leq1/(n+1)!$. Thus the limiting proportion is established, not merely identified from the first few values.

## ↑ Ancestors (8)

1. [Ia](../ia.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
