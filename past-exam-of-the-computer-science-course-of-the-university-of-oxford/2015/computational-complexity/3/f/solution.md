<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [binary numeral system](../../../../../binary-numeral-system.md) representation is taken to be canonical, with no leading zeroes, for each positive [integer](../../../../../integer-split.md). Delimiters separate the components of a pair or triple. Syntax, positivity and this representation convention can all be checked in [logarithmic space](../../../../../logarithmic-space.md). The useful principle is that a large [integer](../../../../../integer-split.md) need not be stored in order to compute its digits one at a time.

First consider Add. Let $x_i,y_i,z_i$ denote the [binary digits](../../../../../binary-digit.md) in position $i$, counting from the least significant position $i=0$ and taking out-of-range digits to be zero. Count the component lengths, and let $L$ be their maximum. Start with [arithmetic carry](../../../../../carry-arithmetic.md) $c_0=0$. For $i=0,\ldots,L-1$, compute

$$
t_i=x_i+y_i+c_i,\qquad
s_i=t_i\bmod2,\qquad
c_{i+1}=\left\lfloor\frac{t_i}2\right\rfloor.
$$

Reject if $s_i\ne z_i$ at any position. After the last position, reject if $c_L=1$; otherwise accept. The final [arithmetic carry](../../../../../carry-arithmetic.md) check prevents accepting a result with an omitted high digit, such as the false equality $11_2+11_2=10_2$ obtained by retaining only two [binary digits](../../../../../binary-digit.md).

The [binary-addition carry invariant](../../../../../binary-addition-carry-invariant.md) is

$$
\sum_{j<i}x_j2^j+\sum_{j<i}y_j2^j
=\sum_{j<i}s_j2^j+c_i2^i.
$$

It holds initially and is preserved by the displayed one-column equations. At the end, it proves that the comparisons and the final [arithmetic carry](../../../../../carry-arithmetic.md) check succeed exactly when $x+y=z$. Each requested [binary digit](../../../../../binary-digit.md) is recovered by scanning the corresponding [input](../../../../../input-computer-science.md) field and counting to its position. The length counters, position $i$ and scan counters require $O(\log n)$ [bits](../../../../../bit.md), while $c_i$ and $t_i\in\{0,1,2,3\}$ require constant space. Thus

$$
\boxed{\mathrm{Add}\in\mathrm L.}
$$

For Pal-Add, construct a [logspace transducer](../../../../../logspace-transducer.md) producing the canonical [binary numeral system](../../../../../binary-numeral-system.md) representation of $x+y$. Put $m=\max(|x|,|y|)$. One least-to-most-significant pass using the same recurrence determines the final [arithmetic carry](../../../../../carry-arithmetic.md) $c_m$. Positivity and canonical representations imply that the sum's digit length is

$$
\ell=\begin{cases}m+1,&c_m=1,\\m,&c_m=0.\end{cases}
$$

Indeed, one summand is at least $2^{m-1}$ and both are less than $2^m$. For each output position, from $\ell-1$ down to $0$, recompute the required sum digit from scratch: reset the [arithmetic carry](../../../../../carry-arithmetic.md) to zero and run the column recurrence from position $0$ up to the requested position, reading [input](../../../../../input-computer-science.md) digits by scans. Positions beyond the summands use zero digits, so position $m$ correctly emits the possible final [arithmetic carry](../../../../../carry-arithmetic.md). Emit only the requested digit, then reuse the work space for the next position.

This produces most-significant-first output with $\ell\leq m+1$ digits. It uses $O(\log n)$ work space because it retains only a fixed number of digit indices, lengths, scan counters and one [arithmetic carry](../../../../../carry-arithmetic.md); it never stores the whole sum. A direct implementation with repeated whole-[input](../../../../../input-computer-science.md) scans uses at most $O(n^3)$ [time complexity](../../../../../time-complexity.md), which is sufficient here. Hence $(x,y)\mapsto\operatorname{bin}(x+y)$ is a [logspace-computable function](../../../../../logspace-computable-function.md).

Finally simulate the assumed [L](../../../../../l-complexity.md) decider for [binary palindrome](../../../../../binary-palindrome.md) on this virtual output, using [logspace composition by recomputation](../../../../../logspace-composition-by-recomputation.md) from part (b). Whenever the simulated [input](../../../../../input-computer-science.md) head asks for a digit, rerun the addition [logspace transducer](../../../../../logspace-transducer.md) until it emits that digit. The virtual [input](../../../../../input-computer-science.md) length is $O(n)$, so both its work space and the addition work space are $O(\log n)$. The simulation accepts exactly when the canonical representation of $x+y$ is a [binary palindrome](../../../../../binary-palindrome.md). Therefore

$$
\boxed{\mathrm{Pal\text{-}Add}\in\mathrm L.}
$$

Equivalently, one could directly compare the sum digits in positions $i$ and $\ell-1-i$, recomputing each digit by the same recurrence. This gives the same [logarithmic space](../../../../../logarithmic-space.md) conclusion without ever writing the full sum on a work tape.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
