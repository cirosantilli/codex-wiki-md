# Algorithm

↑ **Parent:** [Computer science](computer-science.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Algorithm)

An algorithm is a finite, precise procedure for transforming an [input](theoretical-computer-science.md#input-computer-science) into an [output](theoretical-computer-science.md#output-computing).

Here "finite" refers to the description: a short [algorithm](algorithm.md) can perform arbitrarily many steps on increasingly large [inputs](theoretical-computer-science.md#input-computer-science). Solving a [computational problem](theoretical-computer-science.md#computational-problem) additionally requires termination and the specified [output](theoretical-computer-science.md#output-computing) on every permitted [input](theoretical-computer-science.md#input-computer-science). State assumptions explicitly: [binary search](#binary-search) requires a [sorted array](data-structure.md#sorted-array).

An [algorithm](algorithm.md) is an idea that can have implementations in different [programming languages](programming-language.md). Its explanation should make three things visible: the permitted [inputs](theoretical-computer-science.md#input-computer-science), the rule for each step, and the meaning of the returned [output](theoretical-computer-science.md#output-computing). [Algorithm correctness](#algorithm-correctness) then separates finding the right answer from eventually finishing; [time complexity](theoretical-computer-science.md#time-complexity) asks how much work finishing requires.

A particularly useful design question is: what knowledge survives each step? In [binary search](#binary-search), it is the location of every possible match inside the remaining candidate range. Writing that fact as a [loop invariant](#loop-invariant) turns an intuitive shortcut into a procedure whose discarded candidates can be justified. This often helps discover the [algorithm](algorithm.md), rather than merely check it afterward.

**Table of contents**

- [Permutation generation](#permutation-generation)
  - [Permutation generation by insertion](#permutation-generation-by-insertion)
- [Maximum all-true rectangle](#maximum-all-true-rectangle)
  - [Row run length](#row-run-length)
- [Analysis of algorithms](#analysis-of-algorithms)
  - [Adversary argument](#adversary-argument)
- [Algorithm design](#algorithm-design)
- [Two-way array partition](#two-way-array-partition)
  - [Three-way array partitioning](#three-way-array-partitioning)
- [Fair enumeration](#fair-enumeration)
  - [Diagonal merging of lazy lists](#diagonal-merging-of-lazy-lists)
- [Multiselection by balanced rank partitioning](#multiselection-by-balanced-rank-partitioning)
- [Median of medians](#median-of-medians)
- [Selection algorithm](#selection-algorithm)
  - [Comparison tournament](#comparison-tournament)
    - [Tournament selection of the three largest elements](#tournament-selection-of-the-three-largest-elements)
  - [Quickselect](#quickselect)
    - [Median-of-three pivot selection](#median-of-three-pivot-selection)
      - [Quadratic median-of-three selection family](#quadratic-median-of-three-selection-family)
  - [Two-sorted-array order statistic](#two-sorted-array-order-statistic)
- [Comparison lower bound for interval disjointness](#comparison-lower-bound-for-interval-disjointness)
- [Finite candidate elimination bound](#finite-candidate-elimination-bound)
- [Duplicate-aware positional scoring](#duplicate-aware-positional-scoring)
- [Quantum algorithm](#quantum-algorithm)
  - [Approximate quantum counting](#approximate-quantum-counting)
  - [Bernstein-Vazirani algorithm](#bernstein-vazirani-algorithm)
    - [Ancilla preparation for the Bernstein-Vazirani algorithm](#ancilla-preparation-for-the-bernstein-vazirani-algorithm)
    - [Hadamard-conjugated linear oracle](#hadamard-conjugated-linear-oracle)
- [Heuristic algorithm](#heuristic-algorithm)
- [Sweep-line algorithm](#sweep-line-algorithm)
- [Four-sum problem](#four-sum-problem)
- [Bit parallelism](#bit-parallelism)
- [Memory usage](#memory-usage)
  - [Auxiliary space](#auxiliary-space)
- [Running time](#running-time)
- [Sorting](#sorting)
- [Unification](#unification)
  - [First-order unification](#first-order-unification)
    - [Robinson unification algorithm](#robinson-unification-algorithm)
  - [Most general unifier](#most-general-unifier)
- [Bostan-Mori algorithm](#bostan-mori-algorithm)
- [Bitwise operation](#bitwise-operation)
  - [Bitwise complement](#bitwise-complement)
  - [Bitwise AND](#bitwise-and)
- [Exponential search](#exponential-search)
  - [Coarse exponential bracketing](#coarse-exponential-bracketing)
  - [Exponential sign bracketing](#exponential-sign-bracketing)
- [Coordinate compression](#coordinate-compression)
- [Two-pointer technique](#two-pointer-technique)
- [Aho-Corasick algorithm](#aho-corasick-algorithm)
  - [Aho-Corasick automaton](#aho-corasick-automaton)
- [Tonelli-Shanks algorithm](#tonelli-shanks-algorithm)
- [String-searching algorithm](#string-searching-algorithm)
  - [Longest repeated substring](#longest-repeated-substring)
  - [FM-index](#fm-index)
  - [Backward search](#backward-search)
  - [Last-to-first mapping](#last-to-first-mapping)
  - [Burrows-Wheeler transform](#burrows-wheeler-transform)
  - [Failure link](#failure-link)
  - [Knuth-Morris-Pratt algorithm](#knuth-morris-pratt-algorithm)
    - [Knuth-Morris-Pratt automaton](#knuth-morris-pratt-automaton)
  - [Border of a string](#border-of-a-string)
  - [Prefix function](#prefix-function)
- [Redelmeier's algorithm](#redelmeier-s-algorithm)
- [Cycle detection](#cycle-detection)
  - [Brent cycle-finding algorithm](#brent-cycle-finding-algorithm)
- [Floyd's cycle-finding algorithm](#floyd-s-cycle-finding-algorithm)
- [Rotating calipers](#rotating-calipers)
- [Meet-in-the-middle algorithm](#meet-in-the-middle-algorithm)
- [Maximum subarray problem](#maximum-subarray-problem)
  - [Maximum-subarray segment summary](#maximum-subarray-segment-summary)
  - [Kadane's algorithm](#kadane-s-algorithm)
- [Search algorithm](#search-algorithm)
  - [Iterative lengthening search](#iterative-lengthening-search)
  - [Staircase matrix search](#staircase-matrix-search)
  - [AND-OR search](#and-or-search)
  - [Two-sum problem](#two-sum-problem)
  - [Ternary lower-bound search](#ternary-lower-bound-search)
  - [Optimal search algorithm](#optimal-search-algorithm)
  - [Complete search algorithm](#complete-search-algorithm)
  - [Tree search](#tree-search)
- [Backtracking](#backtracking)
  - [Backtracking leaf bound](#backtracking-leaf-bound)
- [Sliding-window algorithm](#sliding-window-algorithm)
- [Brute-force search](#brute-force-search)
- [Search pruning](#search-pruning)
- [Number-theoretic sieve](#number-theoretic-sieve)
  - [Odd-only sieve](#odd-only-sieve)
  - [Totient sieve](#totient-sieve)
  - [Smallest prime factor sieve](#smallest-prime-factor-sieve)
  - [Prime sieve](#prime-sieve)
  - [Wheel factorization](#wheel-factorization)
    - [Wheel modulus](#wheel-modulus)
  - [Du Jiao sieve](#du-jiao-sieve)
  - [Min\_25 sieve](#min-25-sieve)
  - [Segmented sieve](#segmented-sieve)
    - [Odd-only segmented sieve](#odd-only-segmented-sieve)
  - [Linear sieve](#linear-sieve)
- [Matrix-chain multiplication](#matrix-chain-multiplication)
  - [Matrix-chain cost model](#matrix-chain-cost-model)
  - [Matrix-chain dynamic programming](#matrix-chain-dynamic-programming)
  - [Matrix-chain split reconstruction](#matrix-chain-split-reconstruction)
- [Greedy algorithm](#greedy-algorithm)
  - [Interval stabbing problem](#interval-stabbing-problem)
  - [Counterexample to removing a longest increasing subsequence](#counterexample-to-removing-a-longest-increasing-subsequence)
  - [Greedy-choice property](#greedy-choice-property)
    - [Exchange argument](#exchange-argument)
  - [Interval scheduling](#interval-scheduling)
    - [Shortest-duration interval scheduling counterexample](#shortest-duration-interval-scheduling-counterexample)
    - [Weighted interval scheduling](#weighted-interval-scheduling)
- [Algorithm correctness](#algorithm-correctness)
  - [Recursion invariant](#recursion-invariant)
  - [Partial correctness](#partial-correctness)
  - [Total correctness](#total-correctness)
    - [Algorithm termination](#algorithm-termination)
  - [Prefix maximum correctness example](#prefix-maximum-correctness-example)
  - [Formal verification](#formal-verification)
    - [Fairness assumption](#fairness-assumption)
    - [Transition system](#transition-system)
      - [Labelled transition system](#labelled-transition-system)
      - [Terminal state](#terminal-state)
      - [Path in a transition system](#path-in-a-transition-system)
        - [Lasso path](#lasso-path)
      - [Transition relation](#transition-relation)
    - [Model checking](#model-checking)
      - [Satisfaction set](#satisfaction-set)
      - [Bounded model checking](#bounded-model-checking)
    - [Summation loop verification](#summation-loop-verification)
    - [Formal specification](#formal-specification)
      - [Constructive specification](#constructive-specification)
      - [Axiomatic specification](#axiomatic-specification)
      - [Frame condition](#frame-condition)
      - [Planning safety certificate](#planning-safety-certificate)
      - [Planning state invariant](#planning-state-invariant)
      - [Precondition](#precondition)
      - [Postcondition](#postcondition)
    - [Binary correctness](#binary-correctness)
  - [Functional correctness](#functional-correctness)
  - [Loop invariant](#loop-invariant)
    - [Loop variant](#loop-variant)
- [Linear search](#linear-search)
  - [Linear search comparison count](#linear-search-comparison-count)
  - [Linear search correctness](#linear-search-correctness)
- [Equality test](#equality-test)
  - [Equality-only grouping lower bound](#equality-only-grouping-lower-bound)
- [Strength reduction](#strength-reduction)
- [Statistical program profiling](#statistical-program-profiling)
- [Depth-first search](#depth-first-search)
  - [Depth-first search parenthesis property](#depth-first-search-parenthesis-property)
  - [Cost-bounded depth-first search](#cost-bounded-depth-first-search)
  - [Explicit-stack depth-first tree traversal](#explicit-stack-depth-first-tree-traversal)
  - [DFS edge classification](#dfs-edge-classification)
    - [Cross edge in depth-first search](#cross-edge-in-depth-first-search)
    - [Tree edge in depth-first search](#tree-edge-in-depth-first-search)
    - [Back edge in depth-first search](#back-edge-in-depth-first-search)
    - [Forward edge in depth-first search](#forward-edge-in-depth-first-search)
  - [DFS discovery and finishing times](#dfs-discovery-and-finishing-times)
  - [Depth-first tree search](#depth-first-tree-search)
  - [Iterative deepening depth-first search](#iterative-deepening-depth-first-search)
- [Memoization](#memoization)
  - [Overlapping subproblems](#overlapping-subproblems)
  - [Memoized Fibonacci evaluation](#memoized-fibonacci-evaluation)
  - [Memoization arithmetic and stack costs](#memoization-arithmetic-and-stack-costs)
  - [Memoization cache contract](#memoization-cache-contract)
    - [Memoization key](#memoization-key)
    - [Memoization cache lifetime](#memoization-cache-lifetime)
- [Recursion (computer science)](#recursion-computer-science)
  - [Guarded recursion](#guarded-recursion)
  - [Mutual recursion](#mutual-recursion)
  - [Recursion tree](#recursion-tree)
    - [Entropy potential for a divide-and-conquer recurrence](#entropy-potential-for-a-divide-and-conquer-recurrence)
  - [Tail recursion](#tail-recursion)
  - [McCarthy 91 function](#mccarthy-91-function)
    - [Generalized McCarthy function](#generalized-mccarthy-function)
  - [Recursive procedure](#recursive-procedure)
  - [Recursive process](#recursive-process)
  - [Factorial recursion and returning frames](#factorial-recursion-and-returning-frames)
  - [Binary array sum by recursion](#binary-array-sum-by-recursion)
  - [Well-founded progress in recursion](#well-founded-progress-in-recursion)
  - [Base case](#base-case)
  - [Recursive call](#recursive-call)
- [Divide-and-conquer algorithm](#divide-and-conquer-algorithm)
  - [Integer rounding in a divide-and-conquer recurrence](#integer-rounding-in-a-divide-and-conquer-recurrence)
  - [Simultaneous minimum and maximum](#simultaneous-minimum-and-maximum)
  - [Array local maximum](#array-local-maximum)
  - [Divide-and-conquer majority element](#divide-and-conquer-majority-element)
  - [CDQ divide and conquer](#cdq-divide-and-conquer)
  - [Divide-and-conquer combination cost](#divide-and-conquer-combination-cost)
  - [Divide-and-conquer product ledger](#divide-and-conquer-product-ledger)
- [Sorting algorithm](#sorting-algorithm)
  - [External merge sort](#external-merge-sort)
  - [Stooge sort](#stooge-sort)
  - [Heapsort](#heapsort)
  - [Prefix reversal sorting](#prefix-reversal-sorting)
  - [Selection sort](#selection-sort)
  - [Quicksort](#quicksort)
    - [Three-way quicksort](#three-way-quicksort)
  - [Bitonic sorting algorithm](#bitonic-sorting-algorithm)
  - [Patience sorting](#patience-sorting)
  - [Sort key](#sort-key)
    - [Sorting record](#sorting-record)
  - [Sortedness](#sortedness)
  - [Sorting permutation preservation](#sorting-permutation-preservation)
  - [Insertion sort](#insertion-sort)
  - [Comparison sort](#comparison-sort)
    - [Comparison sorting lower bound](#comparison-sorting-lower-bound)
  - [Counting sort](#counting-sort)
    - [Counting sort prefix ranges](#counting-sort-prefix-ranges)
    - [Stable record placement in counting sort](#stable-record-placement-in-counting-sort)
  - [Radix sort](#radix-sort)
    - [Least-significant-digit radix sort](#least-significant-digit-radix-sort)
      - [Radix sort suffix invariant](#radix-sort-suffix-invariant)
    - [Stable digit sort](#stable-digit-sort)
    - [Radix sort key encoding](#radix-sort-key-encoding)
  - [Stable sorting](#stable-sorting)
  - [Merge sort](#merge-sort)
    - [FIFO natural merge sort workspace bound](#fifo-natural-merge-sort-workspace-bound)
    - [Sorted run](#sorted-run)
      - [Maximal initial run](#maximal-initial-run)
- [Merge algorithm](#merge-algorithm)
  - [In-place merge](#in-place-merge)
  - [Locally finite sorted-stream merge](#locally-finite-sorted-stream-merge)
  - [K-way merge algorithm](#k-way-merge-algorithm)
- [Binary search](#binary-search)
  - [Lower-bound binary search invariant](#lower-bound-binary-search-invariant)
  - [Minimum search in a rotated distinct array](#minimum-search-in-a-rotated-distinct-array)
  - [Equal-range search](#equal-range-search)
  - [Upper-bound search](#upper-bound-search)
  - [Missing-value search by deficient value intervals](#missing-value-search-by-deficient-value-intervals)
  - [Average successful search in a perfect binary search tree](#average-successful-search-in-a-perfect-binary-search-tree)
  - [Descending boundary search](#descending-boundary-search)
  - [Sign-bracketing binary search](#sign-bracketing-binary-search)
  - [Distinct-index two-sum by suffix lower bounds](#distinct-index-two-sum-by-suffix-lower-bounds)
  - [Lower-bound search](#lower-bound-search)
- [Karatsuba multiplication](#karatsuba-multiplication)
  - [Karatsuba operand splitting](#karatsuba-operand-splitting)
  - [Karatsuba three-product identity](#karatsuba-three-product-identity)
  - [Karatsuba worked multiplication](#karatsuba-worked-multiplication)
  - [Karatsuba carry handling](#karatsuba-carry-handling)
  - [Karatsuba recursion termination](#karatsuba-recursion-termination)
  - [Karatsuba digit-operation cost](#karatsuba-digit-operation-cost)
  - [Karatsuba practical crossover](#karatsuba-practical-crossover)
- [Randomized algorithm](#randomized-algorithm)
  - [Uniform balanced binary sequence sampling](#uniform-balanced-binary-sequence-sampling)
  - [Derandomization](#derandomization)
    - [Method of conditional probabilities](#method-of-conditional-probabilities)
      - [Conditional expectation of a monochromatic clique count](#conditional-expectation-of-a-monochromatic-clique-count)
      - [Conditional expectation choice invariant](#conditional-expectation-choice-invariant)
      - [Conditional expectations for maximum cut](#conditional-expectations-for-maximum-cut)
        - [Conditional expectation cut formula](#conditional-expectation-cut-formula)
        - [Conditional expectations cut example](#conditional-expectations-cut-example)
        - [Conditional expectations algorithm cost](#conditional-expectations-algorithm-cost)
  - [Probabilistic Turing machine](#probabilistic-turing-machine)
  - [One-sided error](#one-sided-error)
    - [RP (complexity)](#rp-complexity)
    - [co-RP](#co-rp)
  - [ZPP](#zpp)
  - [Error reduction for a randomized algorithm](#error-reduction-for-a-randomized-algorithm)
  - [Polynomial identity testing](#polynomial-identity-testing)
    - [Polynomial identity testing over a finite field](#polynomial-identity-testing-over-a-finite-field)
    - [Random evaluation test for a polynomial identity](#random-evaluation-test-for-a-polynomial-identity)
    - [Independent repetition of a polynomial identity test](#independent-repetition-of-a-polynomial-identity-test)

## Permutation generation

↑ **Parent:** [Algorithm](algorithm.md)

### Permutation generation by insertion

↑ **Parent:** [Permutation generation](#permutation-generation)

Generate every [permutation](combinatorics.md#permutation) of a finite [list](data-structure.md#list-abstract-data-type) by recursively permuting its tail and inserting its head into each possible position. For $n$ distinct input elements, every shorter [permutation](combinatorics.md#permutation) has $n$ insertion positions, giving $n(n-1)!=n!$ results. Removing the distinguished head reconstructs the unique shorter [permutation](combinatorics.md#permutation) and insertion position.

## Maximum all-true rectangle

↑ **Parent:** [Algorithm](algorithm.md)

In a [Boolean](programming-language.md#boolean-data-type) [matrix](vector-space.md#matrix), find an axis-aligned [rectangle](euclidean-geometry.md#rectangle) containing only true entries and having maximum area. One approach first records each row's consecutive true run ending at each column. For each possible top-right corner, extend downwards, maintaining the minimum run width and maximizing height times width. This uses $O(N^3)$ [time complexity](theoretical-computer-science.md#time-complexity) on an $N$ by $N$ [matrix](vector-space.md#matrix) after $O(N^2)$ preprocessing.

### Row run length

↑ **Parent:** [Maximum all-true rectangle](#maximum-all-true-rectangle)

The number of consecutive true entries ending at a specified column of one row of a [Boolean](programming-language.md#boolean-data-type) [matrix](vector-space.md#matrix). It is zero at a false entry and otherwise one plus the previous column's [row run length](#row-run-length), taking the value before column zero to be zero.

## Analysis of algorithms

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Analysis_of_algorithms)

Studying an [algorithm](algorithm.md)'s resource use under a stated cost model. [Time complexity](theoretical-computer-science.md#time-complexity), [space complexity](theoretical-computer-science.md#space-complexity) and [amortized analysis](theoretical-computer-science.md#amortized-analysis) answer different questions, so an operation count should specify the input-size parameter and what each primitive operation costs.

### Adversary argument

↑ **Parent:** [Analysis of algorithms](#analysis-of-algorithms)

A method for proving that an [algorithm](algorithm.md) must perform a certain amount of work: supply observations compatible with more than one possible input until enough information has been acquired to distinguish the required outputs. For exact membership in an arbitrary [array](data-structure.md#array-data-structure), answering every inspected location with a value other than the target forces inspection of every location in the absent case, since any uninspected location could contain the target.

## Algorithm design

↑ **Parent:** [Algorithm](algorithm.md)

Constructing an [algorithm](algorithm.md) that meets a stated specification. Choices such as [divide-and-conquer algorithms](#divide-and-conquer-algorithm), [dynamic programming](mathematical-optimization.md#dynamic-programming) and [greedy algorithms](#greedy-algorithm) organize the construction; an [algorithm correctness](#algorithm-correctness) argument establishes that the result meets the specification.

## Two-way array partition

↑ **Parent:** [Algorithm](algorithm.md)

Rearrange an [array](data-structure.md#array-data-structure) segment $a[l,r)$ into a low segment containing values below a pivot $p$ and a high segment containing values at least $p$, preserving the segment's [multiset](set.md#multiset) and leaving the rest of the [array](data-structure.md#array-data-structure) unchanged. The pivot need not itself occur, and either resulting segment may be empty.

An in-place scan maintains indices $l\leq k\leq j\leq r$ with $a[l,k)<p$ and $a[k,j)\geq p$. A low value at $j$ is swapped into position $k$ and advances both indices; a high value advances only $j$. The unexamined length $r-j$ is a [loop variant](#loop-variant). At exit $j=r$, establishing the separation in $\Theta(r-l+1)$ [time complexity](theoretical-computer-science.md#time-complexity) and $O(1)$ auxiliary [space complexity](theoretical-computer-science.md#space-complexity). Equal values consistently belong to the high side.

### Three-way array partitioning

↑ **Parent:** [Two-way array partition](#two-way-array-partition)

Maintain consecutive regions less than a saved pivot value, equal to it, unclassified, and greater than it. Compare the first unclassified entry: move a smaller one into the lower region, advance over an equal one, or exchange a greater one with the final unclassified entry. In the last case the incoming entry still needs classification. Each step shortens the unclassified interval by one. The final equality interval is nonempty when the pivot was selected from the input; [Quickselect](#quickselect) can discard that entire interval when searching another rank. Saving the value avoids accidentally comparing against a pivot index whose contents have moved.

## Fair enumeration

↑ **Parent:** [Algorithm](algorithm.md)

A [fair enumeration](#fair-enumeration) emits every required occurrence after finitely many computation steps. The inputs can be infinite; completeness does not mean waiting until they have all been exhausted. If two [proper lazy lists](data-structure.md#proper-lazy-list) alternate their next available entries, every occurrence reaches the output after finitely many swaps. In contrast, a nested [list comprehension](programming-language.md#list-comprehension) can remain forever in its first infinite inner [list](data-structure.md#list-abstract-data-type). Fairness concerns input occurrences, even when different occurrences happen to have equal values.

### Diagonal merging of lazy lists

↑ **Parent:** [Fair enumeration](#fair-enumeration)

For an outer [proper lazy list](data-structure.md#proper-lazy-list) of inner [proper lazy lists](data-structure.md#proper-lazy-list), introduce row $i$ in round $i$ and advance each active row once per round. Discard an active row when its terminating constructor is observed. Each round inspects finitely many rows, and the entry at row index $i$, within-row index $j$, is emitted in round $i+j$. Every earlier round has finite work, proving [fair enumeration](#fair-enumeration) of all occurrences.

An implementation can keep a finite [list](data-structure.md#list-abstract-data-type) of row remainders, append at most one newly introduced row, collect one head from every nonempty remainder, and retain their tails for the next round. It must not first combine all not-yet-introduced rows. In fact, `foldr interleave [] ([1,2] : repeat [])` can emit `1` and then block before `2`; [diagonal merging of lazy lists](#diagonal-merging-of-lazy-lists) emits both. If infinitely many empty rows remain after the final output, detecting termination is impossible in general: the [absence-detection obstruction for infinite lists](data-structure.md#absence-detection-obstruction-for-infinite-lists) prevents a universal promise of a terminating empty tail, while every required occurrence can still be emitted.

## Multiselection by balanced rank partitioning

↑ **Parent:** [Algorithm](algorithm.md)

To find the order statistics at ranks $k,2k,\ldots,n$ when $n/k$ is a power of two, partition into equal lower and upper rank halves and recurse, stopping at blocks of size $k$. Return each leaf block's maximum. Half boundaries are multiples of $k$, so these leaf maxima are exactly the requested ranks. Linear-time [selection](#selection-algorithm) gives total $\Theta(n)$ partition work per internal level and $\Theta(n)$ leaf work, hence $\Theta(n(1+\log(n/k)))$ overall. The shorter displayed bound applies when $n/k\geq2$.

## Median of medians

↑ **Parent:** [Algorithm](algorithm.md)

For deterministic linear-time [selection](#selection-algorithm), group keys into fives, compute the median of each group, and recursively select the median of those medians as a pivot. Apart from bounded end effects, at least $3n/10$ keys lie on either side. Thus the selection cost satisfies $T(n)\leq T(\lceil n/5\rceil)+T(7n/10+O(1))+O(n)=O(n)$, since the fractions sum to $9/10<1$. A [strong induction](foundations-of-mathematics.md#strong-induction) with sufficiently large linear coefficient absorbs the lower-order terms.

## Selection algorithm

↑ **Parent:** [Algorithm](algorithm.md)

Find one specified [order statistic](probability-theory.md#order-statistic) without sorting every element. Partitioning about a pivot retains only the side containing the requested rank. [Median of medians](#median-of-medians) guarantees a balanced enough pivot to give worst-case linear [time complexity](theoretical-computer-science.md#time-complexity).

### Comparison tournament

↑ **Parent:** [Selection algorithm](#selection-algorithm)

Pair candidates from a [totally ordered set](set.md#totally-ordered-set) and retain the greater one from each comparison until one winner remains. Every other candidate loses once, so $n-1$ key comparisons suffice to find the [maximum](set.md#maximum-of-a-subset-of-a-total-order) of $n$ distinct values. A balanced tournament on $2^m$ inputs gives the winner $m$ direct losers. Retaining each loser's own defeat record preserves information for finding later order statistics. The comparison records form a rooted tree and are distinct from a graph-theoretic [tournament](graph-theory.md#tournament-graph-theory), which includes a directed comparison between every pair.

#### Tournament selection of the three largest elements

↑ **Parent:** [Comparison tournament](#comparison-tournament)

After a balanced [comparison tournament](#comparison-tournament), the second-largest element is the [maximum](set.md#maximum-of-a-subset-of-a-total-order) among the winner's $m$ direct losers. The third-largest must have lost directly to the winner or to that second-largest element: no smaller element could defeat it. Excluding the known top two leaves at most $(m-1)+(m-1)$ candidates, because the second-largest won at most $m-1$ earlier comparisons. The three stages use at most $(n-1)+(m-1)+(2m-3)$ key comparisons, proving the displayed bound. Defeat records must retain their earlier subtrees; keeping only the overall winner's direct-loser values discards information used by the last stage.

### Quickselect

↑ **Parent:** [Selection algorithm](#selection-algorithm)

A [selection algorithm](#selection-algorithm) that uses [array partitioning](#two-way-array-partition) around a pivot and recursively searches only the side containing the desired [order statistic](probability-theory.md#order-statistic). If there are $s$ entries before the placed pivot, an earlier rank is unchanged and a later rank is reduced by $s+1$. Segment length strictly decreases, proving [algorithm termination](#algorithm-termination). The same reduction can update local bounds in a loop, using constant auxiliary space.

Balanced reductions give linear work by a [geometric series](sequence-and-series.md#geometric-series), while repeatedly discarding only a constant number of entries can give quadratic work. For distinct entries and independent uniform random pivots, a pivot in the middle half has probability at least one half and reduces the retained length to at most three quarters, up to rounding. The expected number of attempts for each such reduction is bounded, so summing expected work over geometric size scales gives $O(n)$ expected time. This random-pivot guarantee is not a worst-case guarantee for a deterministic median-of-three heuristic. With duplicates and a strict two-way partition, random pivot choice alone can also fail to shrink an all-equal segment; a three-way partition treats equal keys together.

#### Median-of-three pivot selection

↑ **Parent:** [Quickselect](#quickselect)

Choose the median value among the first, middle and last entries of an active [array](data-structure.md#array-data-structure) segment. For at least three distinct sampled values, the selected value cannot be the whole segment's minimum or maximum. It can still be the second-smallest or second-largest value, so a balanced split does not follow. Coincident sample indices in segments of length one or two can be handled by the same comparison code. Ties must also have a defined branch policy.

##### Quadratic median-of-three selection family

↑ **Parent:** [Median-of-three pivot selection](#median-of-three-pivot-selection)

A distinct-input counterexample for [Quickselect](#quickselect) that chooses the first/middle/last median, reserves it at the last slot, scans lower values to the front, and finally swaps the pivot into place. Let $A_n$ be the following [permutation](combinatorics.md#permutation) of $0,\ldots,n-1$. For $n<4$, take increasing order. For $n\geq4$, let $B=A_{n-2}+2$ componentwise and $m=\lfloor n/2\rfloor$, then set

$$
A_n(0)=1,\quad A_n(m)=0,\quad A_n(n-1)=B(m-2),\quad A_n(1)=B(n-3),
$$

and put $A_n(j)=B(j-2)$ at every other index $2\leq j\leq n-2$. These assignments use every entry of $B$ once and add zero and one, so they really define a [permutation](combinatorics.md#permutation).

The sampled values are $1,0,B(m-2)$, with the last at least two, so the pivot is one. After the initial pivot swap, the only lower value is the zero at index $m$. Moving it to the front places the displaced $B(m-2)$ at its intended tail position. The final pivot swap moves $B(n-3)$ from index one to the last position. Every other tail entry already has its intended position. Thus the complete partitioned result is exactly $[0,1]$ followed by $B$.

Selecting the maximum consequently repeats the same construction on $n-2$ entries. If $C(n)$ counts only pivot comparisons made by the partition scan, then $C(n)=n-1+C(n-2)$, with $C(1)=0$ and $C(2)=1$. Hence $C(n)=\lfloor n^2/4\rfloor$ and total runtime is $\Theta(n^2)$. For example, $A_6=[1,4,3,0,2,5]$. This disproves a linear worst-case claim even when every value is distinct.

### Two-sorted-array order statistic

↑ **Parent:** [Selection algorithm](#selection-algorithm)

To obtain the $k$-th smallest entry of two ascending [sorted arrays](data-structure.md#sorted-array) of lengths $m,n$, choose prefix lengths $i,j$ with $i+j=k$. Search $\max(0,k-n)\le i\le\min(m,k)$ for the two boundary inequalities in the title, treating missing left boundaries as $-\infty$ and missing right boundaries as $+\infty$. Then all $k$ selected entries precede all unselected entries, so their largest boundary value is the answer. If $A_L>B_R$, decrease $i$; if $B_L>A_R$, increase $i$. These failures are monotone because one prefix grows as the other shrinks. [Binary search](#binary-search) thus takes $O(\log(\min(m,n)+1))$ comparisons when the shorter [array](data-structure.md#array-data-structure) supplies the searched prefix. Repeated values retain their multiplicities in the ranks.

## Comparison lower bound for interval disjointness

↑ **Parent:** [Algorithm](algorithm.md)

Deciding whether $n$ open real intervals are pairwise disjoint has comparison complexity $\Theta(n\log n)$. Sort by left endpoint and scan the maximum previous right endpoint for the upper bound. For the lower bound, map integer keys $z_i$ to $(2z_i,2z_i+1)$. Such intervals intersect exactly when the original integers agree. Each comparison between endpoints $2z_i+a$ and $2z_j+b$, with $a,b\in\{0,1\}$, is determined by a comparison of $z_i,z_j$ and their fixed offsets, so the reduction preserves the [comparison model](theoretical-computer-science.md#comparison-model). Apply the [element distinctness problem](theoretical-computer-science.md#element-distinctness-problem) lower bound.

## Finite candidate elimination bound

↑ **Parent:** [Algorithm](algorithm.md)

Suppose a finite candidate [set](set.md) of size $N$ contains the truth, every query chooses a current candidate, and each wrong reply eliminates that candidate while retaining the truth. Then at most $N-1$ wrong queries occur. If a correct reply uniquely identifies the truth, an infinite strategy of this kind eventually repeats the true candidate; stopping when only one candidate remains takes at most $N-1$ replies. The proof is the strictly decreasing positive [cardinality](cardinal-number.md#cardinality) of the surviving candidate set after every nonidentifying round.

## Duplicate-aware positional scoring

↑ **Parent:** [Algorithm](algorithm.md)

To score a guess against a fixed-length secret, first reserve every equal-position match. For the remaining positions, consume at most one unused secret occurrence for each cow. This two-stage rule prevents an earlier wrong-position token from using the occurrence needed for a later positional match. The sum of bull and cow counts is the [multiset overlap](set.md#multiset-overlap) of the two sequences. With only [equality tests](#equality-test), deletion from a list gives a quadratic-time implementation; token-count maps can improve the allocation step when a suitable key representation is available.

## Quantum algorithm

↑ **Parent:** [Algorithm](algorithm.md)

A computational procedure using quantum state preparation, controlled operations and measurement, together with any required classical processing. Complexity counts the relevant operations and repetitions; a large superposition is not itself a guarantee of a useful speedup.

### Approximate quantum counting

↑ **Parent:** [Quantum algorithm](#quantum-algorithm)

Approximate quantum counting estimates the number $k$ of [satisfying assignments](theoretical-computer-science.md#satisfying-assignment) of a [Boolean function](analysis-of-boolean-functions.md#boolean-function), using a [quantum oracle](theoretical-computer-science.md#quantum-oracle) and [quantum measurement](quantum-measurement.md). Controlled repetitions of a [Grover search algorithm](quantum-theory.md#grover-s-algorithm) iteration let [quantum interference](quantum-system.md#quantum-interference) reveal the count. For one input [bit](information-theory.md#bit), a [Hadamard test](quantum-theory.md#hadamard-test) can give [Pauli Z gate](quantum-theory.md#pauli-z-gate) [expectation value](quantum-system.md#expectation-value) $1-k$: with the complemented [phase oracle](theoretical-computer-science.md#phase-oracle) $U_f=\operatorname{diag}(2f(0)-1,2f(1)-1)$ and $G=-XU_f$, use $\langle+|X=\langle+|$ to obtain $\langle+|G|+\rangle=-[(2f(0)-1)+(2f(1)-1)]/2=1-k$. Repeated preparations estimate this [expectation value](quantum-system.md#expectation-value); one binary measurement result does not distinguish all three counts $0,1,2$.

### Bernstein-Vazirani algorithm

↑ **Parent:** [Quantum algorithm](#quantum-algorithm)

The [Bernstein-Vazirani algorithm](#bernstein-vazirani-algorithm) identifies the coefficient string of a [linear Boolean function](analysis-of-boolean-functions.md#linear-boolean-function) with one [Boolean quantum oracle](quantum-theory.md#boolean-quantum-oracle) call. It contrasts with the $n$ calls required by the [classical query complexity of linear Boolean function identification](theoretical-computer-science.md#classical-query-complexity-of-linear-boolean-function-identification). Prepare the data [qubits](quantum-system.md#qubit) at $|0\rangle^{\otimes n}$ and an [ancilla qubit](quantum-information-theory.md#ancilla-qubit) at $|1\rangle$, apply a [Hadamard gate](quantum-theory.md#hadamard-gate) to every wire, query the [function oracle](theoretical-computer-science.md#function-oracle), and apply the [Hadamard gates](quantum-theory.md#hadamard-gate) again. The full output is $|a\rangle|1\rangle$.

The mechanism is [Bernstein-Vazirani phase kickback](quantum-theory.md#bernstein-vazirani-phase-kickback). The [Pauli X gate](quantum-theory.md#pauli-x-gate) has [eigenvector](linear-operator-theory.md#eigenvector) $|-\rangle=(|0\rangle-|1\rangle)/\sqrt2$ with [eigenvalue](linear-operator-theory.md#eigenvalue) $-1$. Thus the target flips become relative [quantum phases](quantum-system.md#quantum-phase) on the data, giving

$$
2^{-n/2}\sum_x(-1)^{a\cdot x}|x\rangle
=\bigotimes_{j=1}^{n}\frac{|0\rangle+(-1)^{a_j}|1\rangle}{\sqrt2}.
$$

The final [Hadamard transform](quantum-theory.md#hadamard-transform) maps this product to $|a\rangle$, so [computational-basis measurement](quantum-theory.md#quantum-measurement-in-the-computational-basis) recovers every coefficient with certainty. The [ancilla preparation for the Bernstein-Vazirani algorithm](#ancilla-preparation-for-the-bernstein-vazirani-algorithm) ensures the required minus sign, and the [Hadamard-conjugated linear oracle](#hadamard-conjugated-linear-oracle) gives an exact [quantum circuit](quantum-circuit.md) interpretation. One query is optimal for $n\ge1$, since without a query the output cannot depend on the unknown string.

#### Ancilla preparation for the Bernstein-Vazirani algorithm

↑ **Parent:** [Bernstein-Vazirani algorithm](#bernstein-vazirani-algorithm)

The displayed [Bernstein-Vazirani algorithm](#bernstein-vazirani-algorithm) prepares its [ancilla qubit](quantum-information-theory.md#ancilla-qubit) in the [computational-basis state](quantum-theory.md#computational-basis-state) $|1\rangle$ before the first [Hadamard gate](quantum-theory.md#hadamard-gate). At the [function oracle](theoretical-computer-science.md#function-oracle) it is therefore the $-1$ [eigenstate](energy-eigenvalue.md#eigenstate) $|-\rangle$ of the [Pauli X gate](quantum-theory.md#pauli-x-gate), which enables [phase kickback](quantum-theory.md#phase-kickback). Preparing $|0\rangle$ instead yields $|+\rangle$ at the [function oracle](theoretical-computer-science.md#function-oracle); target flips leave this state unchanged, so the data contain no information about $a$.

The [Hadamard-conjugated linear oracle](#hadamard-conjugated-linear-oracle) makes the more general statement transparent. With zero data and initial [ancilla qubit](quantum-information-theory.md#ancilla-qubit) $\alpha|0\rangle+\beta|1\rangle$, the full fixed [quantum circuit](quantum-circuit.md) outputs

$$
\alpha|0\rangle^{\otimes n}|0\rangle+\beta|a\rangle|1\rangle.
$$

For nonzero $a$, the correct data outcome has [probability](probability-theory.md#probability) $|\beta|^2$. To obtain exact identification for all $a$, this preparation must have $\alpha=0$, so it is $|1\rangle$ up to [global phase](quantum-system.md#global-phase). This is a condition on the prescribed preparation circuit: any alternative [quantum state preparation](quantum-circuit.md#quantum-state-preparation) that supplies $|-\rangle$ at the [function oracle](theoretical-computer-science.md#function-oracle) is equivalent.

#### Hadamard-conjugated linear oracle

↑ **Parent:** [Bernstein-Vazirani algorithm](#bernstein-vazirani-algorithm)

Let $U_a|x\rangle|b\rangle=|x\rangle|b\oplus(a\cdot x)\rangle$ be the [Boolean quantum oracle](quantum-theory.md#boolean-quantum-oracle) for a [linear Boolean function](analysis-of-boolean-functions.md#linear-boolean-function), and put $W=H^{\otimes(n+1)}$. The [CNOT gates](quantum-theory.md#controlled-not-gate) $C_{j\to y}^{a_j}$ implement $U_a$, where the data wires control the [ancilla qubit](quantum-information-theory.md#ancilla-qubit). [CNOT control reversal in the Hadamard basis](quantum-theory.md#cnot-control-reversal-in-the-hadamard-basis) and $W^2=I$ imply the exact [unitary operator](vector-space.md#unitary-operator) identity

$$
WU_aW=\prod_{j=1}^{n}C_{y\to j}^{a_j},
\qquad
WU_aW|x\rangle|b\rangle=|x\oplus ba\rangle|b\rangle.
$$

Here $\oplus$ on strings is [bitwise exclusive or](theoretical-computer-science.md#exclusive-or). To conjugate a product, insert $W^2=I$ between its factors; each factor reverses its control and target, and the unused [Hadamard gates](quantum-theory.md#hadamard-gate) cancel. The [global phase](quantum-system.md#global-phase) is exactly $1$. In particular, the identity holds on arbitrary [quantum superpositions](quantum-system.md#quantum-superposition), not only on the initialized inputs of the [Bernstein-Vazirani algorithm](#bernstein-vazirani-algorithm).

## Heuristic algorithm

↑ **Parent:** [Algorithm](algorithm.md)

A [heuristic algorithm](#heuristic-algorithm) uses a selective search or approximation to obtain a useful result efficiently, without a general guarantee of finding the exact optimum.

## Sweep-line algorithm

↑ **Parent:** [Algorithm](algorithm.md)

## Four-sum problem

↑ **Parent:** [Algorithm](algorithm.md)

## Bit parallelism

↑ **Parent:** [Algorithm](algorithm.md)

## Memory usage

↑ **Parent:** [Algorithm](algorithm.md)

### Auxiliary space

↑ **Parent:** [Memory usage](#memory-usage)

The extra working storage required by an [algorithm](algorithm.md), excluding the storage occupied by its input. This includes temporary tables and the stack of active [recursive calls](#recursive-call).

## Running time

↑ **Parent:** [Algorithm](algorithm.md)

## Sorting

↑ **Parent:** [Algorithm](algorithm.md)

Rearranging a finite [sequence](sequence-and-series.md#sequence) according to a specified order while preserving its entries and their multiplicities. A [sorting algorithm](#sorting-algorithm) performs this operation; [lexicographic order](extremal-set-theory.md#lexicographic-order) supplies a common order for tuples or strings.

## Unification

↑ **Parent:** [Algorithm](algorithm.md)

Unification seeks substitutions for variables that make symbolic terms identical. First-order unification compares matching constructors recursively; an [occurs check](programming-language.md#occurs-check) rejects substitutions that would make a variable contain itself.

### First-order unification

↑ **Parent:** [Unification](#unification)

First-order unification seeks substitutions making first-order terms identical. Constructor decomposition and the [occurs check](programming-language.md#occurs-check) produce a [most general unifier](#most-general-unifier) when one exists.

#### Robinson unification algorithm

↑ **Parent:** [First-order unification](#first-order-unification)

### Most general unifier

↑ **Parent:** [Unification](#unification)

A most general unifier is a unifying substitution through which every other unifier factors by a further substitution. It records exactly the equality constraints forced by the terms.

## Bostan-Mori algorithm

↑ **Parent:** [Algorithm](algorithm.md)

The Bostan-Mori algorithm extracts a distant coefficient from a [rational generating function](sequence-and-series.md#rational-generating-function) $P(x)/Q(x)$ by multiplying both by $Q(-x)$. The new denominator is even; retaining the appropriate even or odd numerator coefficients halves the coefficient index at each step.

## Bitwise operation

↑ **Parent:** [Algorithm](algorithm.md)

### Bitwise complement

↑ **Parent:** [Bitwise operation](#bitwise-operation)

### Bitwise AND

↑ **Parent:** [Bitwise operation](#bitwise-operation)

Bitwise AND combines binary representations position by position, setting a bit exactly when it is set in every operand. For [bit masks](programming-language.md#bit-mask) representing sets, it computes intersection.

## Exponential search

↑ **Parent:** [Algorithm](algorithm.md)

### Coarse exponential bracketing

↑ **Parent:** [Exponential search](#exponential-search)

To discover a positive unknown [integer](integer.md) $m$ by comparisons, test the thresholds $2^k,2^{2k},\ldots$ for fixed $k\ge1$. If the first threshold not smaller than $m$ has index $j$, fewer than $2^{kj}$ candidates remain and [binary search](#binary-search) needs at most $kj+O(1)$ comparisons. Since $j\le\log_2(m)/k+1$, the total is at most $(1+1/k)\log_2 m+O_k(1)$. Choosing $k\ge1/\epsilon$ makes the leading constant at most $1+\epsilon$; the additive constant may depend on $\epsilon$.

### Exponential sign bracketing

↑ **Parent:** [Exponential search](#exponential-search)

If $f(0)<0$ and $f(x)>0$ for all sufficiently large positive $x$, testing $1,2,4,\ldots$ eventually finds a positive endpoint. Keep the previous nonpositive endpoint to obtain a bracket. If $t$ is the first successful exponent, there are $t+1$ endpoint tests. Subsequent [sign-bracketing binary search](#sign-bracketing-binary-search) in the last interval takes $t-1$ tests for $t\geq1$, since its width is $2^{t-1}$. No monotonicity is needed, though intermediate sign crossings may be skipped. Fixed-width [integer overflow](programming-language.md#integer-overflow) and unreliable floating-point signs require explicit handling; eventual real positivity alone does not guarantee representable machine endpoints.

## Coordinate compression

↑ **Parent:** [Algorithm](algorithm.md)

Coordinate compression replaces coordinates by a smaller representation while retaining the order or distance information needed by an [algorithm](algorithm.md). Rank compression retains only order; geometry-specific transformations may instead remove known gaps or widths.

## Two-pointer technique

↑ **Parent:** [Algorithm](algorithm.md)

## Aho-Corasick algorithm

↑ **Parent:** [Algorithm](algorithm.md)

The Aho-Corasick algorithm matches multiple patterns in a [string](foundations-of-mathematics.md#string) using a [trie](data-structure.md#trie) equipped with failure links. After preprocessing the patterns, it scans the input while reporting every pattern ending at each position.

### Aho-Corasick automaton

↑ **Parent:** [Aho-Corasick algorithm](#aho-corasick-algorithm)

An Aho-Corasick automaton stores a [trie](data-structure.md#trie) of patterns together with failure links and pattern-output information. It supports simultaneous pattern matching by the [Aho-Corasick algorithm](#aho-corasick-algorithm).

## Tonelli-Shanks algorithm

↑ **Parent:** [Algorithm](algorithm.md)

The Tonelli-Shanks algorithm finds a [square root](algebra.md#square-root) of a [quadratic residue](quadratic-residue.md) [modulo](modular-arithmetic.md#modulo-operation) an [odd prime](prime-number.md#odd-prime). It uses the decomposition of the prime minus one into an odd part and a [power of two](integer.md#power-of-two) to successively correct a candidate root.

## String-searching algorithm

↑ **Parent:** [Algorithm](algorithm.md)

### Longest repeated substring

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

A longest repeated substring is a maximum-length contiguous [string](foundations-of-mathematics.md#string) occurring at two distinct starting positions in a text. The occurrences may overlap unless a nonoverlap constraint is explicitly imposed. It can be found by comparing all pairs of suffixes, or by taking the maximum longest-common-prefix length of adjacent entries of a [suffix array](data-structure.md#suffix-array). The latter characterization concerns correctness; the time needed to build the [suffix array](data-structure.md#suffix-array) depends on the construction algorithm.

### FM-index

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

An [FM-index](#fm-index) is a compressed text index supporting [backward search](#backward-search) through the [Burrows-Wheeler transform](#burrows-wheeler-transform) and occurrence counts. Character [rank queries](data-structure.md#rank-query) locate a matching interval; sampled [suffix array](data-structure.md#suffix-array) positions then allow the actual text positions to be recovered. Query length, number of matches and the chosen sampling density control different parts of the search cost.[§§3.1–3.2, counting and locating occurrences](computer-science-bibliography.md#opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others)

### Backward search

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

[Backward search](#backward-search) finds a query's matching interval in a [suffix array](data-structure.md#suffix-array) by processing the query from right to left. With inclusive one-based interval $[l,r]$, prepending $c$ changes it to $[C(c)+\operatorname{Occ}(c,l-1)+1,C(c)+\operatorname{Occ}(c,r)]$. An empty interval means no match. This works through the occurrence-order property of the [last-to-first mapping](#last-to-first-mapping).[§3.1, Figure 1, BW Search](computer-science-bibliography.md#opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others)

### Last-to-first mapping

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

In a sorted [cyclic rotation](foundations-of-mathematics.md#cyclic-rotation) matrix, the [last-to-first mapping](#last-to-first-mapping) sends the $k$th occurrence of a character in the last column to its $k$th occurrence in the first column. For one-based rows, $\operatorname{LF}(r)=C(L_r)+\operatorname{Occ}(L_r,r)$, where $C(c)$ counts smaller characters and $\operatorname{Occ}(c,r)$ counts $c$ in the first $r$ entries of the last column. It moves a rotation's start one character backwards cyclically. Equal characters retain the [lexicographic order](extremal-set-theory.md#lexicographic-order) of their following sequences, which proves the occurrence-order rule.[§2, properties (a)–(b) and LF-mapping](computer-science-bibliography.md#opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others)

### Burrows-Wheeler transform

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

The [Burrows-Wheeler transform](#burrows-wheeler-transform) appends a unique smallest terminator to a [string](foundations-of-mathematics.md#string), sorts its [cyclic rotations](foundations-of-mathematics.md#cyclic-rotation) in [lexicographic order](extremal-set-theory.md#lexicographic-order), and records the last column. It is reversible because the first and last columns contain the same characters and the [last-to-first mapping](#last-to-first-mapping) preserves the occurrence order of each character. The resulting letter arrangement supports both compression and [backward search](#backward-search).[§2, Background: sorted cyclic shifts and inversion](computer-science-bibliography.md#opportunistic-data-structures-with-applications-by-paolo-ferragina-and-others)

### Failure link

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

A transition to a shorter suffix match after an attempted extension fails. In a [Knuth-Morris-Pratt automaton](#knuth-morris-pratt-automaton), the [prefix function](#prefix-function) determines the next shorter matching prefix.

### Knuth-Morris-Pratt algorithm

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

#### Knuth-Morris-Pratt automaton

↑ **Parent:** [Knuth-Morris-Pratt algorithm](#knuth-morris-pratt-algorithm)

### Border of a string

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

### Prefix function

↑ **Parent:** [String-searching algorithm](#string-searching-algorithm)

For a string $s$, the value $\pi_i$ is the length of the longest proper prefix of $s_0\cdots s_i$ that is also its suffix. Repeatedly following these lengths lists all proper [borders of a string](#border-of-a-string); this is the failure-link information used by the [Knuth-Morris-Pratt algorithm](#knuth-morris-pratt-algorithm).

<h2 id="redelmeier-s-algorithm">Redelmeier's algorithm</h2>

↑ **Parent:** [Algorithm](algorithm.md)

An [algorithm](algorithm.md) for enumerating [polyominoes](combinatorics.md#polyomino) by maintaining included cells, an ordered frontier of untried cells, and excluded cells. Exploring inclusion and exclusion in a consistent order prevents different growth histories from counting the same rooted shape repeatedly.

## Cycle detection

↑ **Parent:** [Algorithm](algorithm.md)

Determine whether repeated deterministic updates revisit a state, and optionally find the preperiod and cycle length. Recording all visited states uses memory proportional to the visited orbit. [Floyd's cycle-finding algorithm](#floyd-s-cycle-finding-algorithm) detects repetition with constant extra memory.

### Brent cycle-finding algorithm

↑ **Parent:** [Cycle detection](#cycle-detection)

A constant-memory [algorithm](algorithm.md) for detecting the eventual cycle in a sequence generated by repeated [function](function.md) evaluation. It holds a checkpoint fixed while a second pointer advances, doubling the checkpoint interval when exhausted; a second pass locates the start of the cycle.

<h2 id="floyd-s-cycle-finding-algorithm">Floyd's cycle-finding algorithm</h2>

↑ **Parent:** [Algorithm](algorithm.md)

For a deterministic iteration $x_{n+1}=f(x_n)$ on a [finite set](set.md#finite-set), move one pointer by one step and another by two steps. They eventually meet inside the repeated cycle. Restarting one pointer at the initial state and advancing both by one step locates the cycle entrance; a further traversal measures its length. The method uses constant extra [space complexity](theoretical-computer-science.md#space-complexity) and time proportional to the preperiod plus cycle length.

## Rotating calipers

↑ **Parent:** [Algorithm](algorithm.md)

A family of algorithms that exploit monotonically changing geometric directions while traversing sorted points or the boundary of a [convex polygon](convex-set.md#convex-polygon). For example, after sorting rays by [polar angle](multivariable-calculus.md#polar-angle) around a point, a second index can advance monotonically to identify all rays lying in each open half-plane. Collinear rays require consistent boundary handling.

## Meet-in-the-middle algorithm

↑ **Parent:** [Algorithm](algorithm.md)

An [algorithm](algorithm.md) that splits choices into two groups, enumerates partial results for each group, and matches compatible results. For $n$ binary choices, the two lists each have about $2^{n/2}$ entries instead of enumerating $2^n$ complete choices; the matching cost and memory requirements depend on the problem.

## Maximum subarray problem

↑ **Parent:** [Algorithm](algorithm.md)

Given a finite sequence of [real numbers](arithmetic.md#real-number), find a nonempty contiguous block with maximum sum. Its restriction to contiguous blocks distinguishes it from choosing an arbitrary [subset](set.md#subset). The problem admits a linear-time solution using [Kadane's algorithm](#kadane-s-algorithm).

### Maximum-subarray segment summary

↑ **Parent:** [Maximum subarray problem](#maximum-subarray-problem)

For a segment, store its total sum $S$, maximum possibly-empty prefix sum $P$, maximum possibly-empty suffix sum $Q$ and maximum possibly-empty internal contiguous sum $B$. Adjacent segment summaries combine by

$$
(S,P,Q,B)=\left(S_L+S_R,\ \max(P_L,S_L+P_R),\ \max(Q_R,S_R+Q_L),\ \max(B_L,B_R,Q_L+P_R)\right).
$$

A prefix either stays on the left or includes the whole left segment and a right prefix. A suffix has the symmetric decomposition. An internal segment either stays in one child or crosses the boundary as a left suffix followed by a right prefix. These cases prove the formulas, including empty candidates. Store the corresponding endpoints to recover a winning segment. This constant-size summary gives a [linear time](theoretical-computer-science.md#linear-time) [divide-and-conquer algorithm](#divide-and-conquer-algorithm) for the empty-allowed [maximum subarray problem](#maximum-subarray-problem).

<h3 id="kadane-s-algorithm">Kadane's algorithm</h3>

↑ **Parent:** [Maximum subarray problem](#maximum-subarray-problem)

For input $a_1,\ldots,a_n$, let $E_i$ be the largest sum of a nonempty contiguous block ending at $i$. The [recurrence relation](sequence-and-series.md#recurrence-relation) $E_1=a_1$ and $E_i=\max(a_i,E_{i-1}+a_i)$ is exact: an optimal block either starts at $i$ or extends an optimal block ending at $i-1$. The answer is $\max_i E_i$. Keeping only the current $E_i$ and best value gives linear [time complexity](theoretical-computer-science.md#time-complexity) and constant extra [space complexity](theoretical-computer-science.md#space-complexity).

## Search algorithm

↑ **Parent:** [Algorithm](algorithm.md)

### Iterative lengthening search

↑ **Parent:** [Search algorithm](#search-algorithm)

[Iterative lengthening search](#iterative-lengthening-search) repeatedly runs [cost-bounded depth-first search](#cost-bounded-depth-first-search), starting with threshold zero and replacing each unsuccessful threshold by the smallest rejected [path cost](theoretical-computer-science.md#path-cost). It uses a [depth-first search](#depth-first-search) stack rather than the potentially large [search frontier](theoretical-computer-science.md#search-frontier) of [uniform-cost search](graph.md#uniform-cost-search).

Suppose an optimal [plan](artificial-intelligence.md#plan) has cost $C^*$ and each pass terminates. At every unsuccessful threshold $L<C^*$, some first rejected prefix of an optimal [plan](artificial-intelligence.md#plan) has [path cost](theoretical-computer-science.md#path-cost) at most $C^*$. Therefore the next threshold is no larger than $C^*$. Any first returned [goal state](theoretical-computer-science.md#goal-state) has cost at most $C^*$ and hence exactly $C^*$. Finite [branching factor](theoretical-computer-science.md#branching-factor) and a positive lower bound on [step costs](theoretical-computer-science.md#step-cost) ensure that only finitely many [search nodes](theoretical-computer-science.md#search-node) precede that cost, giving completeness as well as optimality. With arbitrary real [step costs](theoretical-computer-science.md#step-cost), the threshold increments can be much smaller than the smallest [step cost](theoretical-computer-science.md#step-cost): the difference between two [path costs](theoretical-computer-science.md#path-cost) need not itself be a [step cost](theoretical-computer-science.md#step-cost).

### Staircase matrix search

↑ **Parent:** [Search algorithm](#search-algorithm)

Search a matrix whose rows and columns are both nondecreasing by inspecting the top-right corner of the remaining rectangle. If that value is below the target, discard its row; if above, discard its column; if equal, return its coordinates. The [loop invariant](#loop-invariant) retains every possible match inside the rectangle. Each failure decreases its remaining height plus width by one, proving at most $n+m-1$ inspections for positive dimensions and constant [auxiliary space](#auxiliary-space). Row monotonicity alone is insufficient for the column exclusion.

### AND-OR search

↑ **Parent:** [Search algorithm](#search-algorithm)

A [search algorithm](#search-algorithm) whose OR nodes represent controllable choices and whose AND nodes require solutions for every possible outcome of a chosen action. In [nondeterministic planning](artificial-intelligence.md#nondeterministic-planning), a successful OR choice needs successful continuations for all its AND children. In [contingent planning](artificial-intelligence.md#contingent-planning), those children can represent different observations and updated [belief states](theoretical-computer-science.md#belief-state). Cycle handling must match the required solution concept: ignoring a repeated state is not a proof that the goal will inevitably be reached.

### Two-sum problem

↑ **Parent:** [Search algorithm](#search-algorithm)

Find two distinct input positions whose values sum to a target, or establish that no such pair exists. Distinct values are not required: two equal values may form a pair when they occur at different positions. On a [sorted array](data-structure.md#sorted-array), [distinct-index two-sum by suffix lower bounds](#distinct-index-two-sum-by-suffix-lower-bounds) gives $O(N\log N)$ [running time](#running-time), while a [two-pointer technique](#two-pointer-technique) can give linear time.

### Ternary lower-bound search

↑ **Parent:** [Search algorithm](#search-algorithm)

A [lower-bound search](#lower-bound-search) that probes two positions to retain one of three subintervals. For unresolved $[lo,hi)$ of positive length $d$, put $q=\lfloor d/3\rfloor$, $m_1=lo+q$ and $m_2=hi-1-q$. If $a(m_1)\geq x$, retain $[lo,m_1)$; if $a(m_2)<x$, retain $[m_2+1,hi)$; otherwise retain $[m_1+1,m_2)$. [Sortedness](#sortedness) preserves the lower-bound partition. The new interval lengths are $q,q,d-2q-2$, and the feasible middle case has nonnegative length at most $q$. This proves strict progress and $O(\log(N+1))$ comparison cost. Equality must retain the first possible boundary rather than return an arbitrary matching occurrence.

### Optimal search algorithm

↑ **Parent:** [Search algorithm](#search-algorithm)

A [search algorithm](#search-algorithm) is optimal for a specified objective if its returned solution has the best objective value among all solutions. The objective is part of the claim: minimizing the number of actions does not generally maximize a reward assigned to terminal states. [Breadth-first tree search](tree-graph-theory.md#breadth-first-tree-search) optimizes total cost when all actions have the same positive cost.

### Complete search algorithm

↑ **Parent:** [Search algorithm](#search-algorithm)

A [search algorithm](#search-algorithm) is complete for a specified class of problems if it finds a solution whenever a solution exists in that class. This definition need not require termination on unsolvable instances; an additional termination guarantee should be stated separately. A finite [branching factor](theoretical-computer-science.md#branching-factor) makes [breadth-first tree search](tree-graph-theory.md#breadth-first-tree-search) complete for finite-depth solutions, while [depth-first tree search](#depth-first-tree-search) additionally needs a reason it cannot be trapped on an infinite branch.

### Tree search

↑ **Parent:** [Search algorithm](#search-algorithm)

A [search algorithm](#search-algorithm) that explores action histories in a [search tree](theoretical-computer-science.md#search-tree). Two histories ending in the same state remain distinct nodes unless an additional repetition rule identifies them. Consequently a finite [state space](dynamical-systems.md#state-space) can generate an infinite [search tree](theoretical-computer-science.md#search-tree): a legal stay action at a nonterminal state already suffices. A [graph search](graph.md#graph-search) instead records explored states to control repetitions. Confusing these models changes termination and completeness claims.

## Backtracking

↑ **Parent:** [Algorithm](algorithm.md)

Build a candidate incrementally, abandoning a partial candidate as soon as no valid completion is possible. A [depth-first search](#depth-first-search) explores one choice, restores the previous state, and tries the next. Constraint propagation and bounds can greatly reduce the visited [state space](dynamical-systems.md#state-space), although the worst-case [time complexity](theoretical-computer-science.md#time-complexity) may remain exponential.

### Backtracking leaf bound

↑ **Parent:** [Backtracking](#backtracking)

Suppose [backtracking](#backtracking) assigns each of finitely many variables once along each branch, branching only on distinct values in its initial nonempty [constraint domain](theoretical-computer-science.md#constraint-domain) $D_i$. Then the number of leaves is at most $\prod_i|D_i|$, even if inconsistent partial assignments terminate early. Ignore constraints and associate a leaf with every full domain assignment extending its partial assignment. Each leaf has at least one such extension. Different leaves have disjoint extension families: at their first diverging choice they assigned different values to the same selected variable. These nonempty disjoint families lie in a [Cartesian product](set-theory.md#cartesian-product) of [cardinality](cardinal-number.md#cardinality) $\prod_i|D_i|$, proving the bound. The selected next variable can depend on the preceding assignments, provided each full assignment follows a unique branch.

The bound is exact for an unpruned enumeration tree, but need not be attained when actual constraints cause [search pruning](#search-pruning). Counting complete satisfying assignments alone also does not count failed partial leaves.

## Sliding-window algorithm

↑ **Parent:** [Algorithm](algorithm.md)

An [algorithm](algorithm.md) that maintains information about a contiguous part of a [sequence](sequence-and-series.md#sequence) while moving its endpoints. Updating a fixed-length window [sum](arithmetic.md#sum) needs subtraction of the outgoing term and [addition](arithmetic.md#addition) of the incoming term. A window [product](arithmetic.md#product-of-numbers) can be updated by [division](arithmetic.md#division-mathematics) only when the outgoing factor is nonzero; zero counts or zero-free segments handle that exception.

## Brute-force search

↑ **Parent:** [Algorithm](algorithm.md)

A search [algorithm](algorithm.md) that tests candidates directly, without exploiting enough structure to avoid their enumeration. A small brute-force implementation is often useful for checking an optimized [algorithm](algorithm.md) independently.

## Search pruning

↑ **Parent:** [Algorithm](algorithm.md)

Discarding a branch of a [search tree](theoretical-computer-science.md#search-tree) after proving that no completion can satisfy the constraints or improve the current best solution. For minimization, a [lower bound](set.md#lower-bound-in-a-partially-ordered-set) on every completion justifies pruning when it is at least the best value already found; this is the principle behind [branch and bound](mathematical-optimization.md#branch-and-bound).

## Number-theoretic sieve

↑ **Parent:** [Algorithm](algorithm.md)

A number-theoretic sieve processes many [integers](integer.md) together by marking or updating those sharing a [divisor](divisibility.md#divisor), rather than testing each [integer](integer.md) independently. The [sieve of Eratosthenes](prime-number.md#sieve-of-eratosthenes) marks composite multiples of successive [prime numbers](prime-number.md); related sieves accumulate a [smallest prime factor](prime-number.md#smallest-prime-factor), [Euler's totient function](number-theory.md#euler-totient-function), or [Möbius function](arithmetic-function.md#mobius-function) for every argument up to a bound. The useful structure is that the multiples of a fixed [integer](integer.md) form an [arithmetic progression](arithmetic.md#arithmetic-progression), so one loop can update all affected entries in an array.

For example, initializing an array to true and then marking $2p,3p,\ldots$ for each surviving [prime number](prime-number.md) $p$ leaves precisely the [prime numbers](prime-number.md) unmarked, apart from the separately excluded zero and one. Every [composite number](number-theory.md#composite-number) has a [prime factor](prime-number.md#prime-factor), which proves that every composite is eventually removed. Starting the marking at $p^2$ avoids work already performed by smaller [prime numbers](prime-number.md). Different sieves use different update rules and [time complexity](theoretical-computer-science.md#time-complexity) bounds; the name alone does not imply the complexity of the [sieve of Eratosthenes](prime-number.md#sieve-of-eratosthenes).

### Odd-only sieve

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

An odd-only sieve stores only odd candidates, handling the [prime](prime-number.md) two separately. This reduces the candidate storage and avoids marking even composites repeatedly.

### Totient sieve

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

A totient sieve computes the [Euler totient function](number-theory.md#euler-totient-function) for many integers at once. Initialize $\phi(n)=n$ and, for each [prime](prime-number.md) $p$, replace $\phi(n)$ by $\phi(n)(1-1/p)$ for every multiple $n$ of $p$.

### Smallest prime factor sieve

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

### Prime sieve

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

A [number-theoretic sieve](#number-theoretic-sieve) used to enumerate [prime numbers](prime-number.md) by excluding [composite numbers](number-theory.md#composite-number). The [sieve of Eratosthenes](prime-number.md#sieve-of-eratosthenes) marks multiples of each discovered prime, beginning at its square.

### Wheel factorization

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

Choose a modulus $W$ that is a product of small [primes](prime-number.md). Every [prime](prime-number.md) not dividing $W$ must be [coprime](divisibility.md#coprime-integers) to $W$, so a search can restrict candidates to the corresponding [residue classes](modular-arithmetic.md#residue-class) modulo $W$. For several [linear polynomials](polynomial.md#linear-polynomial), discard each [residue class](modular-arithmetic.md#residue-class) in which any required value is divisible by a selected [prime](prime-number.md). The surviving [residue classes](modular-arithmetic.md#residue-class) can be combined using the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem).

#### Wheel modulus

↑ **Parent:** [Wheel factorization](#wheel-factorization)

### Du Jiao sieve

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

A Du Jiao sieve computes a summatory [arithmetic function](arithmetic-function.md) using a [Dirichlet convolution](arithmetic-function.md#dirichlet-convolution) identity and [memoization](#memoization) of repeated quotient arguments. For the [Mertens function](arithmetic-function.md#mertens-function) $M(n)=\sum_{k\le n}\mu(k)$, the identity $\sum_{d\mid k}\mu(d)=[k=1]$ gives $M(n)=1-\sum_{i=2}^n M(\lfloor n/i\rfloor)$. Grouping equal quotients and precomputing small arguments makes this [recurrence relation](sequence-and-series.md#recurrence-relation) useful for large inputs.

<h3 id="min-25-sieve">Min_25 sieve</h3>

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

A family of [algorithms](algorithm.md) for summatory [multiplicative functions](arithmetic-function.md#multiplicative-function) that first computes suitable sums over [primes](prime-number.md) at quotient values and then incorporates [prime powers](prime-number.md#prime-power). The required prime-sum formulas and complexity depend on the particular [multiplicative function](arithmetic-function.md#multiplicative-function).

### Segmented sieve

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

A [number-theoretic sieve](#number-theoretic-sieve) that processes a large search range in smaller [intervals](real-analysis.md#interval-mathematics). To find [primes](prime-number.md) in $[L,H]$, first generate the [primes](prime-number.md) at most $\sqrt H$, then mark their multiples in the current segment. Memory for the segment depends on its width rather than on $H$.

#### Odd-only segmented sieve

↑ **Parent:** [Segmented sieve](#segmented-sieve)

### Linear sieve

↑ **Parent:** [Number-theoretic sieve](#number-theoretic-sieve)

A [number-theoretic sieve](#number-theoretic-sieve) that visits each [composite number](number-theory.md#composite-number) exactly once, through its [smallest prime factor](prime-number.md#smallest-prime-factor). Keep a growing list of [prime numbers](prime-number.md); for each $i$, generate $ip$ only for stored primes $p\le\operatorname{spf}(i)$. Each composite $m$ has a unique representation $m=\operatorname{spf}(m)(m/\operatorname{spf}(m))$ admitted by this rule, giving $O(N)$ arithmetic updates up to $N$.

## Matrix-chain multiplication

↑ **Parent:** [Algorithm](algorithm.md)

Given a fixed [sequence](sequence-and-series.md#sequence) of compatible [matrices](vector-space.md#matrix) $A_1,\ldots,A_m$, choose a binary parenthesization of $A_1\cdots A_m$ that minimizes the number of scalar multiplications in ordinary [matrix multiplication](vector-space.md#matrix-multiplication). The order of the [matrices](vector-space.md#matrix) is fixed: parenthesization changes the grouping, not the operand order. [Associativity](algebraic-operation.md#associative-property) preserves the product while intermediate [matrix](vector-space.md#matrix) dimensions change the cost. The possible binary groupings are counted by the [Catalan number](combinatorics.md#catalan-number) $C_{m-1}$ for $m\geq1$.

### Matrix-chain cost model

↑ **Parent:** [Matrix-chain multiplication](#matrix-chain-multiplication)

For [matrix dimensions](vector-space.md#matrix-dimensions) $r\times s$ and $s\times t$, ordinary [matrix multiplication](vector-space.md#matrix-multiplication) computes $rt$ [matrix entries](vector-space.md#matrix-entry), each using $s$ [scalar multiplications](vector-space.md#scalar-multiplication). Thus its cost is $rst$ [scalar multiplications](vector-space.md#scalar-multiplication), with $rt(s-1)$ [additions](arithmetic.md#addition) if each sum starts from its first term. Here we minimize only the [scalar multiplication](vector-space.md#scalar-multiplication) count, using this dense [matrix multiplication](vector-space.md#matrix-multiplication) rule throughout. The counts describe [arithmetic operations](numerical-analysis.md#arithmetic-operation), rather than measured elapsed time; [matrix multiplication](vector-space.md#matrix-multiplication) methods that exploit structure or use faster formulas require a different cost rule.

Take [matrices](vector-space.md#matrix) $A$, $B$, $C$ with [matrix dimensions](vector-space.md#matrix-dimensions) $12\times5$, $5\times40$, $40\times3$. Both groupings produce a $12\times3$ [matrix product](vector-space.md#matrix-product), but their intermediate [matrix dimensions](vector-space.md#matrix-dimensions) differ:

$$
\begin{aligned}
(AB)C &: \quad 12\cdot5\cdot40+12\cdot40\cdot3=2400+1440=3840,\\
A(BC) &: \quad 5\cdot40\cdot3+12\cdot5\cdot3=600+180=780.
\end{aligned}
$$

The second grouping first compresses $BC$ into a $5\times3$ [matrix](vector-space.md#matrix), avoiding the $12\times40$ intermediate [matrix](vector-space.md#matrix) $AB$. The saving is $3060$ [scalar multiplications](vector-space.md#scalar-multiplication), although both groupings use exactly two [matrix multiplications](vector-space.md#matrix-multiplication). This is why counting only [matrix multiplication](vector-space.md#matrix-multiplication) operations hides the interesting choice.

<a id="image-the-same-matrix-product-can-require-3840-or-780-scalar-multiplications"></a>
![](matrix-chain-parenthesization-cost-trees.png)

**[Figure 1](#image-the-same-matrix-product-can-require-3840-or-780-scalar-multiplications). The same matrix product can require 3840 or 780 scalar multiplications**. Original [binary trees](data-structure.md#binary-tree) for the three-[matrix](vector-space.md#matrix) example. Leaves keep $A,B,C$ in the same order. Each internal node gives its resulting [matrix dimensions](vector-space.md#matrix-dimensions) and the local [scalar multiplication](vector-space.md#scalar-multiplication) cost; adding those costs gives the total.

[Associativity](algebraic-operation.md#associative-property) permits these regroupings in exact arithmetic; [commutativity](algebraic-operation.md#commutativity) is neither assumed nor generally true for [matrix multiplication](vector-space.md#matrix-multiplication). Swapping $A$ and $B$ here would even make their [matrix product](vector-space.md#matrix-product) undefined. In [floating-point arithmetic](floating-point-arithmetic.md), [round-off error](numerical-analysis.md#round-off-error) can make the two groupings yield different computed [matrix entries](vector-space.md#matrix-entry); the cost optimum alone does not guarantee the smallest numerical error.

### Matrix-chain dynamic programming

↑ **Parent:** [Matrix-chain multiplication](#matrix-chain-multiplication)

Let $A_i$ have [matrix dimensions](vector-space.md#matrix-dimensions) $p_{i-1}\times p_i$, where $p_0,\ldots,p_n$ are positive [integers](integer.md). For $1\leq i\leq j\leq n$, define $m[i,j]$ as the minimum [scalar multiplication](vector-space.md#scalar-multiplication) cost of the contiguous [matrix product](vector-space.md#matrix-product) $A_i\cdots A_j$. The endpoints $(i,j)$ of an [integer interval](integer.md#integer-interval) identify a [dynamic programming state](mathematical-optimization.md#dynamic-programming-state). A single [matrix](vector-space.md#matrix) needs no [matrix multiplication](vector-space.md#matrix-multiplication), giving the [base case](#base-case) $m[i,i]=0$. At the final [matrix multiplication](vector-space.md#matrix-multiplication), split after $A_k$:

$$
m[i,j]=\min_{i\leq k<j}\bigl(m[i,k]+m[k+1,j]+p_{i-1}p_kp_j\bigr),\qquad i<j.
$$

The two subproducts have [matrix dimensions](vector-space.md#matrix-dimensions) $p_{i-1}\times p_k$ and $p_k\times p_j$, regardless of their internal grouping. The [recurrence relation](sequence-and-series.md#recurrence-relation) adds their optimal costs and the final [scalar multiplication](vector-space.md#scalar-multiplication) cost.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; Lecture 21: Dynamic Programming III, printed p. 2, Parenthesization: final split, recurrence and zero one-matrix base case; notes use half-open indices](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-21-dynamic-programming-iii)

Why is this [optimal substructure](mathematical-optimization.md#optimal-substructure)? For a chosen final split $k$, replacing either subproduct's grouping by a cheaper one leaves its [matrix dimensions](vector-space.md#matrix-dimensions) and exact [matrix product](vector-space.md#matrix-product) unchanged, so it decreases the whole cost by the same amount. Therefore an optimal grouping can use optimal groupings on both sides. Conversely, each candidate in the [recurrence relation](sequence-and-series.md#recurrence-relation) joins two achievable groupings. [Mathematical induction](foundations-of-mathematics.md#mathematical-induction) on $j-i+1$, starting with the single-[matrix](vector-space.md#matrix) [base case](#base-case), proves that the minimum is achievable and no grouping is cheaper.

There are also [overlapping subproblems](#overlapping-subproblems): while evaluating the different final splits of $ABCD$, the cases $A(BCD)$ and $(ABC)D$ both request the cost of $BC$. [Recursion](#recursion-computer-science) without reuse recomputes this answer; [memoization](#memoization) or a [dynamic programming](mathematical-optimization.md#dynamic-programming) table stores it once. Fill the table by increasing length $j-i+1$, so both dependencies are ready. Record an attaining split $s[i,j]$ alongside each cost.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; Lecture 21: Dynamic Programming III, printed p. 2, Parenthesization: increasing substring size, cubic time and parent pointers](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-21-dynamic-programming-iii)

The [dynamic programming](mathematical-optimization.md#dynamic-programming) table has $n(n+1)/2$ cost entries. For length $\ell$, there are $n-\ell+1$ entries and $\ell-1$ possible splits, so the exact number of candidate evaluations is

$$
\sum_{\ell=2}^{n}(n-\ell+1)(\ell-1)=\frac{n(n-1)(n+1)}{6}.
$$

Under the unit-cost assumption that [arithmetic operations](numerical-analysis.md#arithmetic-operation), comparisons and access to stored costs each take constant time, this gives [time complexity](theoretical-computer-science.md#time-complexity) $O(n^3)$ and [space complexity](theoretical-computer-science.md#space-complexity) $O(n^2)$, using [Big O notation](real-analysis.md#big-o-notation). These bounds concern choosing a grouping from the [matrix dimensions](vector-space.md#matrix-dimensions); they exclude the subsequent [matrix multiplication](vector-space.md#matrix-multiplication) work. If the dimensions or costs require arbitrarily long [integers](integer.md), their arithmetic and storage costs must also be counted.

### Matrix-chain split reconstruction

↑ **Parent:** [Matrix-chain multiplication](#matrix-chain-multiplication)

Extend the original example by a [matrix](vector-space.md#matrix) $D$ with [matrix dimensions](vector-space.md#matrix-dimensions) $3\times15$, so $(p_0,p_1,p_2,p_3,p_4)=(12,5,40,3,15)$. The [Catalan number](combinatorics.md#catalan-number) $C_3=5$ counts all possible groupings. Their [scalar multiplication](vector-space.md#scalar-multiplication) costs are

$$
\begin{array}{c|r}
\text{grouping}&\text{cost}\\\hline
((AB)C)D&2400+1440+540=4380\\
(A(BC))D&600+180+540=1320\\
(AB)(CD)&2400+1800+7200=11400\\
A((BC)D)&600+225+900=1725\\
A(B(CD))&1800+3000+900=5700
\end{array}
$$

The optimum is $(A(BC))D$, with cost $1320$. Enumeration makes a useful check here, but [dynamic programming](mathematical-optimization.md#dynamic-programming) reaches the same answer by solving ten [integer intervals](integer.md#integer-interval), including the four single-[matrix](vector-space.md#matrix) [base cases](#base-case):

$$
\begin{array}{c|rrrr}
i\backslash j&1&2&3&4\\\hline
1&0&2400&780&1320\\
2&&0&600&825\\
3&&&0&1800\\
4&&&&0
\end{array}
$$

For example, $m[2,4]=\min\{1800+5\cdot40\cdot15,\ 600+5\cdot3\cdot15\}=\min\{4800,825\}=825$. The three final-split candidates for the full [matrix product](vector-space.md#matrix-product) supply a compact certificate:

$$
\begin{aligned}
k=1 &: \quad 0+825+12\cdot5\cdot15=1725,\\
k=2 &: \quad 2400+1800+12\cdot40\cdot15=11400,\\
k=3 &: \quad 780+0+12\cdot3\cdot15=1320.
\end{aligned}
$$

The first candidate already uses the better grouping of $BCD$; the worse $A(B(CD))$ need not be reconsidered at the top level. This is how [optimal substructure](mathematical-optimization.md#optimal-substructure) lets the table represent all five possibilities with only three final candidates.

<a id="image-a-four-matrix-cost-table-and-the-splits-certifying-the-optimum"></a>
![](matrix-chain-dynamic-programming-certificate.png)

**[Figure 2](#image-a-four-matrix-cost-table-and-the-splits-certifying-the-optimum). A four-matrix cost table and the splits certifying the optimum**. Original [dynamic programming](mathematical-optimization.md#dynamic-programming) calculation for $(12,5,40,3,15)$. Orange entries are the nonsingleton [integer intervals](integer.md#integer-interval) used in the recovered optimum. The [binary tree](data-structure.md#binary-tree) follows stored splits down both children to the single-[matrix](vector-space.md#matrix) [base cases](#base-case); the final candidates certify the cost $1320$.

Read $s[1,4]=3$, which separates $ABC$ from $D$. Then $s[1,3]=1$ separates $A$ from $BC$, and $s[2,3]=2$ separates $B$ from $C$. This [recursion](#recursion-computer-science) stops at every $i=j$, returning the corresponding [matrix](vector-space.md#matrix) name. Combining the returned expressions recovers $(A(BC))D$, rather than only its cost. Every [recursive call](#recursive-call) uses a shorter [integer interval](integer.md#integer-interval), establishing [algorithm termination](#algorithm-termination); a tied minimum may choose any attaining split. The recovered [binary tree](data-structure.md#binary-tree) has $n$ leaves and $n-1$ internal nodes, so reconstruction takes $O(n)$ steps. Its attraction is the separation between an enormous family of groupings and a small set of reusable [dynamic programming states](mathematical-optimization.md#dynamic-programming-state).

## Greedy algorithm

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Greedy_algorithm)

A [greedy algorithm](#greedy-algorithm) builds a [feasible solution](mathematical-optimization.md#feasible-point) by repeatedly committing to a locally preferred next choice. Each commitment is final: the [algorithm](algorithm.md) does not revisit it when later choices become available. In [mathematical optimization](mathematical-optimization.md), the important question is whether those commitments can still attain the best [objective function](mathematical-optimization.md#objective-function) value.

For example, a shared telescope can accept several observation requests with fixed time slots. In [interval scheduling](#interval-scheduling), every completed request counts equally, and overlapping requests cannot both be accepted. Choosing the request that finishes earliest leaves the resource available sooner. The example below turns that intuition into a precise rule, then shows why choosing the earliest start or shortest duration can lose jobs.

[Greedy algorithms](#greedy-algorithm) are attractive because a single pass can replace a search through many candidate [subsets](set.md#subset). However, "locally best" is only a design proposal. A problem-specific [greedy-choice property](#greedy-choice-property), often established by an [exchange argument](#exchange-argument), must connect the local decision to the actual [objective function](mathematical-optimization.md#objective-function). The largest-individual-value rule in the [0-1 knapsack problem](mathematical-optimization.md#0-1-knapsack-problem) fails; [Dijkstra's algorithm](shortest-path-problem.md#dijkstra-algorithm) needs its nonnegative-edge assumptions. A rule's success in one [optimization](mathematical-optimization.md) task does not justify it in another.

### Interval stabbing problem

↑ **Parent:** [Greedy algorithm](#greedy-algorithm)

Given finitely many nonempty [closed intervals](real-analysis.md#closed-real-interval) $[s_i,e_i]$, choose as few points as possible so that each interval contains a chosen point. An optimal [greedy algorithm](#greedy-algorithm) repeatedly chooses the smallest end of an uncovered interval. After choosing $t$, any still uncovered interval starts strictly after $t$, since its end cannot be smaller than $t$. Thus the intervals whose ends trigger successive choices are pairwise disjoint. Every feasible point set needs a separate point in each triggering interval, proving that the greedy point set is optimal. Sorting by end and scanning takes $O(n\log n)$ time. The inclusion of endpoints means an interval starting at the last chosen point is already covered.

### Counterexample to removing a longest increasing subsequence

↑ **Parent:** [Greedy algorithm](#greedy-algorithm)

Repeatedly removing a longest [strictly increasing subsequence](combinatorics.md#strictly-increasing-subsequence) need not minimise the number of increasing subsequences in a partition. In $(2,4,1,3)$, removing $(2,3)$ leaves the decreasing pair $(4,1)$, for three subsequences overall. The partition $(2,4)$ and $(1,3)$ uses only two and is optimal because the original sequence is not increasing.

### Greedy-choice property

↑ **Parent:** [Greedy algorithm](#greedy-algorithm)

A [greedy-choice property](#greedy-choice-property) says that some optimal [feasible solution](mathematical-optimization.md#feasible-point) contains the locally selected choice. Together with [optimal substructure](mathematical-optimization.md#optimal-substructure) in the remaining instance, it allows repeated commitments. An [exchange argument](#exchange-argument) often establishes this property.[Algorithms by Jeff Erickson; §4.3 General Pattern, printed pp. 164–165: exchange without worsening an optimum](computer-science-bibliography.md#algorithms-by-jeff-erickson/greedy-algorithms)

For [interval scheduling](#interval-scheduling), a safe first choice need not belong to every optimal [feasible solution](mathematical-optimization.md#feasible-point). When several optima exist, a commitment may exclude one while retaining another. The useful [loop invariant](#loop-invariant) is that the accepted prefix can still be extended to an optimum. Merely keeping the accepted [intervals](real-analysis.md#interval-mathematics) compatible proves feasibility, which is a weaker claim.

#### Exchange argument

↑ **Parent:** [Greedy-choice property](#greedy-choice-property)

An [exchange argument](#exchange-argument) modifies an optimal [feasible solution](mathematical-optimization.md#feasible-point) to include a desired choice while preserving feasibility and not worsening its [objective function](mathematical-optimization.md#objective-function) value. The modification need not strictly improve the optimum; equality suffices.[Algorithms by Jeff Erickson; §4.3 General Pattern, printed pp. 164–165: exchange at the first disagreement](computer-science-bibliography.md#algorithms-by-jeff-erickson/greedy-algorithms)

For [interval scheduling](#interval-scheduling), the exchange replaces the first selected job with an earliest-finishing job. Its safety comes from the finish-time inequality below. Replacing a job with a shorter one has no such guarantee: it might move the occupied [interval](real-analysis.md#interval-mathematics) into the middle of two useful jobs, as the [shortest-duration interval scheduling counterexample](#shortest-duration-interval-scheduling-counterexample) shows.

### Interval scheduling

↑ **Parent:** [Greedy algorithm](#greedy-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Interval_scheduling)

Given a [finite set](set.md#finite-set) of jobs with fixed half-open [intervals](real-analysis.md#interval-mathematics) $[s_i,f_i)$, where $s_i<f_i$, choose a [subset](set.md#subset) $S$ of [maximum](set.md#maximum-of-a-subset-of-a-total-order) [cardinality](cardinal-number.md#cardinality). Each job occupies one shared resource throughout its [interval](real-analysis.md#interval-mathematics). A [feasible solution](mathematical-optimization.md#feasible-point) has pairwise [disjoint](set.md#disjoint-sets) [intervals](real-analysis.md#interval-mathematics): for distinct selected jobs $i,j$, either $f_i\leq s_j$ or $f_j\leq s_i$. Thus a finish and the next start may coincide. Every job has value one; occupied time is not the [objective function](mathematical-optimization.md#objective-function).[6.046J Design and Analysis of Algorithms, Spring 2015; Printed p. 2, Interval Scheduling: fixed requests, one resource, compatibility with endpoint equality, maximum size](computer-science-bibliography.md#6-046j-design-and-analysis-of-algorithms-spring-2015/lecture-1-introduction)

Consider these six original jobs, with arbitrary time units:

$$
\begin{array}{c|rrrrrr}
\text{job}&A&B&C&D&E&F\\\hline
s_i&0&1&3&5&6&8\\
f_i&6&3&5&7&9&10
\end{array}.
$$

Job $B=[1,3)$ can be followed immediately by $C=[3,5)$ and $D=[5,7)$. Job $A=[0,6)$ conflicts with all three. Starting the resource earlier is therefore not automatically beneficial: one long commitment can displace several shorter requests.

The earliest-finish [greedy algorithm](#greedy-algorithm) uses a [sorting algorithm](#sorting-algorithm) to put jobs in [nondecreasing](calculus.md#nondecreasing-function) finish time. Scan that order, accepting the first job and then each job whose start is at least the last accepted finish. Break finish-time ties arbitrarily; an empty [input](theoretical-computer-science.md#input-computer-science) returns the [empty set](set.md#empty-set). For these jobs, the order and decisions are

$$
\begin{array}{c|rrrrrr}
\text{finish order}&B&C&A&D&E&F\\\hline
\text{decision}&\text{take}&\text{take}&\text{skip}&\text{take}&\text{skip}&\text{take}
\end{array}.
$$

After $B,C$, job $A$ starts before the current finish five and is rejected. Accept $D$; then reject $E=[6,9)$ because six is before seven. Finally accept $F=[8,10)$. The result is $S=\{B,C,D,F\}$, with [cardinality](cardinal-number.md#cardinality) four. Leaving $[0,1)$ idle makes room for more jobs.

By contrast, the earliest-start rule scans $A,B,C,D,E,F$. It accepts $A$, skips $B,C,D$, accepts $E$, and skips $F$. Its [feasible solution](mathematical-optimization.md#feasible-point) $\{A,E\}$ contains only two jobs. Here $A$ and $E$ meet at time six and are compatible; $E$ and $F$ overlap on $[8,9)$.

<a id="image-earliest-finish-accepts-four-jobs-earliest-start-accepts-two"></a>
![](interval-scheduling-six-jobs-finish-versus-start.png)

**[Figure 3](#image-earliest-finish-accepts-four-jobs-earliest-start-accepts-two). Earliest finish accepts four jobs; earliest start accepts two**. The same six original [intervals](real-analysis.md#interval-mathematics) appear in both panels. Colored jobs are accepted and gray jobs rejected. A filled start and hollow finish depict a half-open [interval](real-analysis.md#interval-mathematics); jobs meeting at an endpoint are compatible.

There is also an elementary optimality certificate for this example. The four [subsets](set.md#subset) $\{A,B\}$, $\{C\}$, $\{D,E\}$ and $\{F\}$ form a [partition of a set](set.md#partition-of-a-set) of the jobs. A [feasible solution](mathematical-optimization.md#feasible-point) takes at most one job from each group: $A,B$ overlap, as do $D,E$, and each other group is a [singleton](set.md#singleton-mathematics). Hence four is an [upper bound](set.md#upper-bound-in-a-partially-ordered-set), attained by $\{B,C,D,F\}$. Checking all $2^6=64$ [subsets](set.md#subset) gives a unique optimum of size four: $\{B,C,D,F\}$.

The earliest-finish theorem states that this [greedy algorithm](#greedy-algorithm) maximizes job count for every finite instance of [interval scheduling](#interval-scheduling). For the [exchange argument](#exchange-argument), let $q$ be the first job in an optimal [feasible solution](mathematical-optimization.md#feasible-point) and $g$ an earliest-finishing job. Every later selected job $j$ satisfies

$$
f_g\leq f_q\leq s_j.
$$

Replace $q$ by $g$; compatibility and [cardinality](cardinal-number.md#cardinality) survive. The remainder must be optimal among jobs starting at or after $f_g$, or improving it would improve the whole selection. [Mathematical induction](foundations-of-mathematics.md#mathematical-induction) on the smaller remaining instance, starting with the [empty set](set.md#empty-set), completes the outline.[Algorithms by Jeff Erickson; §4.2 Scheduling Classes, Lemma 4.3 and Theorem 4.4, printed pp. 163–164; endpoint equality is allowed by our half-open convention](computer-science-bibliography.md#algorithms-by-jeff-erickson/greedy-algorithms)

Why is the [algorithm](algorithm.md) fast? Once sorted, each job is examined once, using only the last accepted finish to decide compatibility. The scan takes $O(n)$ time; comparison [sorting algorithms](#sorting-algorithm) give total [time complexity](theoretical-computer-science.md#time-complexity) $O(n\log n)$ for $n\geq2$, in [Big O notation](real-analysis.md#big-o-notation), assuming constant-cost endpoint comparisons. Already sorted [input](theoretical-computer-science.md#input-computer-science) needs only the $O(n)$ scan.[6.046J Design and Analysis of Algorithms, Spring 2015; Printed pp. 2–4, earliest-finish rule, compatibility and first-job exchange; scan cost follows by counting one comparison per subsequent request](computer-science-bibliography.md#6-046j-design-and-analysis-of-algorithms-spring-2015/lecture-1-introduction)

The reason the shortcut is correct is stronger than "finishing sooner looks good": the [exchange argument](#exchange-argument) preserves every later job of a suitable optimum. This is the problem-specific fact that permits final decisions without exploring all [subsets](set.md#subset).

#### Shortest-duration interval scheduling counterexample

↑ **Parent:** [Interval scheduling](#interval-scheduling)

In this separate three-job example, labels $A,B,C$ denote new jobs:

$$
A=[0,5),\qquad B=[5,10),\qquad C=[4,6).
$$

Their durations are five, five and two. Consider the rule "accept a shortest remaining job, discard all jobs conflicting with it, and repeat". It selects $C$ first. But $C$ overlaps $A$ on $[4,5)$ and $B$ on $[5,6)$, so both are discarded. The rule returns one job, while the compatible [subset](set.md#subset) $\{A,B\}$ contains two. The common endpoint five is allowed, and no [feasible solution](mathematical-optimization.md#feasible-point) contains all three jobs, so two is the [maximum](set.md#maximum-of-a-subset-of-a-total-order).

<a id="image-a-two-unit-job-blocks-two-compatible-five-unit-jobs"></a>
![](interval-scheduling-shortest-duration-trap.png)

**[Figure 4](#image-a-two-unit-job-blocks-two-compatible-five-unit-jobs). A two-unit job blocks two compatible five-unit jobs**. A separate three-job [counterexample](foundations-of-mathematics.md#counterexample) to choosing shortest duration. The left panel accepts only $C=[4,6)$; the right panel accepts $A=[0,5)$ and $B=[5,10)$. Shaded bands mark the two positive-length overlaps with $C$.

Duration alone ignores where a job sits. Here the shortest job straddles the useful handover time. Earliest finish instead chooses $A$, then $B$, and attains two. A [counterexample](foundations-of-mathematics.md#counterexample) can refute a proposed [greedy-choice property](#greedy-choice-property) even when the rule succeeds on many other [inputs](theoretical-computer-science.md#input-computer-science).

#### Weighted interval scheduling

↑ **Parent:** [Interval scheduling](#interval-scheduling)

[Weighted interval scheduling](#weighted-interval-scheduling) assigns each job a reward $w_i$ and maximizes their sum over compatible jobs. Earliest finish can fail for this different [objective function](mathematical-optimization.md#objective-function); [dynamic programming](mathematical-optimization.md#dynamic-programming) can compare alternatives.[6.046J Design and Analysis of Algorithms, Spring 2015; Printed pp. 4–5, Weighted Interval Scheduling and Dynamic Programming](computer-science-bibliography.md#6-046j-design-and-analysis-of-algorithms-spring-2015/lecture-1-introduction)

For a separate two-job example, let $X=[0,2)$ have reward one and $Y=[1,3)$ reward ten. Earliest finish accepts $X$ and rejects $Y$, earning one; the optimum accepts $Y$, earning ten. Replacing $Y$ by $X$ preserves job count but loses reward. Thus the [interval scheduling](#interval-scheduling) [exchange argument](#exchange-argument) proves the unit-value theorem only: its preserved quantity must match the intended [objective function](mathematical-optimization.md#objective-function).

## Algorithm correctness

↑ **Parent:** [Algorithm](algorithm.md)

[Partial correctness](#partial-correctness) means that, if the [algorithm](algorithm.md) terminates on a permitted [input](theoretical-computer-science.md#input-computer-science), its [output](theoretical-computer-science.md#output-computing) meets the [formal specification](#formal-specification). [Total correctness](#total-correctness) additionally requires [algorithm termination](#algorithm-termination) on every permitted [input](theoretical-computer-science.md#input-computer-science).

A [precondition](#precondition) $P$ describes permitted starting circumstances; a [postcondition](#postcondition) $Q$ describes the required result. [Partial correctness](#partial-correctness) says that starting with $P$ and finishing implies $Q$. [Total correctness](#total-correctness) also guarantees finishing. A [loop invariant](#loop-invariant) supplies the connection between these conditions during repeated steps.[CS 2112 Fall 2019; Loop invariants, Using loop invariants to show code is correct: Establishment, Preservation, Postcondition, and Termination](computer-science-bibliography.md#cs-2112-fall-2019/loop-invariants)

Correctness is relative to a [formal specification](#formal-specification). Returning the first entry of an [array](data-structure.md#array-data-structure) correctly implements "return the first entry", but fails "return the [maximum](set.md#maximum-of-a-subset-of-a-total-order)" on $[3,1,4,4,2]$. A fast wrong answer does not acquire [algorithm correctness](#algorithm-correctness) from its [time complexity](theoretical-computer-science.md#time-complexity). Numerical closeness matters only when the [formal specification](#formal-specification) allows an approximation. [Software testing](computer-science.md#software-testing) and [test coverage](computer-science.md#test-coverage) provide evidence about selected executions; they do not by themselves establish [algorithm correctness](#algorithm-correctness) for every permitted [input](theoretical-computer-science.md#input-computer-science).

### Recursion invariant

↑ **Parent:** [Algorithm correctness](#algorithm-correctness)

A relationship between a recursive procedure's arguments, accumulated state and original input that holds at every reachable [recursive call](#recursive-call). For accumulator-based [exponentiation by squaring](number-theory.md#exponentiation-by-squaring), $acc\,base^{remaining}=x^n$ is a [recursion invariant](#recursion-invariant) under exact arithmetic. The base case converts it into the desired result, while the recursive step and a decreasing argument justify preservation and termination.

### Partial correctness

↑ **Parent:** [Algorithm correctness](#algorithm-correctness)

[Partial correctness](#partial-correctness) means that every terminating execution begun in a [program state](programming-language.md#program-state) satisfying the [precondition](#precondition) $P$ finishes in a [program state](programming-language.md#program-state) satisfying the [postcondition](#postcondition) $Q$. For a sequential program $C$, the usual [Hoare triple](programming-language.md#hoare-triple) notation is

$$
\{P\}\ C\ \{Q\}.
$$

Here the notation expresses [partial correctness](#partial-correctness); it makes no promise that $C$ finishes. The [precondition](#precondition) and [postcondition](#postcondition) describe permitted starting circumstances and required final circumstances, rather than tests performed automatically by the program.[Hoare, 1969, §3 Program Execution, p. 577, and §4 General Reservations, pp. 578–579; the paper instead labels the precondition P, program Q and result R](computer-science-bibliography.md#an-axiomatic-basis-for-computer-programming-by-tony-hoare)

For a sharp example, take the [precondition](#precondition) $n=4$ and the following sequential program over mathematical [integers](integer.md):
```
i = 0
s = 0
while i < n:
    i = i
```
The condition remains true, so execution never reaches the instruction after the loop. Consequently its [partial correctness](#partial-correctness) claim holds for the [postcondition](#postcondition) $2s=n(n+1)$, and even for the impossible [postcondition](#postcondition) $0=1$: there is no terminating execution with a wrong final result. This is [vacuous truth](mathematical-logic.md#vacuous-truth), not evidence that the loop computes a [sum](arithmetic.md#sum). The same program fails [total correctness](#total-correctness) for this permitted [input](theoretical-computer-science.md#input-computer-science).

The distinction is useful in a proof: first show that an answer, whenever produced, is right; then establish [algorithm termination](#algorithm-termination). The [summation loop verification](#summation-loop-verification) supplies both arguments for a loop that actually progresses. Its finite trace illustrates one execution, while its [loop invariant](#loop-invariant) covers every permitted [input](theoretical-computer-science.md#input-computer-science).

### Total correctness

↑ **Parent:** [Algorithm correctness](#algorithm-correctness)

[Total correctness](#total-correctness) requires [partial correctness](#partial-correctness) and [algorithm termination](#algorithm-termination) for every [program state](programming-language.md#program-state) allowed by the [precondition](#precondition). For a deterministic sequential program, every permitted start must reach a final [program state](programming-language.md#program-state) satisfying the [postcondition](#postcondition) after finitely many steps. Thus an infinite execution can satisfy [partial correctness](#partial-correctness), but refutes [total correctness](#total-correctness) for a permitted start.

In the [summation loop verification](#summation-loop-verification), the [loop invariant](#loop-invariant) establishes the answer conditional on exit, and the [loop variant](#loop-variant) establishes exit. Both parts matter: replacing the body by a step that never returns would defeat [total correctness](#total-correctness) even if every completed iteration preserved the [loop invariant](#loop-invariant). Likewise, a terminating loop with the wrong [sum](arithmetic.md#sum) fails [partial correctness](#partial-correctness) and therefore fails [total correctness](#total-correctness).

These obligations depend on the [formal specification](#formal-specification). A program that rejects every [input](theoretical-computer-science.md#input-computer-science) might correctly implement a rejection service, but does not meet a contract promising a [sum](arithmetic.md#sum) for every nonnegative [integer](integer.md). A proof of [total correctness](#total-correctness) also gives no particular physical response-time guarantee: [time complexity](theoretical-computer-science.md#time-complexity) and the execution environment require their own assumptions.

#### Algorithm termination

↑ **Parent:** [Total correctness](#total-correctness)

[Algorithm termination](#algorithm-termination) means that execution finishes after finitely many steps on the [inputs](theoretical-computer-science.md#input-computer-science) under consideration. Specify that domain: the stalled loop in [partial correctness](#partial-correctness) terminates for $n=0$ but runs forever for $n=4$. A successful run on one [input](theoretical-computer-science.md#input-computer-science) does not establish termination on another.

A useful method is a [loop variant](#loop-variant) $V$ that is a nonnegative [integer](integer.md) at every condition check and strictly decreases whenever the condition is true and the body completes. Also prove that condition evaluation and each body execution terminate. An infinite run would then give an infinite strictly decreasing [sequence](sequence-and-series.md#sequence) of nonnegative [integers](integer.md), contradicting their [well-founded relation](set-theory.md#well-founded-relation). This establishes [algorithm termination](#algorithm-termination) without enumerating all executions.

For the [summation loop verification](#summation-loop-verification), $V=n-i$ begins at $n$ and decreases by exactly one per iteration. The body executes exactly $n$ times, including zero times for $n=0$. Merely bounding a decreasing measure below is insufficient for [real numbers](arithmetic.md#real-number): $1,1/2,1/4,\ldots$ decreases forever while staying positive. The choice of a [well-founded relation](set-theory.md#well-founded-relation) supplies the essential progress argument; [well-founded progress in recursion](#well-founded-progress-in-recursion) applies the same idea to [recursive calls](#recursive-call).

### Prefix maximum correctness example

↑ **Parent:** [Algorithm correctness](#algorithm-correctness)

Given a nonempty finite [sequence](sequence-and-series.md#sequence) $a=(a_0,\ldots,a_{n-1})$ of [integers](integer.md), return its [maximum](set.md#maximum-of-a-subset-of-a-total-order) value. Represent the [sequence](sequence-and-series.md#sequence) by an [array](data-structure.md#array-data-structure) whose contents remain unchanged during execution. The [precondition](#precondition) requires an [integer](integer.md) length $n\geq1$ and exact, terminating [integer](integer.md) comparisons and [variable assignments](programming-language.md#variable-assignment). The [postcondition](#postcondition) for returned value $r$ is

$$
r\in\{a_i:0\leq i<n\}\quad\text{and}\quad a_i\leq r\ \text{for every }0\leq i<n.
$$

Thus the [output](theoretical-computer-science.md#output-computing) belongs to the [finite set](set.md#finite-set) of entries and is at least every entry. The contract permits ties and negative [integers](integer.md); it asks for a value, not the position of a particular occurrence. There is no [maximum](set.md#maximum-of-a-subset-of-a-total-order) of an empty [set](set.md) of [integers](integer.md), so empty [input](theoretical-computer-science.md#input-computer-science) is deliberately outside this [precondition](#precondition). A service accepting empty [inputs](theoretical-computer-science.md#input-computer-science) needs a different [formal specification](#formal-specification), such as a separate absent result.

This [Python](programming-language.md#python-programming-language) implementation makes the [variable assignments](programming-language.md#variable-assignment) explicit. Its index arithmetic models exact [integer](integer.md) arithmetic; fixed-width implementations additionally need enough index range for $n$:
```
def find_max(a):
    n = len(a)
    best = a[0]
    k = 1
    while k < n:
        if a[k] > best:
            best = a[k]
        k = k + 1
    return best
```
For the original [input](theoretical-computer-science.md#input-computer-science) $[3,1,4,4,2]$, initialization gives $k=1$ and $\mathrm{best}=3$. Reading $a_1=1$ keeps $3$; reading $a_2=4$ changes it to $4$; reading $a_3=4$ and $a_4=2$ keeps $4$. At successive condition checks, the pairs $(k,\mathrm{best})$ are $(1,3),(2,3),(3,4),(4,4),(5,4)$. The returned [maximum](set.md#maximum-of-a-subset-of-a-total-order) is $4$.

<a id="image-maximum-values-of-successive-prefixes-in-the-original-integer-array"></a>
![](prefix-maximum-invariant-trace.png)

**[Figure 5](#image-maximum-values-of-successive-prefixes-in-the-original-integer-array). Maximum values of successive prefixes in the original integer array**. Each row shows the processed prefix of $[3,1,4,4,2]$ immediately before checking $k<n$. Blue cells have been processed; grey cells have not. The [loop invariant](#loop-invariant) records the [maximum](set.md#maximum-of-a-subset-of-a-total-order) of the blue entries, while the [loop variant](#loop-variant) $n-k$ counts remaining entries. These are exact constructed execution states.

At each condition check, use the [loop invariant](#loop-invariant)

$$
I:\qquad 1\leq k\leq n,\qquad \mathrm{best}=\max\{a_i:0\leq i<k\},
$$

together with the fact that the [input](theoretical-computer-science.md#input-computer-science) [array](data-structure.md#array-data-structure) is unchanged. The prefix is the first $k$ entries of the [sequence](sequence-and-series.md#sequence), so its [finite set](set.md#finite-set) of values is nonempty. The [maximum](set.md#maximum-of-a-subset-of-a-total-order) need not be unique as an occurrence: the invariant concerns its value.

Initialization establishes $I$: $k=1$ and $\mathrm{best}=a_0$, the [maximum](set.md#maximum-of-a-subset-of-a-total-order) of a one-element [set](set.md). For preservation, suppose $I$ and $k<n$ hold. Then $a_k$ is a valid [array](data-structure.md#array-data-structure) entry. Either the comparison replaces $\mathrm{best}$ with the larger value $a_k$, or it keeps a value at least $a_k$. Before increasing $k$, the resulting value is

$$
\max\bigl(\max\{a_i:0\leq i<k\},a_k\bigr)=\max\{a_i:0\leq i<k+1\}.
$$

The [variable assignment](programming-language.md#variable-assignment) $k\gets k+1$ restores the complete [loop invariant](#loop-invariant). Between the two [variable assignments](programming-language.md#variable-assignment), the old prefix formula may temporarily be false; the [loop invariant](#loop-invariant) is required at condition checks, not at every instruction.

At exit, $k\geq n$, while $I$ gives $k\leq n$. Hence $k=n$, and $I$ gives exactly the required [postcondition](#postcondition). This establishes [partial correctness](#partial-correctness). The preservation argument is [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on the number of completed iterations, covering every permitted [integer](integer.md) [sequence](sequence-and-series.md#sequence), rather than just the pictured [input](theoretical-computer-science.md#input-computer-science).

For [algorithm termination](#algorithm-termination), the [loop variant](#loop-variant) $V=n-k$ is a nonnegative [integer](integer.md) whenever $I$ holds. If $k<n$, then $V\geq1$. Every body terminates under the [precondition](#precondition) and changes $V$ to $V-1$. Starting at $n-1$, it reaches zero after exactly $n-1$ iterations. For $n=1$, the initial value is already zero and the body is never entered. Together with [partial correctness](#partial-correctness), this proves [total correctness](#total-correctness).

Starting $\mathrm{best}$ at zero instead of $a_0$ fails on the original negative [input](theoretical-computer-science.md#input-computer-science) $[-7,-3,-3,-8]$: it returns zero, which is neither an entry nor the [maximum](set.md#maximum-of-a-subset-of-a-total-order) $-3$. Keeping $k=1$ forever preserves the correct initial prefix claim but loops forever when $n>1$; a [loop invariant](#loop-invariant) alone does not ensure [algorithm termination](#algorithm-termination). Using `>=` instead of `>` still returns the same [maximum](set.md#maximum-of-a-subset-of-a-total-order) value when entries tie, although a version returning a position would need an explicit tie rule.

### Formal verification

↑ **Parent:** [Algorithm correctness](#algorithm-correctness)

Establishing specified properties of a system using [formal proofs](mathematical-logic.md#formal-proof) about a precise model. [Formal verification](#formal-verification) connects an implementation to a [formal specification](#formal-specification); correctness of the model and its assumptions still matters when applying the result to a physical system.

For a small example, the [summation loop verification](#summation-loop-verification) below starts with executable steps and asks two separate questions: does any returned value satisfy the [postcondition](#postcondition), and does execution reach that return? A [loop invariant](#loop-invariant) answers the first; a [loop variant](#loop-variant) answers the second. This turns an unbounded family of permitted [inputs](theoretical-computer-science.md#input-computer-science) into a few reusable proof obligations.

The model must specify [programming language semantics](programming-language.md#programming-language-semantics), including the meaning of [variable assignments](programming-language.md#variable-assignment), comparisons and [integer arithmetic](arithmetic.md#integer-arithmetic). A proof about exact mathematical [integers](integer.md) need not describe a machine that wraps on [integer overflow](programming-language.md#integer-overflow). Similarly, a correct [formal proof](mathematical-logic.md#formal-proof) of a weak or mistaken [formal specification](#formal-specification) does not establish the intended behavior. Choosing the right [formal specification](#formal-specification) and relating the model to the implemented system remain substantive tasks.

[Software testing](computer-science.md#software-testing) examines chosen executions and can expose a [counterexample](foundations-of-mathematics.md#counterexample). A [formal proof](mathematical-logic.md#formal-proof) instead justifies a statement throughout its stated model; it does not require executing every permitted [input](theoretical-computer-science.md#input-computer-science). This makes [formal verification](#formal-verification) valuable when rare boundary cases matter, while [software testing](computer-science.md#software-testing) can still reveal an incorrect model or misunderstood requirement.

In 1969, [Tony Hoare](computer-science.md#tony-hoare) presented rules for [variable assignment](programming-language.md#variable-assignment), composition and iteration in a small [programming language](programming-language.md). His paper explicitly says those rules do not prove successful termination, and discusses the dependence of arithmetic reasoning on the chosen overflow behavior. These reservations already make the model's scope part of the argument.[Hoare, An Axiomatic Basis for Computer Programming, §2 Computer Arithmetic, pp. 576–577; §§3.1–3.4, pp. 577–578; §4 General Reservations, pp. 578–579](computer-science-bibliography.md#an-axiomatic-basis-for-computer-programming-by-tony-hoare)

#### Fairness assumption

↑ **Parent:** [Formal verification](#formal-verification)

A condition selecting admissible infinite [paths in a transition system](#path-in-a-transition-system), often to exclude executions that postpone an enabled activity forever. The notation $TS\models_{\mathrm{fair}}\varphi$ quantifies only over initial [paths in a transition system](#path-in-a-transition-system) satisfying the chosen condition. For example, $GFp$ requires $p$ infinitely often, while $FGp$ requires $p$ permanently from some point onwards. Neither condition implies the other.

#### Transition system

↑ **Parent:** [Formal verification](#formal-verification)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Transition_system)

A model consisting of a [set](set.md) $S$ of [states](theoretical-computer-science.md#state-computer-science), a [transition relation](#transition-relation) $\to\subseteq S\times S$, initial [states](theoretical-computer-science.md#state-computer-science) $I\subseteq S$, a [set](set.md) $AP$ of [atomic propositions](mathematical-logic.md#atomic-proposition), and a label [function](function.md) $L:S\to2^{AP}$ identifying which [atomic propositions](mathematical-logic.md#atomic-proposition) hold at each [state](theoretical-computer-science.md#state-computer-science). A [path in a transition system](#path-in-a-transition-system) follows permitted transitions. Some definitions omit labels or initial conditions; specify the convention used in each application.

##### Labelled transition system

↑ **Parent:** [Transition system](#transition-system)

A [transition system](#transition-system) whose edges carry action labels. A [CSP operational semantics](computer-science.md#csp-operational-semantics) uses visible [CSP events](computer-science.md#csp-event) and the internal label $\tau$.

##### Terminal state

↑ **Parent:** [Transition system](#transition-system)

A [state](theoretical-computer-science.md#state-computer-science) with no successor in the [transition relation](#transition-relation). Assuming no [terminal states](#terminal-state) makes every finite [path in a transition system](#path-in-a-transition-system) extendible and avoids choosing a separate convention for interpreting infinite-path [temporal logic](mathematical-logic.md#temporal-logic) at a dead end.

##### Path in a transition system

↑ **Parent:** [Transition system](#transition-system)

A finite or infinite [sequence](sequence-and-series.md#sequence) of [states](theoretical-computer-science.md#state-computer-science) in which $s_i\to s_{i+1}$ for each consecutive pair. In infinite-path [linear temporal logic](mathematical-logic.md#linear-temporal-logic) semantics, paths are infinite; an initial path must also start in the specified initial [set](set.md). Repeated [states](theoretical-computer-science.md#state-computer-science) are allowed, unlike conventions for a simple [path in a graph](graph-theory.md#path-in-a-graph).

###### Lasso path

↑ **Parent:** [Path in a transition system](#path-in-a-transition-system)

An infinite [path in a transition system](#path-in-a-transition-system) represented by a finite prefix followed by infinite repetition of a nonempty finite loop. If stored positions are $q_0,\ldots,q_k$ and $q_k\to q_\ell$, the represented [sequence](sequence-and-series.md#sequence) is $q_0\cdots q_{\ell-1}(q_\ell\cdots q_k)^\omega$. The [linear temporal logic](mathematical-logic.md#linear-temporal-logic) condition $GFp$ holds exactly when $p$ occurs on the repeated part, and $FGp$ holds exactly when $p$ holds everywhere on that part.

##### Transition relation

↑ **Parent:** [Transition system](#transition-system)

A [binary relation](set-theory.md#binary-relation) on the [states](theoretical-computer-science.md#state-computer-science) of a system, with $s\to t$ meaning that one permitted step changes $s$ to $t$. A [Boolean formula](theoretical-computer-science.md#boolean-formula) can encode a [transition relation](#transition-relation) after choosing bits for the current and next [states](theoretical-computer-science.md#state-computer-science).

#### Model checking

↑ **Parent:** [Formal verification](#formal-verification)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Model_checking)

##### Satisfaction set

↑ **Parent:** [Model checking](#model-checking)

For a [state](theoretical-computer-science.md#state-computer-science) formula $\varphi$ in a fixed labelled [transition system](#transition-system), its satisfaction set is $\{s\in S:s\models\varphi\}$. This is a [set](set.md) of [states](theoretical-computer-science.md#state-computer-science); it is distinct from the assertion that every initial [state](theoretical-computer-science.md#state-computer-science) satisfies the formula.

##### Bounded model checking

↑ **Parent:** [Model checking](#model-checking)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounded_model_checking)

A [formal verification](#formal-verification) method that encodes a bounded execution and a violated specification as a [Boolean satisfiability problem](theoretical-computer-science.md#boolean-satisfiability-problem). A [satisfying assignment](theoretical-computer-science.md#satisfying-assignment) yields a [counterexample](foundations-of-mathematics.md#counterexample). For infinite-path properties, a [lasso path](#lasso-path) can finitely represent a repeated execution. Failure to find a [counterexample](foundations-of-mathematics.md#counterexample) at one finite bound alone does not prove an unbounded property.[§§2–4, bounded encodings; §5, bounds](computer-science-bibliography.md#symbolic-model-checking-without-bdds-by-armin-biere-and-others)

#### Summation loop verification

↑ **Parent:** [Formal verification](#formal-verification)

Compute $1+2+\cdots+n$, the [triangular number](arithmetic.md#triangular-number) $T_n$, for a nonnegative [integer](integer.md) $n$. The [empty sum](arithmetic.md#empty-sum) gives zero when $n=0$. Use exact mathematical [integers](integer.md) and keep the [input](theoretical-computer-science.md#input-computer-science) $n$ unchanged; every comparison and [variable assignment](programming-language.md#variable-assignment) is a terminating operation. The original sequential procedure is
```
require n is an integer and n >= 0
i = 0
s = 0
while i < n:
    i = i + 1
    s = s + i
return s
```
The order of the two [variable assignments](programming-language.md#variable-assignment) matters: the [addition](arithmetic.md#addition) uses the newly incremented $i$. For $n=4$, the pairs $(i,s)$ at successive condition checks are $(0,0),(1,1),(2,3),(3,6),(4,10)$. At the last check, $i<n$ is false, and the returned [sum](arithmetic.md#sum) is $10$.

The [precondition](#precondition) is $n\in\mathbb Z$ with $n\geq0$, under the exact-arithmetic model just stated. The [postcondition](#postcondition) for returned value $s$ is $2s=n(n+1)$, with $n$ still equal to its starting value. At each condition check use the [loop invariant](#loop-invariant)

$$
I:\qquad i,s\in\mathbb Z,\qquad 0\leq i\leq n,\qquad 2s=i(i+1),
$$

and the [loop variant](#loop-variant) $V=n-i$. The equation says that the accumulator is the [triangular number](arithmetic.md#triangular-number) for precisely the processed prefix $1,\ldots,i$; the inequalities connect that prefix to the loop's condition.

<a id="image-the-summation-loop-restores-its-invariant-before-each-condition-check"></a>
![](summation-loop-contract-control-flow.png)

**[Figure 6](#image-the-summation-loop-restores-its-invariant-before-each-condition-check). The summation loop restores its invariant before each condition check**. Original sequential control flow for the [summation loop verification](#summation-loop-verification). The blue loop head carries the [loop invariant](#loop-invariant); the orange body increments $i$ before adding it to $s$. A false condition leads to the [postcondition](#postcondition). The [loop variant](#loop-variant) decreases on the return arrow. All values are mathematical [integers](integer.md) and $n$ remains unchanged.

Initialization gives $i=s=0$, so $I$ holds, including when $n=0$. For preservation, let the old values satisfy $I$ and $i<n$. Write $i'=i+1$ and $s'=s+i'$ for the values after both [variable assignments](programming-language.md#variable-assignment). Since $i,n$ are [integers](integer.md), $i<n$ gives $i'\leq n$, and

$$
2s'=2s+2(i+1)=i(i+1)+2(i+1)=(i+1)(i+2)=i'(i'+1).
$$

Thus the completed body restores $I$. Between the two [variable assignments](programming-language.md#variable-assignment), the equation can be false; the [loop invariant](#loop-invariant) is required at the loop head. This preservation step is [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on the number of completed iterations.

At exit, the false condition gives $i\geq n$, while $I$ gives $i\leq n$. Hence $i=n$, so $2s=n(n+1)$: this proves [partial correctness](#partial-correctness). For [algorithm termination](#algorithm-termination), $I$ gives the nonnegative [integer](integer.md) $V=n-i$. When the condition is true, $V\geq1$; the terminating body gives $V'=n-i'=V-1$. Therefore the loop cannot repeat forever. Together these arguments prove [total correctness](#total-correctness) for every permitted [input](theoretical-computer-science.md#input-computer-science), including $n=0$.

<a id="image-four-additions-finish-the-sum-an-unchanged-index-cannot-make-progress"></a>
![](summation-loop-trace-and-stalled-variant.png)

**[Figure 7](#image-four-additions-finish-the-sum-an-unchanged-index-cannot-make-progress). Four additions finish the sum; an unchanged index cannot make progress**. Original exact trace for $n=4$: five condition checks and four body executions give $s=10$, while the [loop variant](#loop-variant) decreases from four to zero. The right panel shows the stalled loop from [partial correctness](#partial-correctness): the same [program state](programming-language.md#program-state) repeats and $V=4$ never decreases. Its equation $2s=i(i+1)$ remains true, but it never reaches an exit.

Two changes expose what the proof checks. Swapping the two body instructions computes $0+1+\cdots+(n-1)$, returning $6$ rather than $10$ for $n=4$. Leaving $i$ unchanged can preserve an initial equation forever without producing any answer. The first change breaks the intended [postcondition](#postcondition); the second breaks [algorithm termination](#algorithm-termination). A trace can reveal these failures, while the two proof obligations explain them.

The exact-arithmetic assumption has a concrete boundary. In a stipulated unsigned eight-[bit](information-theory.md#bit) model where each [addition](arithmetic.md#addition) wraps modulo $256$, $n=23$ fits in the [input](theoretical-computer-science.md#input-computer-science) representation, but its intended [triangular number](arithmetic.md#triangular-number) is $276$. The stored accumulator instead finishes at $20$, so the mathematical [postcondition](#postcondition) fails. This is [integer overflow](programming-language.md#integer-overflow), and the proof above does not apply to that altered model. Restricting the same implementation to $0\leq n\leq22$ prevents overflow in its stored loop values, since $T_{22}=253$; alternatively use a representation supporting the required exact [integer arithmetic](arithmetic.md#integer-arithmetic). The equations in the proof are mathematical statements, not instructions to evaluate products in eight [bits](information-theory.md#bit).

#### Formal specification

↑ **Parent:** [Formal verification](#formal-verification)

A mathematically precise description of permitted behaviour. A [formal specification](#formal-specification) for the [microkernel file-read example](operating-system.md#microkernel-file-read-example)'s service could relate an authorized request to the exact returned [bytes](computer-memory.md#byte); a [formal specification](#formal-specification) of its [microkernel](operating-system.md#microkernel)'s [IPC](operating-system.md#inter-process-communication) need only describe the protected transport operation. They state different obligations.

For the [summation loop verification](#summation-loop-verification), require a nonnegative [integer](integer.md) [input](theoretical-computer-science.md#input-computer-science) $n$ and a returned value $s$ satisfying $2s=n(n+1)$. The [formal specification](#formal-specification) describes what answer is acceptable without requiring this particular loop: another implementation may satisfy the same contract. State separately whether [partial correctness](#partial-correctness) or [total correctness](#total-correctness) is required. A [Hoare triple](programming-language.md#hoare-triple) packages the [precondition](#precondition), the program and the [postcondition](#postcondition); [Hoare logic](programming-language.md#hoare-logic) supplies rules for establishing such claims.

Precision alone does not ensure a useful requirement. The [postcondition](#postcondition) $s\geq0$ permits returning zero for every nonnegative [integer](integer.md) [input](theoretical-computer-science.md#input-computer-science); it does not specify the intended [triangular number](arithmetic.md#triangular-number). Conversely, an impossible [precondition](#precondition) permits no starts, making a universal correctness claim vacuous. Check both that intended [inputs](theoretical-computer-science.md#input-computer-science) are admitted and that admitted [outputs](theoretical-computer-science.md#output-computing) express the intended task.

##### Constructive specification

↑ **Parent:** [Formal specification](#formal-specification)

Specify behavior by constructing a mathematical model and defining the operations on that model. Finite sequences model a [FIFO queue](data-structure.md#fifo-queue): insertion appends, the head is the first element, and successful deletion removes it. An [axiomatic specification](#axiomatic-specification) can then be checked against the model without requiring the implementation to use that representation.

##### Axiomatic specification

↑ **Parent:** [Formal specification](#formal-specification)

Describe operations through laws relating their observable results, without selecting an internal representation. For an [abstract data type](computer-science.md#abstract-data-type), the laws must state the operation domains and error results as well as ordinary cases. A [disjoint union](set-theory.md#disjoint-union) can distinguish a successful value from an error with the same textual spelling.

##### Frame condition

↑ **Parent:** [Formal specification](#formal-specification)

A clause stating which parts of a [program state](programming-language.md#program-state) an operation preserves. A query's returned value alone does not prohibit it from also mutating the receiver; a binary update's result equation alone does not preserve its distinct operand. Explicit [frame conditions](#frame-condition) rule out these behaviors and make substitution and composition arguments possible.

##### Planning safety certificate

↑ **Parent:** [Formal specification](#formal-specification)

An auxiliary [planning fluent](artificial-intelligence.md#planning-fluent) certifying that a safety condition has been checked for the current state in [automated planning](artificial-intelligence.md#automated-planning). A checking action requires facts establishing the condition and adds the certificate; the hazardous action requires that certificate.

Every action capable of invalidating the check must delete the certificate. Otherwise checking a safe configuration and then changing it could authorize an unsafe action using stale evidence. For river crossing, certify that the departure bank contains no incompatible pair, invalidate the certificate on every load, unload or crossing, and require it before sailing. This compiles a safety test into positive [STRIPS](artificial-intelligence.md#strips) [preconditions](#precondition) when a suitable finite static compatibility relation is supplied.

##### Planning state invariant

↑ **Parent:** [Formal specification](#formal-specification)

A property true initially and preserved by every applicable action in an [automated planning](artificial-intelligence.md#automated-planning) model. [Mathematical induction](foundations-of-mathematics.md#mathematical-induction) on the plan length then proves it for every reachable state. Typical examples are unique object locations, a capacity bound, and exactly one occupancy marker being true. An invariant is a consequence to prove from the action rules; merely declaring the intended capacity in prose does not enforce it.

##### Precondition

↑ **Parent:** [Formal specification](#formal-specification)

The condition required of a starting [program state](programming-language.md#program-state) for a stated correctness guarantee. In the [summation loop verification](#summation-loop-verification), $n\in\mathbb Z$ and $n\geq0$ admit $n=0$ and $n=4$, but exclude $n=-1$. The accompanying model assumes exact [integer arithmetic](arithmetic.md#integer-arithmetic) and terminating elementary operations. The initial values of $i,s$ need no restriction because initialization overwrites them before use.

A [precondition](#precondition) is a logical assumption, not automatically an executable check. Writing `require` in a procedure states its contract; an implementation that checks or rejects invalid [inputs](theoretical-computer-science.md#input-computer-science) needs that behavior specified too. Weakening a [precondition](#precondition) admits more starts and therefore demands more proof: dropping $n\geq0$ here makes $n=-2$ a terminating [counterexample](foundations-of-mathematics.md#counterexample) to $2s=n(n+1)$, since initialization returns zero while $n(n+1)=2$.

##### Postcondition

↑ **Parent:** [Formal specification](#formal-specification)

The condition required of a final [program state](programming-language.md#program-state) when a program finishes under its [precondition](#precondition). The [summation loop verification](#summation-loop-verification) requires returned value $s$ to satisfy $2s=n(n+1)$ and preserves the [input](theoretical-computer-science.md#input-computer-science) $n$. Relating the answer to the original [input](theoretical-computer-science.md#input-computer-science) matters: allowing the program to replace $n$ by zero would change the intended contract.

A [postcondition](#postcondition) alone gives no promise of [algorithm termination](#algorithm-termination). It also need not specify a unique [output](theoretical-computer-science.md#output-computing): $s\geq0$ allows many answers, while the exact [triangular number](arithmetic.md#triangular-number) equation determines one [integer](integer.md) answer for each permitted $n$. Stronger [postconditions](#postcondition) express more obligations; proving only a weaker consequence cannot justify the stronger requirement.

#### Binary correctness

↑ **Parent:** [Formal verification](#formal-verification)

Conformance of compiled machine code to the behaviour of the code model used to justify it. [Binary correctness](#binary-correctness) can extend [formal verification](#formal-verification) across the compilation step; the result applies to the particular compiled artifact and its assumptions.

### Functional correctness

↑ **Parent:** [Algorithm correctness](#algorithm-correctness)

Conformance of an implementation's behaviour to its specified functional requirements. The exact obligations come from the [formal specification](#formal-specification): correct delivery of an [IPC](operating-system.md#inter-process-communication) payload and correct computation of a [file](file-system.md#computer-file) read are different requirements. Neither requirement by itself supplies a numerical response-time bound.

### Loop invariant

↑ **Parent:** [Algorithm correctness](#algorithm-correctness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Loop_invariant)

A statement true whenever execution reaches a chosen point in a loop, usually immediately before its condition is tested. Establish it initially, preserve it through each iteration, and combine it with the exit condition to establish [algorithm correctness](#algorithm-correctness). Termination needs a separate argument.[CS 2112 Fall 2019; Loop invariants, Using loop invariants to show code is correct: the three partial-correctness obligations and separate Termination step](computer-science-bibliography.md#cs-2112-fall-2019/loop-invariants)

Write $I$ for the [loop invariant](#loop-invariant), $B$ for the condition, $P$ for the [precondition](#precondition), and $Q$ for the [postcondition](#postcondition). Prove that initialization under $P$ establishes $I$, that a completed body starting with $I$ and $B$ restores $I$, and that $I$ with false $B$ implies $Q$.[CS 2112 Fall 2019; Loop invariants, Using loop invariants to show code is correct: Establishment, Preservation, and Postcondition](computer-science-bibliography.md#cs-2112-fall-2019/loop-invariants)

In the [prefix maximum correctness example](#prefix-maximum-correctness-example), the [loop invariant](#loop-invariant) remembers exactly the [maximum](set.md#maximum-of-a-subset-of-a-total-order) of the processed prefix and the valid index bounds. The weaker statement $\mathrm{best}\geq a_0$ survives every iteration, but does not imply the [postcondition](#postcondition): for $[3,1,4,4,2]$, the wrong value $3$ satisfies it. A useful [loop invariant](#loop-invariant) retains enough information to recover the answer when the condition becomes false.

#### Loop variant

↑ **Parent:** [Loop invariant](#loop-invariant)

A decreasing measure used to prove [algorithm termination](#algorithm-termination). A nonnegative [integer](integer.md) [loop variant](#loop-variant) must strictly decrease after every completed body whose condition was true; the body itself must terminate.[CS 2112 Fall 2019; Loop invariants, Using loop invariants to show code is correct: Termination and the decrementing function](computer-science-bibliography.md#cs-2112-fall-2019/loop-invariants)

The [prefix maximum correctness example](#prefix-maximum-correctness-example) uses $V=n-k$. It counts unread entries and is independent of whether the new entry changes the [maximum](set.md#maximum-of-a-subset-of-a-total-order). Ties therefore cannot stall progress: $k$ increases even when $\mathrm{best}$ stays the same. An [integer](integer.md) bounded below cannot strictly decrease indefinitely, which supplies the missing [algorithm termination](#algorithm-termination) argument.

<a id="image-control-flow-and-four-proof-obligations-for-the-prefix-maximum-correctness-example"></a>
![](prefix-maximum-proof-obligations.png)

**[Figure 8](#image-control-flow-and-four-proof-obligations-for-the-prefix-maximum-correctness-example). Control flow and four proof obligations for the prefix maximum correctness example**. Initialization, preservation, and exit establish [partial correctness](#partial-correctness); the [loop variant](#loop-variant) establishes [algorithm termination](#algorithm-termination) and hence [total correctness](#total-correctness). The [loop invariant](#loop-invariant) is restored after both [variable assignments](programming-language.md#variable-assignment). The [input](theoretical-computer-science.md#input-computer-science) [array](data-structure.md#array-data-structure) stays unchanged throughout.

Strict decrease and a lower bound are insufficient for arbitrary [real numbers](arithmetic.md#real-number). The positive [sequence](sequence-and-series.md#sequence) $1,1/2,1/4,\ldots$ strictly decreases and is bounded below by zero, but never reaches zero. Choosing an [integer](integer.md) measure avoids this failure.

## Linear search

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_search)

[Linear search](#linear-search), also called [sequential search](#linear-search), examines a finite [sequence](sequence-and-series.md#sequence) from its beginning, performing an [equality test](#equality-test) on each entry until one matches the target or the entries run out. It needs no [sorted array](data-structure.md#sorted-array) or [total order](set.md#total-order) on the values. This makes it useful for a small collection, a one-off lookup, or data available only in succession: the next entry is enough to make progress.

Specify the answer precisely. For an [array](data-structure.md#array-data-structure) $A$ of length $n\geq0$ with indices $0,\ldots,n-1$ and target $x$, return the smallest index $j$ satisfying $A_j=x$, or a distinct absent result if no such index exists. Repeated values are allowed. In this contract, finding a later duplicate is insufficient when an earlier match exists. Assume the [input](theoretical-computer-science.md#input-computer-science) remains unchanged during the search and each [equality test](#equality-test) terminates with a stable truth value expressing the intended matching relation.

Here is an implementation in [Python](programming-language.md#python-programming-language); `None` represents absence and is distinct from the valid index zero:
```
def linear_search(entries, target):
    for index, entry in enumerate(entries):
        if entry == target:
            return index
    return None
```
The official [Python](programming-language.md#python-programming-language) [sequence](sequence-and-series.md#sequence) method `s.index(x)` likewise specifies the first occurrence, but signals absence by raising `ValueError`. An API's absent-result convention belongs to its contract.[Python 3.14 documentation, Common Sequence Operations: s.index(x), first occurrence and ValueError](computer-science-bibliography.md#python-3-14-documentation/built-in-types-python-3-14-documentation)

Take the original unsorted [array](data-structure.md#array-data-structure) $A=[7,4,7,2,9]$. For $x=7$, the first [equality test](#equality-test) succeeds and returns index $0$; the other $7$ at index $2$ is never inspected. For $x=2$, the checks against $7,4,7$ fail, the check against $2$ succeeds, and the answer is index $3$ after four [equality tests](#equality-test). For absent target $x=6$, all five [equality tests](#equality-test) fail and the answer is `None`. On the empty [sequence](sequence-and-series.md#sequence), there is no entry to inspect: return `None` with zero [equality tests](#equality-test).

<a id="image-linear-search-on-an-unsorted-array-first-duplicate-later-match-and-absent-target"></a>
![](linear-search-unsorted-array-trace.png)

**[Figure 9](#image-linear-search-on-an-unsorted-array-first-duplicate-later-match-and-absent-target). Linear search on an unsorted array: first duplicate, later match, and absent target**. Indices start at zero. Each numbered cell is one [equality test](#equality-test); green cells match, orange cells fail, and grey cells are never inspected. The empty [sequence](sequence-and-series.md#sequence) requires zero [equality tests](#equality-test).

Value order never justifies skipping an entry in this [algorithm](algorithm.md). For $x=2$, stopping because the first value $7$ is larger would give a wrong absent result. Any [permutation](combinatorics.md#permutation) of the [input](theoretical-computer-science.md#input-computer-science) remains searchable by [linear search](#linear-search), although the first matching index and number of [equality tests](#equality-test) can change. By contrast, [binary search](#binary-search) uses a [total order](set.md#total-order) and the [sorted array](data-structure.md#sorted-array) property to discard whole candidate ranges. Its logarithmic [time complexity](theoretical-computer-science.md#time-complexity) additionally assumes cheap access to middle entries; a sorted [linked list](data-structure.md#linked-list) does not acquire constant-cost indexed access merely by being sorted. Sorting for a single query also has a cost, and changes positions relative to the original [sequence](sequence-and-series.md#sequence).

### Linear search comparison count

↑ **Parent:** [Linear search](#linear-search)

Count just the [equality tests](#equality-test) between the target and an entry, excluding loop conditions and index updates. If the first match is at index $j$, [linear search](#linear-search) uses exactly $C=j+1$ [equality tests](#equality-test). If the target is absent, it uses exactly $C=n$. Thus for $n\geq1$ the best successful case costs one [equality test](#equality-test), and the worst case costs $n$, attained by absence or a first match at the last index. For $n=0$, the sole outcome is absence with $C=0$.

<a id="image-linear-search-comparison-count-depends-on-the-first-matching-position"></a>
![](linear-search-position-comparison-count.png)

**[Figure 10](#image-linear-search-comparison-count-depends-on-the-first-matching-position). Linear search comparison count depends on the first matching position**. For length $n=8$, a first match at index $j$ costs $j+1$ [equality tests](#equality-test); absence costs eight. The dashed mean $4.5$ assumes a successful unique target uniformly located over the eight positions. It does not include absent queries.

An [expected value](expected-value.md) needs a specified [probability distribution](probability-distribution.md). For $n\geq1$, condition on success, assume the target occurs exactly once, and assume its position $J$ has a [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution) of indices $0,\ldots,n-1$. Then the [expected value](expected-value.md) of the [linear search comparison count](#linear-search-comparison-count) is

$$
\mathbb E[C\mid\text{success}]=\frac{1}{n}\sum_{j=0}^{n-1}(j+1)=\frac{n+1}{2}.
$$

This is the average of the costs $1,2,\ldots,n$ under those assumptions, with no assumption that the [array](data-structure.md#array-data-structure) is sorted. It is not a universal average for arbitrary queries. For example, with $n=5$, a unique successful target at index $0$ with [probability](probability-theory.md#probability) $3/4$ and at index $4$ with [probability](probability-theory.md#probability) $1/4$ has [expected value](expected-value.md) $(3/4)\cdot1+(1/4)\cdot5=2$, rather than $3$.

Duplicates also require care about what is sampled. Choose a position uniformly in $[7,4,7,2,9]$, then search for its value. All queries succeed, but the five possible sampled positions give costs $1,2,1,4,5$: both positions holding $7$ cause an immediate match at index $0$. The [expected value](expected-value.md) is $13/5$, not $(5+1)/2$. Uniformly choosing an occurrence does not uniformly locate the first match.

More generally, let the success [probability](probability-theory.md#probability) be $p>0$ and let $q_j$ be the conditional [probability](probability-theory.md#probability) that the first matching index is $j$, allowing duplicates. Since $\sum_{j=0}^{n-1}q_j=1$, the [expected value](expected-value.md) is

$$
\mathbb E[C]=p\sum_{j=0}^{n-1}(j+1)q_j+(1-p)n.
$$

Under the unique, uniformly located successful-target assumptions this becomes $p(n+1)/2+(1-p)n$. If every query is absent, $p=0$ and $C=n$ without needing conditional probabilities. When $n=0$, success is impossible and $C=0$; the successful-search conditional formula is undefined.

Converting the [linear search comparison count](#linear-search-comparison-count) to execution time needs a cost model. Under constant-cost [equality tests](#equality-test), next-entry access, and loop bookkeeping, worst-case [time complexity](theoretical-computer-science.md#time-complexity) is $O(n)$ in [Big O notation](real-analysis.md#big-o-notation) for $n\geq1$, with constant overhead even for the empty [sequence](sequence-and-series.md#sequence). Variable-length entries can make an [equality test](#equality-test) expensive. On a [linked list](data-structure.md#linked-list), advance along its links; repeatedly restarting at the head to obtain the next numeric index adds work that the comparison count does not capture. These are exact operation counts and conditional mathematical averages, not runtime measurements.

### Linear search correctness

↑ **Parent:** [Linear search](#linear-search)

The [loop invariant](#loop-invariant) just before inspecting index $i$ is: $0\leq i\leq n$, and no entry at an index $k<i$ matches $x$. Initially $i=0$, so there are no earlier entries. A failed [equality test](#equality-test) extends the excluded region by one position and preserves the [loop invariant](#loop-invariant). A successful [equality test](#equality-test) at index $i$ establishes a match; the [loop invariant](#loop-invariant) establishes that it is the first one. At exhaustion, $i=n$ and every entry has failed, so the absent result is correct. The number $n-i$ of remaining entries decreases after each failed [equality test](#equality-test), proving termination for a finite [sequence](sequence-and-series.md#sequence). Together these establish [algorithm correctness](#algorithm-correctness) under the assumptions that the [input](theoretical-computer-science.md#input-computer-science) is stable and each [equality test](#equality-test) terminates. No step of the argument compares the relative order of values.

## Equality test

↑ **Parent:** [Algorithm](algorithm.md)

A terminating check returning whether two values match under a specified relation. Mathematical equality is one such relation; a chosen [equivalence relation](set-theory.md#equivalence-relation) can instead express matching keys. [Linear search](#linear-search) only needs this check, whereas [binary search](#binary-search) also uses relative order. The cost of an [equality test](#equality-test) depends on the representation and implementation of its operands.

### Equality-only grouping lower bound

↑ **Parent:** [Equality test](#equality-test)

In the comparison model exposing only an [equality test](#equality-test) between otherwise opaque values, partitioning $n$ values into [equivalence classes](set-theory.md#equivalence-class) takes $\Omega(n^2)$ tests in the worst case. Run the algorithm on pairwise distinct values. If any pair remains untested, changing just those two values to equal is consistent with every answer observed so far but changes the required output partition. Every pair must therefore be tested. With a compatible [total order](set.md#total-order), [comparison sort](#comparison-sort) can instead group equal values in $O(n\log n)$ time.

## Strength reduction

↑ **Parent:** [Algorithm](algorithm.md)

Replace an operation by an equivalent operation sequence with lower cost on the target machine. For fixed-width wrapping integers, multiplication by eight equals left shift by three, and multiplication by fifteen equals left shift by four minus the original operand. Condition codes and wider results must also be preserved if the original machine instruction exposes them.

// Destination: computer-science.bigb

## Statistical program profiling

↑ **Parent:** [Algorithm](algorithm.md)

Periodically sample an executing program's [instruction pointer](computer-science.md#instruction-pointer) and accumulate an address histogram. Samples approximate time spent in address regions, rather than exact instruction execution counts. Jittering the sampling interval reduces accidental synchronization with periodic code.

// Destination: computer-science.bigb

## Depth-first search

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Depth-first_search)

[Depth-first search](#depth-first-search) is a [graph search](graph.md#graph-search) that follows a branch as far as it can before returning to try the next unexplored branch. Starting at a [vertex](graph.md#vertex-graph-theory) $s$ of an [undirected graph](graph-theory.md#undirected-graph) on a [finite set](set.md#finite-set) of [vertices](graph.md#vertex-graph-theory), mark $s$ as discovered. Scan its [graph neighbours](graph-theory.md#neighbour-of-a-vertex) in a fixed order: for each undiscovered [vertex](graph.md#vertex-graph-theory), record the current [vertex](graph.md#vertex-graph-theory) as its [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree) in the discovery [tree](tree-graph-theory.md), mark the new [vertex](graph.md#vertex-graph-theory), and explore it immediately using [recursion](#recursion-computer-science). Return when its [adjacency list](data-structure.md#adjacency-list) is exhausted. Discovery marks persist after return, preventing a [graph cycle](graph-theory.md#cycle-in-a-graph) from causing repeated exploration. This branch-and-return rule is the maze exploration described in MIT's notes. [MIT 6.006, lecture 14: depth-first search, pp. 2–3](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-14-graphs-ii-depth-first-search)

Use the same unweighted [undirected graph](graph-theory.md#undirected-graph) as [breadth-first search](tree-graph-theory.md#breadth-first-search), with [vertex set](graph.md#vertex-set) $V=\{A,B,C,D,E,F,G\}$ and [edges](graph-theory.md#edge-of-a-graph)

$$
E=\{AB,AC,BD,BE,CE,CF,EG,FG\},
$$

where $XY$ denotes the unordered pair $\{X,Y\}$. Visit [graph neighbours](graph-theory.md#neighbour-of-a-vertex) in [lexicographic order](extremal-set-theory.md#lexicographic-order) of their one-letter labels, starting at $A$. The discovery order, computed by the diagram's generator, is

$$
A,B,D,E,C,F,G.
$$

The discovery [edges](graph-theory.md#edge-of-a-graph) in order are $AB,BD,BE,EC,CF,FG$. They form a [rooted tree](tree-graph-theory.md#rooted-tree) spanning the reached [vertices](graph.md#vertex-graph-theory), with [root of a tree](tree-graph-theory.md#root-of-a-tree) $A$. The other [edges](graph-theory.md#edge-of-a-graph), $AC$ and $EG$, remain in the original [graph](graph.md) but never discover a new [vertex](graph.md#vertex-graph-theory). In particular, the [graph cycle](graph-theory.md#cycle-in-a-graph) $A,B,E,C,A$ causes no repeated discovery.

<a id="image-depth-first-search-discovery-edges-and-the-active-call-stack-on-seven-vertices"></a>
![](depth-first-search-stack.png)

**[Figure 11](#image-depth-first-search-discovery-edges-and-the-active-call-stack-on-seven-vertices). Depth-first search: discovery edges and the active call stack on seven vertices**. Numbers show first-discovery order. Solid [edges](graph-theory.md#edge-of-a-graph) form the discovery [tree](tree-graph-theory.md); dashed [edges](graph-theory.md#edge-of-a-graph) belong only to the original [graph](graph.md). The right panel shows the [call stack](data-structure.md#call-stack) from oldest call to current call, including the return from $D$ before entering $E$.

At $D$ there is no undiscovered [graph neighbour](graph-theory.md#neighbour-of-a-vertex), so its call returns to $B$. The next call enters $E$, then $C$, then $F$, then $G$. Immediately after discovering $G$, the [call stack](data-structure.md#call-stack) is $A,B,E,C,F,G$, with $G$ on top; $D$ is still discovered but its call has finished. The maximum [call stack](data-structure.md#call-stack) depth is six, although seven [vertices](graph.md#vertex-graph-theory) are discovered. Following the recorded [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree) backwards at each step reconstructs a [graph path](graph-theory.md#path-in-a-graph); here the route from $A$ to $G$ is $A,B,E,C,F,G$, using five [edges](graph-theory.md#edge-of-a-graph). [Breadth-first search](tree-graph-theory.md#breadth-first-search) instead finds $A,B,E,G$, using three [edges](graph-theory.md#edge-of-a-graph). [Depth-first search](#depth-first-search) establishes [reachability](graph.md#reachability-in-a-graph) but does not guarantee the fewest [edges](graph-theory.md#edge-of-a-graph).

An explicit [LIFO stack](data-structure.md#stack-data-structure) can replace [recursion](#recursion-computer-science), but its entries and discovery rule must be specified. To reproduce this exact traversal, store one frame per active [vertex](graph.md#vertex-graph-theory), retaining the next position in its [adjacency list](data-structure.md#adjacency-list). Advance the top frame by one [graph neighbour](graph-theory.md#neighbour-of-a-vertex); if that [vertex](graph.md#vertex-graph-theory) is undiscovered, mark it and push its frame immediately; pop an exhausted frame. Pushing all undiscovered [graph neighbours](graph-theory.md#neighbour-of-a-vertex) at once and marking them on push is a different iterative variant. Even pushing them in reverse [lexicographic order](extremal-set-theory.md#lexicographic-order) does not generally reproduce the [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree) relationships above: $C$ would already be marked while processing $A$, so $E$ could not discover $C$.

With an [adjacency list](data-structure.md#adjacency-list) representation, constant-cost discovery checks and frame operations, and the [graph neighbours](graph-theory.md#neighbour-of-a-vertex) already ordered, [depth-first search](#depth-first-search) has [time complexity](theoretical-computer-science.md#time-complexity) $O(|V|+|E|)$ in [Big O notation](real-analysis.md#big-o-notation). Each reached [vertex](graph.md#vertex-graph-theory) is entered once and each incident [edge](graph-theory.md#edge-of-a-graph) is examined at most twice in an [undirected graph](graph-theory.md#undirected-graph); initializing all discovery marks costs $O(|V|)$. The [call stack](data-structure.md#call-stack) has depth at most $|V|$, since no active [vertex](graph.md#vertex-graph-theory) repeats. Discovery marks and the recorded [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree) for each nonroot [vertex](graph.md#vertex-graph-theory) also need $O(|V|)$ auxiliary [space complexity](theoretical-computer-science.md#space-complexity), excluding storage for the [graph](graph.md). Sorting [adjacency lists](data-structure.md#adjacency-list) to obtain a chosen order is additional work. [Sedgewick and Wayne, Algorithms: DepthFirstPaths discovery marks and resource bounds](https://raw.githubusercontent.com/kevin-wayne/algs4/master/src/main/java/edu/princeton/cs/algs4/DepthFirstPaths.java)

One start explores only its [connected component of a graph](graph.md#component-graph-theory). To cover a disconnected [graph](graph.md), start again at every still-undiscovered [vertex](graph.md#vertex-graph-theory) while keeping all discovery marks; the discovery [trees](tree-graph-theory.md) form a [forest](tree-graph-theory.md#forest). [Depth-first search](#depth-first-search) is useful for [reachability](graph.md#reachability-in-a-graph), constructing a [spanning tree](tree-graph-theory.md#spanning-tree) of a [connected graph](graph.md#connected-graph), and organizing the return steps needed by a [depth-first traversal of a tree](tree-graph-theory.md#depth-first-traversal-of-a-tree). For detecting a [graph cycle](graph-theory.md#cycle-in-a-graph) in a [simple graph](graph.md#simple-graph) that is an [undirected graph](graph-theory.md#undirected-graph), an [edge](graph-theory.md#edge-of-a-graph) to an already discovered [vertex](graph.md#vertex-graph-theory) other than the current [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree) closes a [graph cycle](graph-theory.md#cycle-in-a-graph); the immediate return [edge](graph-theory.md#edge-of-a-graph) to that [parent in a rooted tree](tree-graph-theory.md#parent-in-a-rooted-tree) is not itself a [graph cycle](graph-theory.md#cycle-in-a-graph).

// Target: computer-science.bigb

### Depth-first search parenthesis property

↑ **Parent:** [Depth-first search](#depth-first-search)

The discovery-to-finishing intervals of distinct [vertices](graph.md#vertex-graph-theory) in a [depth-first search](#depth-first-search) are either disjoint or strictly nested. A recursive call completes before its caller returns; separate completed branches have disjoint intervals. Thus the displayed nesting holds exactly when $v$ is a proper [descendant in a rooted tree](tree-graph-theory.md#descendant-in-a-rooted-tree) of $u$ in the discovery [forest](tree-graph-theory.md#forest). A [directed path](graph-theory.md#directed-path) alone does not imply this nesting, because it can leave the current branch through an already discovered ancestor.

### Cost-bounded depth-first search

↑ **Parent:** [Depth-first search](#depth-first-search)

A [cost-bounded depth-first search](#cost-bounded-depth-first-search) follows the usual [depth-first search](#depth-first-search) order but immediately rejects a generated [search node](theoretical-computer-science.md#search-node) whose accumulated [path cost](theoretical-computer-science.md#path-cost) exceeds a threshold $L$. It can also return the least rejected [path cost](theoretical-computer-science.md#path-cost), providing the next threshold for [iterative lengthening search](#iterative-lengthening-search). Positive [step costs](theoretical-computer-science.md#step-cost) ensure that a rejected prefix cannot become a cheaper extension. With finite [branching factor](theoretical-computer-science.md#branching-factor) and every [step cost](theoretical-computer-science.md#step-cost)ing at least $\epsilon>0$, every admitted [search node](theoretical-computer-science.md#search-node) has [search depth](theoretical-computer-science.md#search-depth) at most $\lfloor L/\epsilon\rfloor$, so the pass terminates. Merely requiring every individual [step cost](theoretical-computer-science.md#step-cost) to be positive does not exclude an infinite branch of finite total [path cost](theoretical-computer-science.md#path-cost).

### Explicit-stack depth-first tree traversal

↑ **Parent:** [Depth-first search](#depth-first-search)

An [explicit-stack depth-first tree traversal](#explicit-stack-depth-first-tree-traversal) stores pending subtree roots instead of suspended recursive calls. In a [binary tree](data-structure.md#binary-tree), visit the current node, defer its nonempty right child on a [stack](data-structure.md#stack-data-structure), and continue with its left child; pop when the current subtree is empty. The unvisited subtrees remain disjoint and, together with the visited nodes, partition the original tree. This [loop invariant](#loop-invariant) proves that accumulating each visited label gives the tree sum. At most one right sibling per ancestor is pending, so auxiliary storage is $O(d)$ for depth $d$ and running time is $\Theta(N)$ for $N$ nodes. Unlike a full recursive [stack frame](data-structure.md#stack-frame), a pending entry need contain only a subtree [pointer](computer-memory.md#pointer-computer-programming).

### DFS edge classification

↑ **Parent:** [Depth-first search](#depth-first-search)

Classify [directed edges](graph-theory.md#directed-edge) relative to a [depth-first search](#depth-first-search) forest. Tree [edges](graph-theory.md#edge-of-a-graph) discover a new [vertex](graph.md#vertex-graph-theory); forward [edges](graph-theory.md#edge-of-a-graph) reach a proper descendant without being its discovery [edge](graph-theory.md#edge-of-a-graph); back [edges](graph-theory.md#edge-of-a-graph) reach an active ancestor; cross [edges](graph-theory.md#edge-of-a-graph) connect completed branches or trees. Discovery and finish intervals are nested for ancestry. The classification depends on the chosen search order, not only on the [graph](graph.md).

#### Cross edge in depth-first search

↑ **Parent:** [DFS edge classification](#dfs-edge-classification)

A [directed edge](graph-theory.md#directed-edge) whose endpoints have no ancestor-descendant relationship in the [depth-first search](#depth-first-search) forest. Their discovery-to-finishing intervals are disjoint by the [DFS parenthesis property](#depth-first-search-parenthesis-property). Such an edge can connect different completed branches or different search trees.

#### Tree edge in depth-first search

↑ **Parent:** [DFS edge classification](#dfs-edge-classification)

A [directed edge](graph-theory.md#directed-edge) whose examination first discovers its target and recursively enters it. It becomes the target's parent edge in the [depth-first search](#depth-first-search) forest.

#### Back edge in depth-first search

↑ **Parent:** [DFS edge classification](#dfs-edge-classification)

A [directed edge](graph-theory.md#directed-edge) from a [vertex](graph.md#vertex-graph-theory) to an active ancestor in its [depth-first search](#depth-first-search). Together with the tree path from that ancestor it witnesses a [directed cycle](graph-theory.md#directed-cycle).

#### Forward edge in depth-first search

↑ **Parent:** [DFS edge classification](#dfs-edge-classification)

A [directed edge](graph-theory.md#directed-edge) to a proper descendant in the [depth-first search](#depth-first-search) forest that is not a tree [edge](graph-theory.md#edge-of-a-graph). Its endpoints satisfy $d(u)<d(v)<f(v)<f(u)$.

### DFS discovery and finishing times

↑ **Parent:** [Depth-first search](#depth-first-search)

A traversal clock incremented on each vertex discovery and finish records two times per vertex. The active [recursion](#recursion-computer-science) interval of an ancestor contains that of each descendant. A finished vertex has no unexamined outgoing edge. These facts constrain possible finishing orders even when traversal order is unspecified.

### Depth-first tree search

↑ **Parent:** [Depth-first search](#depth-first-search)

The [tree search](#tree-search) version of [depth-first search](#depth-first-search) follows one action history until it ends, then returns to another choice. Repeated states do not automatically stop a branch. An infinite branch can prevent discovery of a goal on a different finite branch, so this method is not generally a [complete search algorithm](#complete-search-algorithm). A finite [search tree](theoretical-computer-science.md#search-tree) restores completeness, but the first successful history need not minimize cost or maximize a terminal reward.

### Iterative deepening depth-first search

↑ **Parent:** [Depth-first search](#depth-first-search)

Repeat a depth-limited [depth-first search](#depth-first-search) with successively larger depth limits. With unit-cost steps, the first successful depth is the minimum number of steps, provided each depth-limited search is complete. Each pass stores only the current path and its search bookkeeping.

## Memoization

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Memoization)

[Memoization](#memoization) retains a completed [function](function.md) result under a [memoization key](#memoization-key) and returns that result when an equivalent request recurs. For a terminating [pure function](programming-language.md#pure-function), repeated evaluation can therefore become lookup rather than repeated work. The benefit is especially striking with [recursion](#recursion-computer-science) and [overlapping subproblems](#overlapping-subproblems): a large [tree](tree-graph-theory.md) of calls can refer to a small [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) of distinct answers. The [memoization cache contract](#memoization-cache-contract) determines whether reuse is correct; the [memoization cache lifetime](#memoization-cache-lifetime) determines whether an answer is still present when wanted.

[Memoization](#memoization) records computed answers, whereas a [memory cache](computer-memory.md#cache-computing) retains data from [computer memory](computer-memory.md). A [CPU](computer-science.md#central-processing-unit) [cache hit](computer-memory.md#cache-hit) does not by itself prevent a program from evaluating the same [function](function.md) again. [Spreadsheet dependency evaluation](spreadsheet.md#spreadsheet-dependency-evaluation) adds an explicit mechanism for invalidating affected [cached cell values](spreadsheet.md#cached-cell-value) after inputs change; a general [memoization](#memoization) table does not discover such changes automatically.

A documented early motivation was to let programs improve their efficiency during execution through rote learning: the abstract of a 1968 paper explicitly proposes such a [programming language](programming-language.md) facility.[Donald Michie, “Memo” Functions and Machine Learning, Nature 218, pp. 19–22 (1968), abstract: programming-language rote learning motivated by efficiency during execution](computer-science-bibliography.md#“memo”-functions-and-machine-learning-by-donald-michie)

### Overlapping subproblems

↑ **Parent:** [Memoization](#memoization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Overlapping_subproblems)

[Overlapping subproblems](#overlapping-subproblems) occur when several parts of a calculation request the same smaller problem. [Memoization](#memoization) can share its answer if the [memoization key](#memoization-key) identifies that problem completely. For the [Fibonacci numbers](sequence-and-series.md#fibonacci-number), both $F_5$ and $F_4$ require $F_3$. In [dynamic programming](mathematical-optimization.md#dynamic-programming), the [dynamic programming state](mathematical-optimization.md#dynamic-programming-state) plays the corresponding role of identifying a reusable continuation. Overlap explains potential savings; the [recurrence relation](sequence-and-series.md#recurrence-relation) and its base cases still need to be correct.

### Memoized Fibonacci evaluation

↑ **Parent:** [Memoization](#memoization)

The [Fibonacci numbers](sequence-and-series.md#fibonacci-number) give an exact example. For a nonnegative [integer](integer.md) $n$, their [recurrence relation](sequence-and-series.md#recurrence-relation) is

$$
F_0=0,\qquad F_1=1,\qquad F_n=F_{n-1}+F_{n-2}\quad(n\geq2).
$$

To obtain $F_5=5$ by direct [recursion](#recursion-computer-science), evaluate $F_4$ and $F_3$ separately; computing $F_4$ also evaluates $F_3$. The full call [tree](tree-graph-theory.md) has 15 occurrences but just six distinct arguments, $0,1,2,3,4,5$. Shared dependencies form a [Directed acyclic graph](combinatorics.md#directed-acyclic-graph) because every [directed edge](graph-theory.md#directed-edge) goes to a strictly smaller argument. [Memoization](#memoization) evaluates a distinct argument on first demand; filling values in increasing argument order is the corresponding bottom-up [dynamic programming](mathematical-optimization.md#dynamic-programming) calculation.[MIT 6.006 Spring 2020, Lecture 15: Recursive Algorithms, printed pp. 2–3, Fibonacci Numbers and Re-using Subproblem Solutions](computer-science-bibliography.md#lecture-15-recursive-algorithms-6-006-spring-2020-by-massachusetts-institute-of-technology-6-006-course-staff)

<a id="image-repeated-calls-for-fibonacci-numbers-and-their-shared-directed-acyclic-graph-of-dependencies"></a>
![](memoization-fibonacci-recursion-and-dependencies.png)

**[Figure 12](#image-repeated-calls-for-fibonacci-numbers-and-their-shared-directed-acyclic-graph-of-dependencies). Repeated calls for Fibonacci numbers and their shared Directed acyclic graph of dependencies**. The call [tree](tree-graph-theory.md) contains 15 occurrences for $F_5$. The dependency [graph](graph.md) contains six distinct arguments and eight [directed edges](graph-theory.md#directed-edge). Equal labels have equal colors; arrows in the right panel point from a caller to the value it requires.

Use an initially empty [hash table](data-structure.md#hash-table) `memo`, shared by every recursive call. Count even the first evaluations of the two base cases, store only completed results, evaluate the left term first, and retain all entries. The following original procedure assumes a nonnegative [integer](integer.md) argument:

```
def cached_fib(n, memo):
    if n in memo:
        return memo[n]
    if n < 2:
        value = n
    else:
        value = cached_fib(n - 1, memo) + cached_fib(n - 2, memo)
    memo[n] = value
    return value
```

Every self-call must pass through the [memoization](#memoization) lookup. Wrapping only the outer call while leaving inner calls uncached retains the repeated work. Test membership rather than whether the stored value is nonzero: $F_0=0$ is a valid completed result.

For cold $F_5$, the lookup arguments are $5,4,3,2,1,0,1,2,3$. The first six are absent; the last three reuse completed answers. Results are stored on return in argument order $1,0,2,3,4,5$, with values $1,0,1,2,3,5$. Thus there are nine wrapper calls, six body evaluations and four [additions](arithmetic.md#addition). Repeating $F_5$ with the same table takes one wrapper call and no body evaluation. Requesting $F_6$ next evaluates only its body, reuses $F_5$ and $F_4$, and stores $F_6=8$: three wrapper calls, one body evaluation and two hits.

<a id="image-an-exact-memoization-lookup-trace-and-the-effect-of-retaining-or-clearing-its-table"></a>
![](memoization-cache-trace-and-lifetime.png)

**[Figure 13](#image-an-exact-memoization-lookup-trace-and-the-effect-of-retaining-or-clearing-its-table). An exact memoization lookup trace and the effect of retaining or clearing its table**. The first row records cold $F_5$ lookup order. The table records successive requests with one retained table; clearing it before the final request restores the cold counts. Calls include lookups that immediately return stored values; bodies count only first evaluations.

The direct-call count satisfies $C_0=C_1=1$ and $C_n=1+C_{n-1}+C_{n-2}$. Its exact solution is $C_n=2F_{n+1}-1$, as substitution into this [recurrence relation](sequence-and-series.md#recurrence-relation) verifies. With the specified [memoization](#memoization) procedure, a cold call at $n\geq2$ evaluates $n+1$ distinct bodies, makes $n-1$ [additions](arithmetic.md#addition) and makes $2n-1$ wrapper calls. There are $n-2$ hits: each of the $n-1$ nonbase bodies issues two recursive calls, in addition to the initial call. The difference is between the number of occurrences and the number of distinct subproblems.

### Memoization arithmetic and stack costs

↑ **Parent:** [Memoization](#memoization)

Under constant-cost lookup and [integer](integer.md) [addition](arithmetic.md#addition), [Memoized Fibonacci evaluation](#memoized-fibonacci-evaluation) has [time complexity](theoretical-computer-science.md#time-complexity) $O(n)$ in [Big O notation](real-analysis.md#big-o-notation), retaining $O(n)$ values. A [hash table](data-structure.md#hash-table) needs its own lookup-cost assumptions; an [array](data-structure.md#array-data-structure) indexed by $0,\ldots,n$ avoids [hash collisions](computer-science.md#hash-collision) in this example. [Memoization](#memoization) removes repeated bodies, but also pays for keys, lookups and retained answers. A workload without reuse can pay those costs without saving evaluations.

The [call stack](data-structure.md#call-stack) remains. Left-first [recursion](#recursion-computer-science) descends through arguments $n,n-1,\ldots,1$ before returning, giving $n$ simultaneously active frames for $n\geq2$. Therefore the auxiliary [space complexity](theoretical-computer-science.md#space-complexity) includes $O(n)$ frames as well as $O(n)$ table entries in the constant-size-value model. An iterative bottom-up [dynamic programming](mathematical-optimization.md#dynamic-programming) calculation removes these recursive frames; retaining only the two previous [Fibonacci numbers](sequence-and-series.md#fibonacci-number) suffices when only the final value is wanted, but discards the table useful for later requests.

Exact [Fibonacci numbers](sequence-and-series.md#fibonacci-number) do not remain constant-size values. For $k\geq2$, the [recurrence relation](sequence-and-series.md#recurrence-relation) gives $2^{(k-2)/2}\leq F_k\leq2^{k-1}$, so the representation of $F_k$ as a [binary number](arithmetic.md#binary-number) has order $k$ [bits](information-theory.md#bit). With ordinary [addition](arithmetic.md#addition) costing order $k$ [bit](information-theory.md#bit) operations on such operands, the $n-1$ [additions](arithmetic.md#addition) cost order $n^2$ [bit](information-theory.md#bit) operations in total. Retaining all values also requires order $n^2$ [bits](information-theory.md#bit) of value storage, before keys and frame overhead. The linear bound counts [additions](arithmetic.md#addition) under its stated cost model; it is not a linear bound on exact [integer arithmetic](arithmetic.md#integer-arithmetic) in [bits](information-theory.md#bit).[MIT 6.006 Spring 2020, Lecture 15: Recursive Algorithms, printed p. 3, final three bullets: growing Fibonacci bit lengths and addition cost](computer-science-bibliography.md#lecture-15-recursive-algorithms-6-006-spring-2020-by-massachusetts-institute-of-technology-6-006-course-staff)

### Memoization cache contract

↑ **Parent:** [Memoization](#memoization)

For a terminating [pure function](programming-language.md#pure-function), a reusable entry must record its correct completed result, and equal [memoization keys](#memoization-key) must imply equal results throughout the entry's [memoization cache lifetime](#memoization-cache-lifetime). Reusing that result must also preserve the behavior callers require. These conditions separate correctness from speed: a complete key can be correct even if it rarely repeats.

A procedure using [deterministic computation](theoretical-computer-science.md#deterministic-computation) can still have a required [side effect](programming-language.md#side-effect-computer-science). If a procedure returns $n^2$ and appends an audit record on every call, serving the second call from a table preserves the numerical answer but skips the second record. Likewise, if each call promises a fresh [mutable list](data-structure.md#mutable-list), returning the same stored [mutable list](data-structure.md#mutable-list) changes observable sharing and allows a caller to damage later answers. Plain result reuse is unsuitable for those contracts.[Python documentation, functools.lru\_cache: paragraph warning against functions with side effects, distinct mutable results, or impure time/random results](computer-science-bibliography.md#python-3-14-documentation/functools-higher-order-functions-and-operations-on-callable-objects-python-3-14-documentation)

Completion matters for [recursion](#recursion-computer-science). Suppose computing key $A$ needs key $B$, and computing $B$ needs $A$. A table containing only completed answers has no answer to return for the second $A$; remembering completed values does not make this [directed cycle](graph-theory.md#directed-cycle) terminate. Marking a key `ACTIVE` before descending detects re-entry, as in [spreadsheet dependency evaluation](spreadsheet.md#spreadsheet-dependency-evaluation), but detection is not a solution of the circular equations. If computation fails, clear its active mark and do not publish an unfinished value. The example using [Fibonacci numbers](sequence-and-series.md#fibonacci-number) avoids this issue through a strictly decreasing argument.

The call counts above assume sequential execution and no eviction. Concurrent requests for an absent key can both begin evaluation before either publishes its result; keeping a table coherent alone does not ensure one body execution per key.[Python documentation, functools.cache and functools.lru\_cache: thread-safe cache updates can still allow repeated evaluation before completion](computer-science-bibliography.md#python-3-14-documentation/functools-higher-order-functions-and-operations-on-callable-objects-python-3-14-documentation)

#### Memoization key

↑ **Parent:** [Memoization cache contract](#memoization-cache-contract)

A [memoization key](#memoization-key) identifies all information that determines a reusable answer. Write $x$ for explicit arguments and $c$ for relevant context. For a [function](function.md) $f$ and key [function](function.md) $K$, the necessary value condition is

$$
K(x,c)=K(y,d)\ \Longrightarrow\ f(x,c)=f(y,d).
$$

This implication need hold only for contexts in which the entry can be reused. The condition concerns [key equality](data-structure.md#key-equality), not merely equality of [hash function](computer-science.md#hash-function) outputs: a [hash table](data-structure.md#hash-table) must resolve [hash collisions](computer-science.md#hash-collision) by comparing complete keys. Include the identity or version of the procedure if one table stores results for several procedures or changing implementations.

For an original toy example, let $g(n,a)=an$. Caching only by $n$ after $g(3,2)=6$ incorrectly returns $6$ for $g(3,4)$, whose answer is $12$. The pair $(n,a)$ is complete for this [function](function.md). If $a$ is hidden in mutable configuration, either freeze that configuration for the [memoization cache lifetime](#memoization-cache-lifetime), include a reliable version in the key, or invalidate affected entries before reuse. A version is sufficient only if every relevant change updates it. Object identity alone is likewise insufficient for a [mutable list](data-structure.md#mutable-list) whose contents determine the answer.

#### Memoization cache lifetime

↑ **Parent:** [Memoization cache contract](#memoization-cache-contract)

A [memoization cache lifetime](#memoization-cache-lifetime) is the interval over which retained entries are available and valid. One table per top-level request shares recursive subproblems within that request; keeping a table between requests also allows the warm $F_5$ and incremental $F_6$ examples. Clearing it loses those savings. Evicting a correct answer can preserve correctness for a terminating [pure function](programming-language.md#pure-function), while forcing recomputation; changing an input without invalidating an obsolete answer can break correctness.

Specify who owns the table, when context changes invalidate it, and how long keys and results occupy [computer memory](computer-memory.md). In a concrete implementation, retained references can keep arguments and answers alive until removal or clearing.[Python documentation, functools.lru\_cache: cache\_clear and retention of argument and return-value references until eviction or clearing](computer-science-bibliography.md#python-3-14-documentation/functools-higher-order-functions-and-operations-on-callable-objects-python-3-14-documentation) The [memoization](#memoization) promise is conditional reuse of valid completed answers, not an automatic guarantee of freshness, termination or bounded [computer memory](computer-memory.md).

// Target: computer-science.bigb

## Recursion (computer science)

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Recursion_(computer_science))

[Recursion](#recursion-computer-science) solves a problem by invoking the same procedure on smaller instances, with base cases answered directly. For [merge sort](#merge-sort), an empty or one-entry [array](data-structure.md#array-data-structure) is already sorted, and every larger [array](data-structure.md#array-data-structure) is split into two shorter parts. The decreasing lengths justify termination; a self-call without a progress rule would not suffice.

A [recursive procedure](#recursive-procedure) refers to itself, directly or through another procedure. A [recursive call](#recursive-call) starts another invocation, with its own arguments and local [variables](mathematics.md#variable-mathematics); the caller can wait for its returned [output](theoretical-computer-science.md#output-computing). A [base case](#base-case) supplies an answer without further [recursive calls](#recursive-call). To establish [algorithm termination](#algorithm-termination), also show that every [recursive call](#recursive-call) progresses in a [well-founded relation](set-theory.md#well-founded-relation). “Smaller” means smaller in that chosen relation: argument values need not all decrease, and the arguments need not even be numbers.

[Recursion](#recursion-computer-science) is especially expressive when a [data structure](data-structure.md) already decomposes into smaller structures. A [binary tree](data-structure.md#binary-tree) has two child [subtrees](data-structure.md#subtree), so [structural recursion](programming-language.md#structural-recursion) can follow its shape. A short rule for each case can describe an entire traversal or computation. The distinction between a [recursive procedure](#recursive-procedure) and the [recursive process](#recursive-process) it generates helps connect that compact description to its resource use.[Structure and Interpretation of Computer Programs, second edition, §1.2.1: procedure versus process; §1.2.2: closing discussion before Counting change, hierarchical data and straightforward definitions](computer-science-bibliography.md#structure-and-interpretation-of-computer-programs-by-harold-abelson-and-others)

### Guarded recursion

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

A recursive definition in which returning around a recursive dependency requires progress of the kind relevant to its semantics. In [communicating sequential processes](computer-science.md#communicating-sequential-processes), the visible guard must survive [CSP hiding](computer-science.md#csp-hiding); a loop whose apparent guard becomes a [CSP internal action](computer-science.md#csp-internal-action) is not visibly guarded.

### Mutual recursion

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mutual_recursion)

Two or more functions are mutually recursive when their definitions call one another in a cycle. Two [algebraic data types](programming-language.md#algebraic-data-type) can likewise be mutually recursive when constructors of each refer to the other. For alternating sequences `Zig a b` and `Zag b a`, descending one constructor exchanges the [type parameters](programming-language.md#type-parameter); a pair of mapping functions must exchange its arguments correspondingly. A mutually recursive fold may have two independent result types $r,s$: its handlers have types `a -> s -> r` and `b -> r -> s`, with empty results of types `r` and `s`. Equality of the two result types is not required by [type inference](programming-language.md#type-inference).

### Recursion tree

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

A [recursion tree](#recursion-tree) records recursive calls as nodes and their direct recursive subcalls as children. Its node labels can record the work done outside those subcalls. Summing the work over levels or charging it to nodes proves a total [running time](#running-time) bound. For $T(n)=aT(n/b)+f(n)$, level $j$ has approximately $a^j$ instances of size $n/b^j$, so its nonrecursive work is $a^jf(n/b^j)$. Summing those quantities explains the cases of the [master theorem](sequence-and-series.md#master-theorem).

#### Entropy potential for a divide-and-conquer recurrence

↑ **Parent:** [Recursion tree](#recursion-tree)

If $0<m<n$, the displayed identity expresses the decrease of the potential $n\log_2n$ across a split. Here $H_2(a)=-a\log_2a-(1-a)\log_2(1-a)$ is the [binary entropy function](analysis-of-boolean-functions.md#binary-entropy-function). If every split fraction stays in $[\delta,1-\delta]$ for a fixed $0<\delta\leq1/2$, the potential decreases by at least $nH_2(\delta)>0$. Consequently, for a [recurrence relation](sequence-and-series.md#recurrence-relation) with linear work at each split, the [inductive hypothesis](foundations-of-mathematics.md#induction-hypothesis) $T(n)\leq A n\log_2n+B n$ closes when $A H_2(\delta)\geq1$ and $B$ covers the base cases. This is a proof by the [substitution method for a recurrence](sequence-and-series.md#substitution-method-for-a-recurrence) of an $O(n\log n)$ [time complexity](theoretical-computer-science.md#time-complexity) bound without requiring equal subproblem sizes.

### Tail recursion

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

[Recursion](#recursion-computer-science) in which the recursive call is the last operation required to obtain the current call's result. An accumulator can encode the state that would otherwise be updated by a loop. A suitable [compiler](programming-language.md#compiler) can replace the call by a jump, avoiding growing [call stack](data-structure.md#call-stack) storage. In [Scala](programming-language.md#scala), a tail-recursion annotation requests a check that the recursive method is eligible for this transformation.

### McCarthy 91 function

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

#### Generalized McCarthy function

↑ **Parent:** [McCarthy 91 function](#mccarthy-91-function)

### Recursive procedure

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

A procedure whose definition invokes itself directly or indirectly. This is a property of its [programming language syntax](programming-language.md#programming-language-syntax). It does not determine whether execution accumulates unfinished operations.[Structure and Interpretation of Computer Programs, second edition, §1.2.1: paragraph beginning “In contrasting iteration and recursion”](computer-science-bibliography.md#structure-and-interpretation-of-computer-programs-by-harold-abelson-and-others)

### Recursive process

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

A computation that retains pending operations while further calls run, then completes those operations as results return. A [recursive procedure](#recursive-procedure) can instead describe an iterative process: passing an updated accumulator onward may leave no arithmetic pending. Avoiding growing [call stack](data-structure.md#call-stack) storage in that case depends on the implementation. A fixed number of [variables](mathematics.md#variable-mathematics) also does not imply fixed storage in [bits](information-theory.md#bit) when their [integer](integer.md) values grow.[Structure and Interpretation of Computer Programs, second edition, §1.2.1: deferred operations, state variables, and implementation dependence of space use; bit-storage qualification added here](computer-science-bibliography.md#structure-and-interpretation-of-computer-programs-by-harold-abelson-and-others)

### Factorial recursion and returning frames

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

For a [natural number](arithmetic.md#natural-number) $n$, the [factorial](combinatorics.md#factorial) satisfies $0!=1$ and $n!=n(n-1)!$ for $n\geq1$. The following description includes the zero [base case](#base-case) explicitly; a negative or nonintegral [input](theoretical-computer-science.md#input-computer-science) is outside its [precondition](#precondition):
```
F(n):
    require n is an integer and n >= 0
    if n == 0:
        return 1
    child_result = F(n - 1)
    return n * child_result
```
For $n=4$, the arguments on descent are $4,3,2,1,0$. Each positive-argument invocation postpones one [multiplication](arithmetic.md#multiplication) until its [recursive call](#recursive-call) returns. At the deepest point, the [call stack](data-structure.md#call-stack) has five [stack frames](data-structure.md#stack-frame): four suspended callers and the active zero [base case](#base-case). The invocation at zero returns $1$ to the invocation at one, rather than finishing the entire computation. Returns then give

$$
F(0)=1,\quad F(1)=1\cdot1=1,\quad F(2)=2\cdot1=2,\quad F(3)=3\cdot2=6,\quad F(4)=4\cdot6=24.
$$

A [stack frame](data-structure.md#stack-frame) retains the caller's argument and where to resume. When the invocation at three receives $2$, it uses its own $n=3$, obtains $6$, and returns that value to the invocation at four. The [recursive calls](#recursive-call) share a definition, but their local [variables](mathematics.md#variable-mathematics) belong to separate invocations.

<a id="image-factorial-descent-builds-pending-work-returning-frames-complete-it"></a>
![](recursion-factorial-returning-frames.png)

**[Figure 14](#image-factorial-descent-builds-pending-work-returning-frames-complete-it). Factorial descent builds pending work; returning frames complete it**. Original trace of $F(4)$ with [base case](#base-case) $F(0)=1$. The central snapshot shows all five [stack frames](data-structure.md#stack-frame) at maximum depth. Downward arrows create [recursive calls](#recursive-call); upward arrows carry completed answers to suspended callers. A return removes only the completed invocation's [stack frame](data-structure.md#stack-frame).

The [natural number](arithmetic.md#natural-number) measure $n$ decreases by one on every [recursive call](#recursive-call), so [algorithm termination](#algorithm-termination) follows. For [algorithm correctness](#algorithm-correctness), use [mathematical induction](foundations-of-mathematics.md#mathematical-induction): the zero [base case](#base-case) returns $0!=1$; assuming the child's answer is $(n-1)!$, the caller returns $n(n-1)!=n!$. This also explains why keeping the caller's $n$ matters.

There are exactly $n+1$ invocations and $n$ [multiplications](arithmetic.md#multiplication), including one invocation and no [multiplications](arithmetic.md#multiplication) when $n=0$. Ordinary execution of this [recursive process](#recursive-process) uses at most $n+1$ active [stack frames](data-structure.md#stack-frame), hence $O(n)$ frames for $n\geq1$ in [Big O notation](real-analysis.md#big-o-notation). If each test, call, [subtraction](arithmetic.md#subtraction) and [multiplication](arithmetic.md#multiplication) is counted as constant cost, its [time complexity](theoretical-computer-science.md#time-complexity) is $O(n)$. That is an arithmetic-operation model: exact arbitrary-length [integer](integer.md) [multiplication](arithmetic.md#multiplication) has growing cost, and neither the [factorial](combinatorics.md#factorial) [output](theoretical-computer-science.md#output-computing) nor every [stack frame](data-structure.md#stack-frame)'s numeric contents occupies a universally fixed number of [bits](information-theory.md#bit).

### Binary array sum by recursion

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

Keep an [array](data-structure.md#array-data-structure) $A$ unchanged, and sum entries in the half-open [integer interval](integer.md#integer-interval) of [array indices](data-structure.md#array-index) $[l,r)$. The [precondition](#precondition) requires [integers](integer.md) $0\leq l\leq r\leq\operatorname{length}(A)$ and exact, terminating [integer](integer.md) [addition](arithmetic.md#addition). An empty range returns the [empty sum](arithmetic.md#empty-sum) zero; a one-entry range returns that entry. Every longer range splits at its middle [array index](data-structure.md#array-index):
```
S(A, l, r):
    require integer indices with 0 <= l <= r <= length(A)
    size = r - l
    if size == 0:
        return 0
    if size == 1:
        return A[l]
    middle = l + floor(size / 2)
    left_sum = S(A, l, middle)
    right_sum = S(A, middle, r)
    return left_sum + right_sum
```
For the original [array](data-structure.md#array-data-structure) $A=[6,-2,5,1]$, call $S(A,0,4)$. The left half returns $6+(-2)=4$, the right half returns $5+1=6$, and the original invocation returns $4+6=10$. The right half's left endpoint increases from zero to two: what decreases is range length $r-l$, not every argument. Negative entries affect the answer but do not affect [algorithm termination](#algorithm-termination).

<a id="image-seven-calls-compute-an-array-sum-with-only-three-frames-active-at-once"></a>
![](recursion-binary-array-sum-call-tree.png)

**[Figure 15](#image-seven-calls-compute-an-array-sum-with-only-three-frames-active-at-once). Seven calls compute an array sum with only three frames active at once**. Original [binary tree](data-structure.md#binary-tree) of invocations for $A=[6,-2,5,1]$, with [integer intervals](integer.md#integer-interval) labeling ranges and upward arrows labeling returned sums. Small numbers give the order in which invocations begin when the left child runs first. The highlighted [graph path](graph-theory.md#path-in-a-graph) contains the three active [stack frames](data-structure.md#stack-frame) while the entry $-2$ is read; the result $6$ from the completed left sibling is retained by its parent.

For range length $n=r-l\geq2$, the children have lengths $\lfloor n/2\rfloor$ and $\lceil n/2\rceil$, both positive and strictly less than $n$. The [floor function](calculus.md#floor-function) chooses the split; the [ceiling function](calculus.md#ceiling-function) gives the other length. [Algorithm termination](#algorithm-termination) follows by this [natural number](arithmetic.md#natural-number) measure. For [algorithm correctness](#algorithm-correctness), apply [mathematical induction](foundations-of-mathematics.md#mathematical-induction) on $n$: the two [base cases](#base-case) return the specified [sum](arithmetic.md#sum); for a larger range, the two disjoint child ranges cover every original [array index](data-structure.md#array-index) exactly once, so [addition](arithmetic.md#addition) of their correct [sums](arithmetic.md#sum) gives the required [sum](arithmetic.md#sum).

For $n\geq1$, the invocation [tree](tree-graph-theory.md) is a [full binary tree](data-structure.md#full-binary-tree) with $n$ leaves, one per [array](data-structure.md#array-data-structure) entry. If $I$ is its number of nonleaf [vertices](graph.md#vertex-graph-theory), counting [edges](graph-theory.md#edge-of-a-graph) gives $2I=I+n-1$, so $I=n-1$. Thus the total invocation count is $2n-1$, and there are $n-1$ combining [additions](arithmetic.md#addition). Here $n=4$ gives seven calls and three combining [additions](arithmetic.md#addition). For $n=1$, there is one call and no combining [addition](arithmetic.md#addition); for $n=0$, there is also one call and no combining [addition](arithmetic.md#addition), but no entry leaf, so the $2n-1$ formula does not apply.

The [call stack](data-structure.md#call-stack) holds the active branch, rather than the entire invocation [tree](tree-graph-theory.md). Execute the left child completely before the right child, retaining the left result in the parent [stack frame](data-structure.md#stack-frame). The maximum number of active [stack frames](data-structure.md#stack-frame) is $1+\lceil\log_2 n\rceil$ for $n\geq1$, and one for $n=0$. Balanced splitting therefore needs $O(\log n)$ frames for $n\geq2$, compared with the $O(n)$ frames of the [factorial](combinatorics.md#factorial) [recursive process](#recursive-process). Assuming constant-cost [array](data-structure.md#array-data-structure) access, index operations and [addition](arithmetic.md#addition), its [time complexity](theoretical-computer-science.md#time-complexity) is $O(n)$ and its auxiliary [space complexity](theoretical-computer-science.md#space-complexity) is $O(\log n)$ [machine words](computer-science.md#machine-word) for $n\geq2$, excluding the stored [input](theoretical-computer-science.md#input-computer-science). Pass the same [array](data-structure.md#array-data-structure) with different endpoints, rather than copying slices. These bounds require all stored indices and partial sums to fit in a constant number of [machine words](computer-science.md#machine-word); exact unbounded [integer](integer.md) [addition](arithmetic.md#addition) and storage require a separate [bit](information-theory.md#bit) cost analysis.

### Well-founded progress in recursion

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

A [base case](#base-case) and a decreasing [natural number](arithmetic.md#natural-number) measure work together. Check that every invocation satisfies its [precondition](#precondition), each [base case](#base-case) finishes with the correct [output](theoretical-computer-science.md#output-computing), and every other invocation makes finitely many [recursive calls](#recursive-call) with strictly smaller measure. All local work must also terminate. By [well-founded induction](set-theory.md#well-founded-induction), the children finish, so their caller finishes; if their answers are correct and the combination rule preserves the [postcondition](#postcondition), the caller is correct too. This proves [total correctness](#total-correctness), not just correctness conditional on return.

Strict decrease without a lower bound is insufficient: subtracting one forever from a negative [integer](integer.md) never reaches zero. Even a positive real-valued measure can decrease indefinitely, as $1,1/2,1/4,\ldots$ shows. A [well-founded relation](set-theory.md#well-founded-relation) rules out that descent. In [structural recursion](programming-language.md#structural-recursion), a proper child [subtree](data-structure.md#subtree) of a finite [binary tree](data-structure.md#binary-tree) supplies progress without numeric arguments. The proof obligation is the relation between parent and child instances, together with terminating local work and complete [base cases](#base-case).

### Base case

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

A case answered without further [recursive calls](#recursive-call). Complete [base cases](#base-case) are one part of an [algorithm termination](#algorithm-termination) argument; the other cases must progress in a [well-founded relation](set-theory.md#well-founded-relation).

### Recursive call

↑ **Parent:** [Recursion (computer science)](#recursion-computer-science)

An invocation made by a [recursive procedure](#recursive-procedure) of itself, directly or through another procedure. Each invocation has its own arguments and local [variables](mathematics.md#variable-mathematics); a returning invocation supplies an [output](theoretical-computer-science.md#output-computing) to its caller.

## Divide-and-conquer algorithm

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divide-and-conquer_algorithm)

A [divide-and-conquer algorithm](#divide-and-conquer-algorithm) divides a problem into smaller instances, solves them using [recursion](#recursion-computer-science), and combines their answers. In [merge sort](#merge-sort), the division makes two contiguous halves, and the [merge algorithm](#merge-algorithm) combines the resulting [sorted arrays](data-structure.md#sorted-array). The important design step is finding a combination rule cheaper than solving the whole problem afresh.

Halving the [input](theoretical-computer-science.md#input-computer-science) is only one part of the design. The number of [recursive calls](#recursive-call) and the work outside those calls determine whether the smaller instances actually save time. [Divide-and-conquer combination cost](#divide-and-conquer-combination-cost) keeps these quantities separate; the [divide-and-conquer product ledger](#divide-and-conquer-product-ledger) shows how an algebraic identity changes the number of required calls in [Karatsuba multiplication](#karatsuba-multiplication).

For [algorithm correctness](#algorithm-correctness), specify the meaning of each returned answer, prove the [base cases](#base-case), and show that combining correct smaller answers gives the required [output](theoretical-computer-science.md#output-computing). [Induction](foundations-of-mathematics.md#mathematical-induction) then proves correctness, provided every [recursive call](#recursive-call) progresses towards a [base case](#base-case). The combination rule must reconstruct everything the caller needs: two sorted halves alone are not a [sorted array](data-structure.md#sorted-array), and four digit blocks alone are not their [integer](integer.md) product.

### Integer rounding in a divide-and-conquer recurrence

↑ **Parent:** [Divide-and-conquer algorithm](#divide-and-conquer-algorithm)

An integer-valued problem size requires integer subproblem sizes and a base case. For the displayed unequal split with $n\geq2$, both children have positive size less than $n$, and $1/4\leq m/n\leq1/2$. The [entropy potential for a divide-and-conquer recurrence](#entropy-potential-for-a-divide-and-conquer-recurrence) therefore supplies a uniform positive potential decrease. The squared sizes satisfy $m^2+(n-m)^2\leq5n^2/8$, which similarly closes a quadratic [inductive hypothesis](foundations-of-mathematics.md#induction-hypothesis) when the work at the root is $n^2$.

### Simultaneous minimum and maximum

↑ **Parent:** [Divide-and-conquer algorithm](#divide-and-conquer-algorithm)

The minimum and maximum of a nonempty [array](data-structure.md#array-data-structure) can be found with at most $\lceil3n/2\rceil-2$ pairwise comparisons. Compare consecutive pairs once, retaining smaller entries as minimum candidates and larger entries as maximum candidates. If an entry is unpaired, put it into both candidate sets. Each candidate set has $\lceil n/2\rceil$ entries, and finding one extremum on $r$ entries uses $r-1$ comparisons. Thus the total is $\lfloor n/2\rfloor+2(\lceil n/2\rceil-1)$, equal to the stated bound; the singleton case uses zero. Balanced [divide-and-conquer algorithms](#divide-and-conquer-algorithm) can perform both candidate reductions. Pairing is important: arbitrary equal splitting with only a two-element base case does not attain this comparison count at every size.

### Array local maximum

↑ **Parent:** [Divide-and-conquer algorithm](#divide-and-conquer-algorithm)

An entry of a finite [array](data-structure.md#array-data-structure) which strictly exceeds each existing immediate neighbour. At either endpoint only one neighbour is tested, and the unique entry of a singleton qualifies vacuously. For distinct entries, a [divide-and-conquer algorithm](#divide-and-conquer-algorithm) finds such an entry in $O(\log n)$ time. Maintain an index interval whose left endpoint exceeds the excluded entry immediately to its left, if any, and whose right endpoint exceeds the excluded entry immediately to its right, if any. If a midpoint has a larger internal neighbour, recurse towards it; the comparison supplies the new boundary inequality. Otherwise the midpoint exceeds its internal neighbours and the boundary inequalities cover any external neighbour. Halving the interval and preserving this [recursion invariant](#recursion-invariant) proves correctness and the bound.

### Divide-and-conquer majority element

↑ **Parent:** [Divide-and-conquer algorithm](#divide-and-conquer-algorithm)

An entry occurring strictly more than half the time in an [array](data-structure.md#array-data-structure) must occur strictly more than half the time in at least one half: otherwise the two frequency bounds sum to at most half the whole length. Recursively find each half's possible [majority element](data-structure.md#majority-element), then verify at most two candidates over the whole subarray using only equality tests. [Induction](foundations-of-mathematics.md#mathematical-induction) proves correctness, and linear combination work over a balanced [recursion](#recursion-computer-science) tree gives worst-case $\Theta(n\log n)$ time. A tagged absent result avoids confusing failure with a valid element.

### CDQ divide and conquer

↑ **Parent:** [Divide-and-conquer algorithm](#divide-and-conquer-algorithm)

### Divide-and-conquer combination cost

↑ **Parent:** [Divide-and-conquer algorithm](#divide-and-conquer-algorithm)

The combination cost is the work needed to reconstruct an answer from the returned smaller answers. In a [time complexity](theoretical-computer-science.md#time-complexity) calculation, also count partitioning the [input](theoretical-computer-science.md#input-computer-science), preparing arguments, and other work outside [recursive calls](#recursive-call). Write their total as $g(n)$ for a size-$n$ call. For an ideal balanced [divide-and-conquer algorithm](#divide-and-conquer-algorithm) making $a$ calls of size $n/2$, the [recurrence relation](sequence-and-series.md#recurrence-relation) is

$$
T(1)=c_0,\qquad T(n)=aT(n/2)+g(n)\quad(n>1),
$$

where $a$ is a fixed positive [integer](integer.md) and $c_0>0$ is the [base case](#base-case) cost. Take $n=2^k$, a [power of two](integer.md#power-of-two), so the size becomes one after exactly $k$ divisions. This is a model of total sequential work: all $a$ smaller calls contribute, even if a machine could run some simultaneously.

At level $j$, there are $a^j$ calls, each of size $n/2^j$. Expanding the [recurrence relation](sequence-and-series.md#recurrence-relation) gives the exact identity

$$
T(n)=a^k c_0+\sum_{j=0}^{k-1}a^j g(n/2^j).
$$

The first term counts the [base cases](#base-case); the [sum](arithmetic.md#sum) stops before their level because $g$ describes work in nonterminal calls. This separates depth, number of calls, and local work. [Merge sort](#merge-sort) has two smaller calls and a linear [merge algorithm](#merge-algorithm), giving $T(n)=2T(n/2)+O(n)=O(n\log n)$ in [Big O notation](real-analysis.md#big-o-notation). The MIT notes derive this by summing equal work across levels, and contrast it with the same two-way split followed by quadratic local work.[6.006 Introduction to Algorithms, Fall 2011, Lecture 3: slides 32–44, recurrence and equal work per level; slide 46, quadratic local work](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-3-insertion-sort-merge-sort)

<a id="image-the-same-halving-tree-can-have-linear-or-quadratic-work-at-each-call"></a>
![](divide-and-conquer-combination-work-levels.png)

**[Figure 16](#image-the-same-halving-tree-can-have-linear-or-quadratic-work-at-each-call). The same halving tree can have linear or quadratic work at each call**. Original exact cost models with $n=16$, two children per nonterminal call, and one unit per [base case](#base-case). For local work $g(s)=s$, every internal level costs 16 and the total is 80. For $g(s)=s^2$, internal levels cost 256, 128, 64, 32 and the total is 496. The tree shows instance sizes; the ledger counts work rather than execution order.

For the first constructed model, set $a=2$, $c_0=1$ and $g(s)=s$. Every internal level costs $2^j(n/2^j)=n$, while the leaves cost $n$. Thus $T(n)=n\log_2 n+n$, giving $T(16)=80$. If the same split instead has $g(s)=s^2$, then the [finite geometric series](sequence-and-series.md#finite-geometric-series) gives

$$
T(n)=n+n^2\sum_{j=0}^{k-1}2^{-j}=2n^2-n,
$$

so $T(16)=496$. The root alone already costs $n^2$ in this second model. Smaller arguments do not eliminate expensive reconstruction. These are stipulated operation counts, rather than measured running times or exact [merge sort](#merge-sort) instruction counts.

[Binary search](#binary-search) has a different saving: after its comparison, only one half remains a candidate. With constant-cost indexed [array](data-structure.md#array-data-structure) access and comparisons, its worst-case [time complexity](theoretical-computer-science.md#time-complexity) satisfies an upper [recurrence relation](sequence-and-series.md#recurrence-relation) $T(n)\leq T(\lfloor n/2\rfloor)+C$ for $n\geq1$, with $T(0)=c_0$. There is one continuing branch, rather than two. At most $\lfloor\log_2 n\rfloor+1$ nonempty candidate ranges are inspected for $n\geq1$. Copying the retained half into a fresh [array](data-structure.md#array-data-structure) on every step would add linear work at that step and lose this logarithmic bound. The shrinking range and its representation both matter.

### Divide-and-conquer product ledger

↑ **Parent:** [Divide-and-conquer algorithm](#divide-and-conquer-algorithm)

Splitting two [integers](integer.md) in [positional notation](integer.md#positional-notation) gives $x=aq+b$ and $y=cq+d$, where $q=B^m$ shifts a block by $m$ [numeral digits](integer.md#numerical-digit) in fixed [radix](integer.md#radix) $B\geq2$. The [distributive property](algebraic-operation.md#distributive-property) gives

$$
xy=acq^2+(ad+bc)q+bd.
$$

Computing $ac,ad,bc,bd$ separately needs four block [multiplications](arithmetic.md#multiplication). Merely halving the operands therefore gives an ideal [recurrence relation](sequence-and-series.md#recurrence-relation) $F(n)=4F(n/2)+O(n)$, still with quadratic [time complexity](theoretical-computer-science.md#time-complexity). The [Karatsuba three-product identity](#karatsuba-three-product-identity) instead computes $ac$, $bd$ and $(a+b)(c+d)$, recovering the middle [coefficient](vector-space.md#coefficient) by two [subtractions](arithmetic.md#subtraction). The MIT notes present precisely this four-product versus three-product distinction.[6.006 Introduction to Algorithms, Fall 2011, Lecture 11: Numerics I, printed pp. 4–5, High Precision Multiplication and Karatsuba's Method](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-11-numerics-i)

For an original small example, multiply $47$ by $63$. Set $B=q=10$, $a=4$, $b=7$, $c=6$, $d=3$. Four separate block products would give $ac=24$, $ad=12$, $bc=42$, $bd=21$. The three-product calculation is

$$
\begin{aligned}
u&=ac=24,&v&=bd=21,&w&=(a+b)(c+d)=11\cdot9=99,\\
h&=w-u-v=99-24-21=54,\\
47\cdot63&=100u+10h+v=2400+540+21=2961.
\end{aligned}
$$

The crucial reuse is that $u$ and $v$ supply the outer [coefficients](vector-space.md#coefficient) and also remove the unwanted terms from $w$. There is no need to compute $ad$ and $bc$ separately. Expanding $w=ac+ad+bc+bd$ proves the identity. [Induction](foundations-of-mathematics.md#mathematical-induction) extends it to [Karatsuba multiplication](#karatsuba-multiplication) once each smaller block product is correct and [Karatsuba recursion termination](#karatsuba-recursion-termination) supplies decreasing sizes and complete [base cases](#base-case).

<a id="image-four-block-products-or-three-the-exact-ledger-for-47-cdot63"></a>
![](divide-and-conquer-four-versus-three-products.png)

**[Figure 17](#image-four-block-products-or-three-the-exact-ledger-for-47-cdot63). Four block products or three: the exact ledger for $47\cdot63$**. The left ledger computes both cross products separately. The right ledger reuses $ac=24$ and $bd=21$ to recover their sum as $99-24-21=54$. Both reconstructions yield $2961$. Counts refer to block [multiplication](arithmetic.md#multiplication) calls at this split; the extra [numeral digit](integer.md#numerical-digit) in $4+7=11$ prevents interpreting all three as single-digit products.

The operation model matters. Let $n$ count [numeral digits](integer.md#numerical-digit) in fixed [radix](integer.md#radix) $B$, and count single-digit [multiplication](arithmetic.md#multiplication), [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction) and copying as constant-cost operations. The nonrecursive work on size-$n$ operands is $O(n)$: it includes forming sums, positional shifts and [Karatsuba carry handling](#karatsuba-carry-handling). Treating an arbitrarily large [integer](integer.md) [multiplication](arithmetic.md#multiplication) as one operation would hide the very saving being studied. The coefficients $24,54,21$ above must be shifted and added; concatenating them does not give $2961$.

In the ideal equal-half model, [Karatsuba multiplication](#karatsuba-multiplication) has $K(n)=3K(n/2)+O(n)$. At depth $j$ its additional work is at most a constant times $n(3/2)^j$, and its leaf count is $3^k=n^{\log_2 3}$ for $n=2^k$. A [geometric series](sequence-and-series.md#geometric-series) gives $K(n)=O(n^{\log_2 3})$, where $\log_2 3\approx1.585$. Four recursive products would instead give $4^k=n^2$ leaves. Saving one block product repeatedly changes the exponent, even though the combination requires extra [addition](arithmetic.md#addition) and [subtraction](arithmetic.md#subtraction).

For the literal sum-based version, each operand sum can occupy one extra [numeral digit](integer.md#numerical-digit). Its worst-case upper [recurrence relation](sequence-and-series.md#recurrence-relation) is $K(n)\leq3K(\lceil n/2\rceil+1)+Cn$ for a nondecreasing cost envelope, above a fixed [base case](#base-case) threshold of at least three digits. [Karatsuba digit-operation cost](#karatsuba-digit-operation-cost) proves that this extra digit preserves the exponent; [Karatsuba operand splitting](#karatsuba-operand-splitting) handles odd lengths and leading zero padding. For signed [integers](integer.md), apply the nonnegative procedure to their [absolute values](real-analysis.md#absolute-value) and restore the sign. The small ledger establishes an exact identity, while [Karatsuba practical crossover](#karatsuba-practical-crossover) explains why it alone cannot predict a speedup for two-digit operands.

## Sorting algorithm

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sorting_algorithm)

A [sorting algorithm](#sorting-algorithm) rearranges a finite [sequence](sequence-and-series.md#sequence) into nondecreasing order under a chosen [total order](set.md#total-order) on its keys. Its [output](theoretical-computer-science.md#output-computing) must contain every [input](theoretical-computer-science.md#input-computer-science) entry exactly once, including repetitions: producing ordered values is insufficient if entries are lost. [Merge sort](#merge-sort) is one such [algorithm](algorithm.md); [stable sorting](#stable-sorting) adds a requirement about equal keys.

Sorting creates reusable structure: equal [sort keys](#sort-key) become adjacent, and a [sorted array](data-structure.md#sorted-array) supports [binary search](#binary-search). However, an [algorithm correctness](#algorithm-correctness) check must establish both [sortedness](#sortedness) and [sorting permutation preservation](#sorting-permutation-preservation). Replacing every entry by the smallest key can produce ordered keys while destroying the original data. [Stable sorting](#stable-sorting) imposes a third condition when equal [sort keys](#sort-key) occur: retain their arrival order.

For example, take complete [sorting records](#sorting-record) $(2,A),(1,B),(2,C),(1,D)$, with the first component as the [sort key](#sort-key) and the letter as associated data. A correct [output](theoretical-computer-science.md#output-computing) is $(1,B),(1,D),(2,A),(2,C)$. The [sort keys](#sort-key) are ordered, every complete [sorting record](#sorting-record) remains, and the equal-key pairs keep $A$ before $C$ and $B$ before $D$. The [output](theoretical-computer-science.md#output-computing) $(1,D),(1,B),(2,C),(2,A)$ satisfies [sortedness](#sortedness) and [sorting permutation preservation](#sorting-permutation-preservation), but fails [stable sorting](#stable-sorting). The [output](theoretical-computer-science.md#output-computing) $(1,B),(1,B),(2,A),(2,A)$ has the right [multiset](set.md#multiset) of [sort keys](#sort-key) but loses $C,D$ and duplicates $A,B$; it fails [sorting permutation preservation](#sorting-permutation-preservation) of complete [sorting records](#sorting-record).

To express [stable sorting](#stable-sorting) precisely, label every [input](theoretical-computer-science.md#input-computer-science) occurrence by its original position, even when two complete [sorting records](#sorting-record) have identical contents. Let $p(i)$ be the [output](theoretical-computer-science.md#output-computing) position of the occurrence originally at position $i$. Besides [sortedness](#sortedness) and [sorting permutation preservation](#sorting-permutation-preservation), require

$$
i<j\ \text{and}\ k(A_i)=k(A_j)\quad\Longrightarrow\quad p(i)<p(j).
$$

Here $k$ is the [sort key](#sort-key) [function](function.md). Sorting by the pair $(k(A_i),i)$ under [lexicographic order](extremal-set-theory.md#lexicographic-order) gives the same order as [stable sorting](#stable-sorting) by $k$: the original position breaks ties without discarding associated data. For a two-field ordering, first apply [stable sorting](#stable-sorting) by the secondary [sort key](#sort-key), then apply [stable sorting](#stable-sorting) by the primary [sort key](#sort-key). The second pass retains the secondary order within each group of equal primary [sort keys](#sort-key). For instance, $(2,B),(1,C),(2,A),(1,A)$ first becomes $(2,A),(1,A),(2,B),(1,C)$ by letter, then $(1,A),(1,C),(2,A),(2,B)$ by number.

### External merge sort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

A [sorting algorithm](#sorting-algorithm) that sorts memory-sized runs and merges them using storage-backed passes. It can also eliminate repeated [database tuples](computer-science.md#database-tuple).

### Stooge sort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stooge_sort)

First exchange the endpoints of the current subarray if they are out of order. For current length $m>2$, put $k=\lfloor m/3\rfloor$ and recursively sort its first $m-k$ entries, its last $m-k$ entries, then its first $m-k$ entries again. Each child has length $\lceil2m/3\rceil$; the split must use the current subproblem length. The [master theorem](sequence-and-series.md#master-theorem) gives exponent $\log_{3/2}3\approx2.7095$, worse than quadratic. The usual algorithm is not stable: endpoint exchange on $[2_a,2_b,1]$ leaves the equal-key records reversed after sorting.

### Heapsort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Heapsort)

Build a [max-heap](data-structure.md#max-heap) in an [array](data-structure.md#array-data-structure), then repeatedly exchange its root with the last element of the active heap and restore [heap order](data-structure.md#heap-order) by [heapify down](data-structure.md#sift-down). The inactive suffix grows in ascending order. Bottom-up heap construction costs $O(n)$ because the number of nodes at height $h$ decreases geometrically, and the extraction phase costs $O(n\log n)$. Iterative sifting uses constant auxiliary storage. Long-distance exchanges can reverse equal-key records, so the usual version does not provide [stable sorting](#stable-sorting).

### Prefix reversal sorting

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

To sort a [permutation](combinatorics.md#permutation) using [prefix reversals](combinatorics.md#prefix-reversal), work backwards through final positions. On an active prefix of length $m$, find its largest value. If it is already at the final position, shorten the active prefix. Otherwise move it to the front with one reversal if necessary, then reverse the entire active prefix to put it last. Already settled suffix positions are untouched.

The settled suffix is a [loop invariant](#loop-invariant), and active-prefix length decreases to one. This proves reachability of the identity [permutation](combinatorics.md#permutation) in at most $2(n-1)$ nontrivial flips. The construction is a finite upper bound, not a promise of minimum length; [breadth-first search](tree-graph-theory.md#breadth-first-search) can find the minimum for small instances.

### Selection sort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

Selection sort repeatedly chooses a minimum element from the unprocessed collection and moves it to the next output position. After each step the output [string prefix](data-structure.md#string-prefix) is sorted and no larger than any remaining element. Repeated linear minimum scans give quadratic worst-case time. A [linked list](data-structure.md#linked-list) implementation can detach and append existing nodes using constant auxiliary space while preserving duplicate elements. The sorted result is nondecreasing, not strictly increasing when duplicates occur.

### Quicksort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

A [divide-and-conquer algorithm](#divide-and-conquer-algorithm) that partitions entries relative to a pivot, recursively sorts the smaller and larger partitions, and combines their results. A three-way partition keeps all equal keys in a central bucket. Correctness follows from the partition order and recursive correctness; excluding the pivot from child inputs provides decreasing finite lengths. The choice of pivot controls balance and therefore running time.

#### Three-way quicksort

↑ **Parent:** [Quicksort](#quicksort)

Partitioning into keys smaller than, equal to and greater than the pivot. Only the smaller and greater partitions need recursive sorting. Keeping the common partition helper in both a direct sorter and a tree-building factorisation ensures that flattening the tree introduces no extra key comparisons.

### Bitonic sorting algorithm

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

A [divide-and-conquer algorithm](#divide-and-conquer-algorithm) that sorts two halves, reverses one result to form a [bitonic sequence](sequence-and-series.md#bitonic-sequence), then performs a bitonic merge. For the shuffle-and-adjacent-comparison merging network on $n=2^k$ entries, $k$ passes each cost $\Theta(n)$, so merging costs $\Theta(n\log n)$. The complete [recurrence relation](sequence-and-series.md#recurrence-relation) is $T(n)=2T(n/2)+\Theta(n\log n)$, giving $\Theta(n(\log n)^2)$ time. A compare-exchange operation preserves the [multiset](set.md#multiset) of entries while putting its two selected entries in order.

### Patience sorting

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

### Sort key

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

A [sort key](#sort-key) is the value extracted from a complete entry to determine its ordering. Model extraction as a [function](function.md) $k$ into a [total order](set.md#total-order); compare $k(A_i)$ and $k(A_j)$, while moving the complete entries. Ordering [sorting records](#sorting-record) by an age field does not also compare their names. Repeated [sort keys](#sort-key) are allowed, so this induces equal-key groups even when the complete [sorting records](#sorting-record) differ. Keep the [sort key](#sort-key) [function](function.md) and the comparison rule fixed throughout a sort; inconsistent comparisons need not admit any sorted result.

#### Sorting record

↑ **Parent:** [Sort key](#sort-key)

A complete entry comprising a [sort key](#sort-key) together with any associated data. In $(2,A)$, the [sort key](#sort-key) is $2$ and $A$ stands for the associated data or an identity label. [Sorting permutation preservation](#sorting-permutation-preservation) concerns these complete entries, rather than only their extracted [sort keys](#sort-key).

### Sortedness

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

For an [output](theoretical-computer-science.md#output-computing) [sequence](sequence-and-series.md#sequence) $B$ of length $n$, [sortedness](#sortedness) means

$$
k(B_i)\leq k(B_{i+1})\qquad(0\leq i<n-1)
$$

under the chosen [total order](set.md#total-order) on [sort keys](#sort-key). Its [transitivity](set-theory.md#transitive-relation) also gives $k(B_i)\leq k(B_j)$ whenever $i<j$. An empty [sequence](sequence-and-series.md#sequence) and a one-entry [sequence](sequence-and-series.md#sequence) satisfy [sortedness](#sortedness) without any adjacent comparison. For longer [sequences](sequence-and-series.md#sequence), checking adjacent pairs suffices; checking only the first and last [sort keys](#sort-key) does not. For example, $(1,3,2,4)$ passes an endpoint comparison but fails [sortedness](#sortedness) at $3,2$. [Sortedness](#sortedness) alone says nothing about which [input](theoretical-computer-science.md#input-computer-science) entries survived.

### Sorting permutation preservation

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

The [output](theoretical-computer-science.md#output-computing) of a [sorting algorithm](#sorting-algorithm) must be a [permutation](combinatorics.md#permutation) of the complete [input](theoretical-computer-science.md#input-computer-science) [sequence](sequence-and-series.md#sequence). For equal lengths $n$, require a [permutation](combinatorics.md#permutation) $\pi$ of $\{0,\ldots,n-1\}$ such that

$$
B_i=A_{\pi(i)}\qquad(0\leq i<n).
$$

Equivalently, the [input](theoretical-computer-science.md#input-computer-science) and [output](theoretical-computer-science.md#output-computing) have the same [multiset](set.md#multiset) of complete entries: each entry has the same multiplicity. Equality of the underlying [sets](set.md) is insufficient; $(1,1,2)$ and $(1,2,2)$ have the same [set](set.md) of values and the same length but different [multisets](set.md#multiset). When tracking occurrences rather than contents, retain original identity labels to check that each one is moved exactly once. A swap preserves this [multiset](set.md#multiset) automatically; an overwrite need not.

### Insertion sort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Insertion_sort)

[Insertion sort](#insertion-sort) grows a sorted prefix of an [array](data-structure.md#array-data-structure) one entry at a time. In the adjacent-swap version, start with position $i=1$, compare its current [sort key](#sort-key) with the preceding [sort key](#sort-key), and swap the complete [sorting records](#sorting-record) only when the right [sort key](#sort-key) is strictly smaller. Continue leftward until no swap is needed or the entry reaches position zero; then process original position $i+1$. A tie stops the pass. This is the strict comparison and exchange rule in the authored implementation.[Insertion.java by Robert Sedgewick and others](computer-science-bibliography.md#insertion-java-by-robert-sedgewick-and-others)

Take $A=(2_A,1_B,2_C,1_D)$, where the subscript labels a complete [sorting record](#sorting-record) and comparisons inspect only its [sort key](#sort-key). Starting from index zero, the complete key-comparison trace is:

| Comparison | Right [sort key](#sort-key) smaller than left? | Action | [Array](data-structure.md#array-data-structure) after the action |
| --- | --- | --- | --- |
| 1, insert position $1$ | $1_B<2_A$: yes | Swap positions $0,1$. | $(1_B,2_A,2_C,1_D)$ |
| 2, insert position $2$ | $2_C<2_A$: no | Stop this pass on a tie. | $(1_B,2_A,2_C,1_D)$ |
| 3, insert position $3$ | $1_D<2_C$: yes | Swap positions $2,3$. | $(1_B,2_A,1_D,2_C)$ |
| 4, continue leftward | $1_D<2_A$: yes | Swap positions $1,2$. | $(1_B,1_D,2_A,2_C)$ |
| 5, continue leftward | $1_D<1_B$: no | Stop this pass on a tie. | $(1_B,1_D,2_A,2_C)$ |

<a id="sorting-stable-insertion-compare-swap-trace"></a>
![](sorting-stable-insertion-compare-swap-trace.png)

**[Figure 18](#sorting-stable-insertion-compare-swap-trace). Insertion sort: five sort key comparisons and three complete-entry swaps**. Each row after the [input](theoretical-computer-science.md#input-computer-science) shows the state after one comparison. Orange cells mark an adjacent swap; green cells mark a stopping tie. Identity letters are not compared. Both equal-key groups retain their [input](theoretical-computer-science.md#input-computer-science) order, demonstrating [stable sorting](#stable-sorting).

The [loop invariant](#loop-invariant) is that, before pass $i$, positions $0,\ldots,i-1$ satisfy [sortedness](#sortedness) and contain precisely the entries originally in that prefix. Moving the next entry left through strictly larger [sort keys](#sort-key) extends that prefix, and every swap retains [sorting permutation preservation](#sorting-permutation-preservation). Equal-key entries never cross, giving [stable sorting](#stable-sorting). Each leftward step decreases the position, and each completed pass increases the prefix length, so the [algorithm](algorithm.md) terminates.

With constant-cost key comparisons and swaps, reverse-ordered distinct [sort keys](#sort-key) cause $1+2+\cdots+(n-1)=n(n-1)/2$ comparisons and swaps. Thus worst-case [time complexity](theoretical-computer-science.md#time-complexity) is $O(n^2)$ in [Big O notation](real-analysis.md#big-o-notation). An already sorted [array](data-structure.md#array-data-structure) needs only $n-1$ key comparisons for $n\geq1$ and no swaps. The adjacent-swap version uses constant auxiliary [space complexity](theoretical-computer-science.md#space-complexity). Small or nearly sorted [arrays](data-structure.md#array-data-structure) can therefore make [insertion sort](#insertion-sort) useful despite its quadratic worst case.

### Comparison sort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Comparison_sort)

A [comparison sort](#comparison-sort) learns the ordering of [sort keys](#sort-key) only by comparing pairs. The keys are otherwise opaque: their numeric values, digits or encodings cannot choose an [array](data-structure.md#array-data-structure) index or a branch. It may move complete [sorting records](#sorting-record) and retain previous answers. [Merge sort](#merge-sort) and the adjacent-swap [insertion sort](#insertion-sort) are [comparison sorts](#comparison-sort); [counting sort](#counting-sort) and [radix sort](#radix-sort) exploit additional information.

#### Comparison sorting lower bound

↑ **Parent:** [Comparison sort](#comparison-sort)

Any deterministic [comparison sort](#comparison-sort) correct for all orders of $n$ distinct [sort keys](#sort-key) needs at least $\lceil\log_2(n!)\rceil$ comparisons on some [input](theoretical-computer-science.md#input-computer-science). Here $n!$ is a [factorial](combinatorics.md#factorial), $\log_2$ a [logarithm](calculus.md#logarithm), and the brackets denote the [ceiling function](calculus.md#ceiling-function). This is a worst-case requirement, not a requirement on every [input](theoretical-computer-science.md#input-computer-science).[Theorem 11.5: deterministic comparison-tree lower bound](computer-science-bibliography.md#open-data-structures-an-introduction-by-pat-morin/11-1-comparison-based-sorting)

For three distinct [sort keys](#sort-key), the diagram has one leaf for each possible ordering of the original entries $a,b,c$. Some paths need two comparisons, others three; two comparisons cannot distinguish all six orders.

<a id="sorting-three-distinct-keys-comparison-decision-tree"></a>
![](sorting-three-distinct-keys-comparison-decision-tree.png)

**[Figure 19](#sorting-three-distinct-keys-comparison-decision-tree). A comparison decision tree distinguishes the six orders of three distinct sort keys**. Each internal node tests the [sort keys](#sort-key) of two fixed original entries. A leaf gives the order in which their complete [sorting records](#sorting-record) must be emitted. There are $3!=6$ leaves and maximum depth three. The diagram assumes distinct [sort keys](#sort-key), so no equality branch is needed.

For the proof outline, represent adaptive comparisons by a [binary tree](data-structure.md#binary-tree): distinct [sort keys](#sort-key) give only two outcomes per comparison. A leaf fixes an [output](theoretical-computer-science.md#output-computing) [permutation](combinatorics.md#permutation); one leaf cannot correctly handle two different strict orders. Hence there must be at least $n!$ leaves. Maximum depth $h$ permits at most $2^h$ leaves, so $2^h\geq n!$ gives the bound. Even a three-way comparator has only two reachable outcomes on this distinct-key family.

The growth follows without a precise approximation to the [factorial](combinatorics.md#factorial). At least $\lfloor n/2\rfloor$ of its factors are at least $n/2$, so for $n\geq2$,

$$
\log_2(n!)\geq\lfloor n/2\rfloor\log_2(n/2).
$$

The brackets denote the [floor function](calculus.md#floor-function). This gives a constant times $n\log n$ lower bound for large $n$, matching the worst-case comparison growth of [merge sort](#merge-sort).

Distinct [sort keys](#sort-key) are essential to the $n!$ counting argument. Identical [sort keys](#sort-key) do not create $n!$ different strict orders. If all [sort keys](#sort-key) coincide, [stable sorting](#stable-sorting) returns the arrival order. This does not remove the worst-case bound for a [comparison sort](#comparison-sort) required to handle arbitrary distinct-key [inputs](theoretical-computer-science.md#input-computer-science).

### Counting sort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Counting_sort)

[Counting sort](#counting-sort) uses [integer](integer.md) [sort keys](#sort-key) in $\{0,\ldots,K-1\}$ directly as indices into an [array](data-structure.md#array-data-structure) of counts. Constant-cost counting and indexing give $O(n+K)$ [time complexity](theoretical-computer-science.md#time-complexity) in [Big O notation](real-analysis.md#big-o-notation). To retain complete [sorting records](#sorting-record), cumulative counts locate their [output](theoretical-computer-science.md#output-computing) ranges; filling each range from its end while scanning the [input](theoretical-computer-science.md#input-computer-science) backwards gives [stable sorting](#stable-sorting). Emitting bare [sort keys](#sort-key) from counts would discard associated data. The $K$ term matters when the key range is large.[Open Data Structures: An Introduction by Pat Morin; Theorem 11.7 and stability](computer-science-bibliography.md#open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort)

For an original worked example, take $n=7$ complete [sorting records](#sorting-record) and $K=4$ possible [integer](integer.md) [sort keys](#sort-key):

$$
A=\bigl((2,\mathrm A),(0,\mathrm B),(2,\mathrm C),(1,\mathrm D),(0,\mathrm E),(3,\mathrm F),(2,\mathrm G)\bigr).
$$

The letters label the associated data, and are never compared. Both [input](theoretical-computer-science.md#input-computer-science) and [output](theoretical-computer-science.md#output-computing) [array indices](data-structure.md#array-index) start at zero, so their valid positions are $0,\ldots,6$; the count [array](data-structure.md#array-data-structure) has [array indices](data-structure.md#array-index) $0,\ldots,3$. [Stable sorting](#stable-sorting) must produce

$$
B=\bigl((0,\mathrm B),(0,\mathrm E),(1,\mathrm D),(2,\mathrm A),(2,\mathrm C),(2,\mathrm G),(3,\mathrm F)\bigr).
$$

The equal-[sort key](#sort-key) groups retain $\mathrm B,\mathrm E$ and $\mathrm A,\mathrm C,\mathrm G$ in arrival order. [Counting sort prefix ranges](#counting-sort-prefix-ranges) explain where those groups belong; [stable record placement in counting sort](#stable-record-placement-in-counting-sort) explains how to fill them without losing that order or the complete [sorting records](#sorting-record).

#### Counting sort prefix ranges

↑ **Parent:** [Counting sort](#counting-sort)

For $n\geq0$ [sorting records](#sorting-record) with [integer](integer.md) [sort keys](#sort-key) in $\{0,\ldots,K-1\}$, where $K\geq1$, let $c_k$ count the [input](theoretical-computer-science.md#input-computer-science) occurrences of [sort key](#sort-key) $k$. Define two [prefix sums](arithmetic.md#prefix-sum):

$$
S_k=\sum_{h=0}^{k-1}c_h,\qquad P_k=\sum_{h=0}^{k}c_h=S_k+c_k.
$$

The [empty sum](arithmetic.md#empty-sum) gives $S_0=0$. Here $c_k,S_k,P_k$ are counts of [sorting records](#sorting-record). Exactly $S_k$ [sorting records](#sorting-record) have smaller [sort keys](#sort-key), so the [output](theoretical-computer-science.md#output-computing) positions for [sort key](#sort-key) $k$ form the half-open [integer interval](integer.md#integer-interval)

$$
\{j\in\mathbb Z:S_k\leq j<P_k\}=[S_k,P_k)\cap\mathbb Z.
$$

Its right endpoint $P_k$ is excluded: the last occupied [array index](data-structure.md#array-index) is $P_k-1$ when $c_k>0$.[Open Data Structures: An Introduction by Pat Morin; §11.2.1 Counting Sort, paragraphs after Figure 11.7: running sums count keys at most k and determine the output block](computer-science-bibliography.md#open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort)

For the seven-[sorting record](#sorting-record) example, the frequency [array](data-structure.md#array-data-structure), inclusive cumulative count [array](data-structure.md#array-data-structure), and start [array](data-structure.md#array-data-structure) are

$$
c=(2,1,3,1),\qquad P=(2,3,6,7),\qquad S=(0,2,3,6).
$$

Thus [sort keys](#sort-key) zero, one, two and three occupy the [integer intervals](integer.md#integer-interval) $[0,2)$, $[2,3)$, $[3,6)$ and $[6,7)$, respectively. In particular, the three [sorting records](#sorting-record) with [sort key](#sort-key) two belong at [array indices](data-structure.md#array-index) three, four and five. The inclusive cumulative count $P_2=6$ counts all six [sorting records](#sorting-record) with [sort keys](#sort-key) at most two; six is the exclusive endpoint, not the final position of a [sorting record](#sorting-record) with [sort key](#sort-key) two.

<a id="image-frequencies-and-prefix-sums-reserve-disjoint-counting-sort-output-ranges"></a>
![](counting-sort-frequency-prefix-ranges.png)

**[Figure 20](#image-frequencies-and-prefix-sums-reserve-disjoint-counting-sort-output-ranges). Frequencies and prefix sums reserve disjoint counting sort output ranges**. Original seven-[sorting record](#sorting-record) example with $K=4$. The bar heights count [sorting records](#sorting-record). The table gives the start $S_k$ and exclusive endpoint $P_k$ for each [sort key](#sort-key); the lower strip shows zero-based [output](theoretical-computer-science.md#output-computing) [array indices](data-structure.md#array-index). The boundary seven lies just beyond the last slot six.

These [integer intervals](integer.md#integer-interval) fit together because $P_k=S_{k+1}$ for $k<K-1$, and $P_{K-1}=n$. Their lengths $P_k-S_k=c_k$ add to $n$, so they partition all [output](theoretical-computer-science.md#output-computing) positions without overlaps or gaps. An absent [sort key](#sort-key) contributes an empty [integer interval](integer.md#integer-interval): with frequencies $(0,2,0,1)$, the endpoints are $(0,2,2,3)$ and [sort key](#sort-key) two has range $[2,2)$. For empty [input](theoretical-computer-science.md#input-computer-science), every count and endpoint is zero; every reserved [integer interval](integer.md#integer-interval) is empty. This makes the same formulas cover missing [sort keys](#sort-key) and the empty case.

#### Stable record placement in counting sort

↑ **Parent:** [Counting sort](#counting-sort)

Initialize a mutable endpoint [array](data-structure.md#array-data-structure) $E$ to the inclusive cumulative counts $P$. Scan [input](theoretical-computer-science.md#input-computer-science) [array indices](data-structure.md#array-index) $i=n-1,n-2,\ldots,0$. For each complete [sorting record](#sorting-record) $A_i$ with [sort key](#sort-key) $k$, first decrement $E_k$, then write $A_i$ at [output](theoretical-computer-science.md#output-computing) [array index](data-structure.md#array-index) $E_k$. This is equivalent to writing at the old endpoint minus one and then decrementing the endpoint.[Open Data Structures: An Introduction by Pat Morin; §11.2.1 Counting Sort, final scan paragraph and stability paragraph after Theorem 11.7](computer-science-bibliography.md#open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort)

In the worked example, the first [input](theoretical-computer-science.md#input-computer-science) [sorting record](#sorting-record) read is $(2,\mathrm G)$ at [array index](data-structure.md#array-index) six. Its endpoint changes from $E_2=6$ to $E_2=5$, so the complete [sorting record](#sorting-record) goes to $B_5$. Next, $(3,\mathrm F)$ changes $E_3$ from seven to six and goes to $B_6$. Writing before the decrement at the old endpoint would put $\mathrm G$ outside its reserved [integer interval](integer.md#integer-interval) and try to put $\mathrm F$ beyond the [output](theoretical-computer-science.md#output-computing) [array](data-structure.md#array-data-structure). All seven writes are:

$$
\begin{array}{c|c|c|c|c}
\text{step}&\text{input index }i&A_i& E_k\text{ before}\to\text{after}&\text{output index}\\\hline
1&6&(2,\mathrm G)&6\to5&5\\
2&5&(3,\mathrm F)&7\to6&6\\
3&4&(0,\mathrm E)&2\to1&1\\
4&3&(1,\mathrm D)&3\to2&2\\
5&2&(2,\mathrm C)&5\to4&4\\
6&1&(0,\mathrm B)&1\to0&0\\
7&0&(2,\mathrm A)&4\to3&3
\end{array}
$$

Each endpoint changes only when a [sorting record](#sorting-record) with its own [sort key](#sort-key) is placed. Consequently, $E_2$ stays at five through the placements of $\mathrm F,\mathrm E,\mathrm D$ before dropping to four for $\mathrm C$.

<a id="image-a-backward-input-scan-gives-forward-order-among-equal-sort-keys"></a>
![](counting-sort-reverse-stable-placement.png)

**[Figure 21](#image-a-backward-input-scan-gives-forward-order-among-equal-sort-keys). A backward input scan gives forward order among equal sort keys**. Original complete trace of the seven-[sorting record](#sorting-record) example. Each row shows the endpoint decrement and resulting [output](theoretical-computer-science.md#output-computing) [array](data-structure.md#array-data-structure); the newly written complete [sorting record](#sorting-record) is dark. Both [input](theoretical-computer-science.md#input-computer-science) and [output](theoretical-computer-science.md#output-computing) [array indices](data-structure.md#array-index) start at zero. The final order is $\mathrm B,\mathrm E,\mathrm D,\mathrm A,\mathrm C,\mathrm G,\mathrm F$.

Here is a complete implementation under the stated [input](theoretical-computer-science.md#input-computer-science) contract; each [sorting record](#sorting-record) is a pair whose first component is its [integer](integer.md) [sort key](#sort-key):

```
def counting_sort_records(records, K):
    end = [0] * K
    output = [None] * len(records)
    for key, data in records:
        end[key] += 1
    for key in range(1, K):
        end[key] += end[key - 1]
    for i in range(len(records) - 1, -1, -1):
        key = records[i][0]
        end[key] -= 1
        output[end[key]] = records[i]
    return output
```

The same [array](data-structure.md#array-data-structure) `end` successively stores frequencies, inclusive cumulative counts, and moving exclusive endpoints; the formulas $c,S,P$ describe their mathematical values without requiring three stored [arrays](data-structure.md#array-data-structure). The write copies the complete [sorting record](#sorting-record), including its associated data. In particular, two occurrences of an identical pair still cause two separate writes.

For a short [algorithm correctness](#algorithm-correctness) proof, let $r_k$ be the number of already placed [sorting records](#sorting-record) with [sort key](#sort-key) $k$. A [loop invariant](#loop-invariant) is

$$
E_k=P_k-r_k,\qquad [S_k,E_k)\text{ is unfilled},\qquad [E_k,P_k)\text{ is filled}.
$$

All [integer intervals](integer.md#integer-interval) here mean [output](theoretical-computer-science.md#output-computing) [array indices](data-structure.md#array-index). Initially $r_k=0$, so each whole reserved [integer interval](integer.md#integer-interval) is unfilled. When the next [sorting record](#sorting-record) has [sort key](#sort-key) $k$, fewer than $c_k$ such occurrences have been placed, giving $E_k>S_k$. Decrementing selects a fresh slot inside its reserved [integer interval](integer.md#integer-interval). At termination, $r_k=c_k$ and $E_k=S_k$: every [output](theoretical-computer-science.md#output-computing) slot has been filled exactly once with a complete [input](theoretical-computer-science.md#input-computer-science) occurrence. The disjoint, increasing [sort key](#sort-key) ranges establish [sortedness](#sortedness), while the fresh-slot property establishes [sorting permutation preservation](#sorting-permutation-preservation).

For [stable sorting](#stable-sorting), take two [input](theoretical-computer-science.md#input-computer-science) occurrences with equal [sort keys](#sort-key) at [array indices](data-structure.md#array-index) $i<j$. The backward scan visits $j$ first and puts it farther right in their shared [integer interval](integer.md#integer-interval). When $i$ is visited, the endpoint has decreased at least once, so its [output](theoretical-computer-science.md#output-computing) position is smaller. Thus their original order survives. A forward scan with this same decrement rule reverses every equal-[sort key](#sort-key) group: it would put $\mathrm A,\mathrm C,\mathrm G$ at positions five, four, three. A forward scan can instead be stable if it starts from $S_k$ and fills each [integer interval](integer.md#integer-interval) left to right, incrementing after each write. The scan direction and endpoint convention must agree.

Count initialization takes $K$ writes, [output](theoretical-computer-science.md#output-computing) initialization takes $n$ writes, counting takes $n$ updates, the [prefix sum](arithmetic.md#prefix-sum) pass takes $K-1$ updates, and placement takes $n$ writes. Hence [time complexity](theoretical-computer-science.md#time-complexity) and auxiliary storage are $O(n+K)$ in [Big O notation](real-analysis.md#big-o-notation), assuming constant-cost [sort key](#sort-key) access, [integer](integer.md) arithmetic, [array](data-structure.md#array-data-structure) indexing and complete [sorting record](#sorting-record) movement. Large records can instead be represented by constant-size references.[Open Data Structures: An Introduction by Pat Morin; §11.2.1 Counting Sort, auxiliary counter and output arrays, loop-cost discussion and Theorem 11.7](computer-science-bibliography.md#open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort)

For example, three [sorting records](#sorting-record) with [sort keys](#sort-key) zero, $999999$ and zero require one million counters if $K=1000000$; unused [sort keys](#sort-key) still incur initialization and [prefix sum](arithmetic.md#prefix-sum) work. The bound is therefore linear in the [input](theoretical-computer-science.md#input-computer-science) length only when $K=O(n)$. Empty [input](theoretical-computer-science.md#input-computer-science) skips the record scans, but this implementation still initializes $K$ counters and accumulates their [prefix sums](arithmetic.md#prefix-sum). For nonempty [input](theoretical-computer-science.md#input-computer-science), counting all $n$ records and filling their ranges gives a concrete termination argument.

Direct [sort key](#sort-key) indexing is a different operation from a binary comparison. The [comparison sorting lower bound](#comparison-sorting-lower-bound) concerns [comparison sorts](#comparison-sort); [counting sort](#counting-sort) uses its restricted [integer](integer.md) [sort keys](#sort-key) as [array indices](data-structure.md#array-index). Its small-$K$ speed is particularly useful for categorical numerical labels and for each [stable sorting](#stable-sorting) pass of [radix sort](#radix-sort): the reserved [integer intervals](integer.md#integer-interval) turn group sizes into exact destinations.

### Radix sort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radix_sort)

[Radix sort](#radix-sort) sorts encoded [sort keys](#sort-key) a digit at a time. Its least-significant-digit version uses [stable sorting](#stable-sorting) on each successive digit, often by [counting sort](#counting-sort). For $d$ digits with $R$ possible values each, it takes $O(d(n+R))$ [time complexity](theoretical-computer-science.md#time-complexity) in [Big O notation](real-analysis.md#big-o-notation), assuming constant-cost digit extraction and indexing. [Stable sorting](#stable-sorting) retains the ordering established by earlier digits when a later digit ties. Both digit access and the direct indexing in [counting sort](#counting-sort) lie outside the [comparison sort](#comparison-sort) model, so these bounds do not contradict the [comparison sorting lower bound](#comparison-sorting-lower-bound).[Open Data Structures: An Introduction by Pat Morin; Theorem 11.8](computer-science-bibliography.md#open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort)

#### Least-significant-digit radix sort

↑ **Parent:** [Radix sort](#radix-sort)

A least-significant-digit radix sort processes [numerical digits](integer.md#numerical-digit) from smallest to largest [place value](integer.md#place-value). Fix [integers](integer.md) $R\ge2$ and $d\ge1$, and take $n$ complete [sorting records](#sorting-record) whose [sort keys](#sort-key) satisfy $0\le k<R^d$. Use exactly $d$ positions in [positional notation](integer.md#positional-notation) with [radix](integer.md#radix) $R$, including leading zeros. At pass $j=0,\ldots,d-1$, apply a [stable digit sort](#stable-digit-sort) to the current [array](data-structure.md#array-data-structure) using

$$
\delta_j(k)=\left\lfloor\frac{k}{R^j}\right\rfloor\bmod R.
$$

The [floor function](calculus.md#floor-function) selects the integer [quotient](arithmetic.md#quotient), and the [remainder](integer.md#remainder) selects the current [numerical digit](integer.md#numerical-digit). Move the complete [sorting record](#sorting-record), including its associated data. There are exactly $d$ passes, so this procedure terminates even for an empty [array](data-structure.md#array-data-structure). The [radix sort suffix invariant](#radix-sort-suffix-invariant) supplies its [algorithm correctness](#algorithm-correctness) argument.

For an original [input](theoretical-computer-science.md#input-computer-science), let the letters identify the attached data:

$$
(314_A,027_B,305_C,042_D,217_E,005_F,127_G,040_H).
$$

Here $R=10$, $d=3$, and leading zeros only align [place values](integer.md#place-value); $005$ represents the [integer](integer.md) five. The exact pass ledger is:

$$
\begin{array}{c|llllllll}
\text{input}&314_A&027_B&305_C&042_D&217_E&005_F&127_G&040_H\\
\text{units}&040_H&042_D&314_A&305_C&005_F&027_B&217_E&127_G\\
\text{tens}&305_C&005_F&314_A&217_E&027_B&127_G&040_H&042_D\\
\text{hundreds}&005_F&027_B&040_H&042_D&127_G&217_E&305_C&314_A
\end{array}
$$

After the units pass, the [numerical digits](integer.md#numerical-digit) are $0,2,4,5,5,7,7,7$. The ties retain $C$ before $F$ and $B$ before $E$ before $G$. This [array](data-structure.md#array-data-structure) is not yet ordered by its whole [integer](integer.md) [sort keys](#sort-key): $314$ still precedes $305$. After the tens pass, the two-position suffixes are $05,05,14,17,27,27,40,42$. In particular, $217_E$ now precedes $027_B$: their tens [numerical digits](integer.md#numerical-digit) differ, so [stable sorting](#stable-sorting) does not require retaining their previous order. The hundreds pass produces the final [sorted array](data-structure.md#sorted-array), with all attached letters preserved.

<a id="image-three-stable-digit-passes-order-successively-longer-suffixes"></a>
![](radix-sort-stable-digit-pass-ledger.png)

**[Figure 22](#image-three-stable-digit-passes-order-successively-longer-suffixes). Three stable digit passes order successively longer suffixes**. Original decimal [radix sort](#radix-sort) ledger. Each card carries an unchanged record label. Orange marks the [numerical digit](integer.md#numerical-digit) read in the current pass; green marks lower positions already processed. The suffix row beneath each pass shows precisely what is ordered, rather than claiming whole-key [sortedness](#sortedness) early.

##### Radix sort suffix invariant

↑ **Parent:** [Least-significant-digit radix sort](#least-significant-digit-radix-sort)

After $p$ passes, $0\le p\le d$, the [array](data-structure.md#array-data-structure) is in nondecreasing order of $s_p(k)=k\bmod R^p$, the [integer](integer.md) represented by its $p$ lowest [numerical digits](integer.md#numerical-digit). Equivalently it is ordered by the [tuple](set-theory.md#finite-tuple) $(\delta_{p-1}(k),\ldots,\delta_0(k))$ under [lexicographic order](extremal-set-theory.md#lexicographic-order), with the most significant processed [numerical digit](integer.md#numerical-digit) first. Among equal suffixes it retains the original order of the complete [sorting records](#sorting-record).

The [loop invariant](#loop-invariant) has a simple [mathematical induction](foundations-of-mathematics.md#mathematical-induction) proof. Before any pass, $s_0(k)=k\bmod1=0$ for every [sort key](#sort-key), so the original [array](data-structure.md#array-data-structure) satisfies it. Suppose it holds after $p$ passes. The next [stable digit sort](#stable-digit-sort) puts smaller $\delta_p$ groups first and preserves the existing $s_p$ order within each tie. Since

$$
s_{p+1}(k)=R^p\delta_p(k)+s_p(k),\qquad 0\le s_p(k)<R^p,
$$

the new [array](data-structure.md#array-data-structure) is ordered by $s_{p+1}$. Equal new suffixes have equal current [numerical digits](integer.md#numerical-digit) and equal old suffixes, so their original order is also preserved. Every pass is a [permutation](combinatorics.md#permutation) of complete [sorting records](#sorting-record), establishing [sorting permutation preservation](#sorting-permutation-preservation). At termination $p=d$, the assumption $k<R^d$ gives $s_d(k)=k$: the invariant becomes whole-key [sortedness](#sortedness), together with [stable sorting](#stable-sorting).

#### Stable digit sort

↑ **Parent:** [Radix sort](#radix-sort)

A [stable digit sort](#stable-digit-sort) applies [stable sorting](#stable-sorting) to complete [sorting records](#sorting-record) using one specified [numerical digit](integer.md#numerical-digit) of their encoded [sort keys](#sort-key). [Counting sort](#counting-sort) can supply it; [stable record placement in counting sort](#stable-record-placement-in-counting-sort) moves records without discarding their associated data. Stability concerns equal current [numerical digits](integer.md#numerical-digit), even when the full [sort keys](#sort-key) differ. This is the information-preservation step in [least-significant-digit radix sort](#least-significant-digit-radix-sort).[Open Data Structures: An Introduction by Pat Morin; §11.2.1, associated-data and stability paragraphs; §11.2.2, least-significant passes and correctness paragraph after Figure 11.8](computer-science-bibliography.md#open-data-structures-an-introduction-by-pat-morin/11-2-counting-sort-and-radix-sort)

An original two-record counterexample exposes the need for the tie rule. Start with $(42_A,41_B)$ at width three. A units pass gives $(041_B,042_A)$. Both tens [numerical digits](integer.md#numerical-digit) are four. A deliberately unstable tens pass may reverse their tie and return $(042_A,041_B)$: it is sorted by the tens [numerical digit](integer.md#numerical-digit), yet its two-position suffixes $42,41$ are decreasing. The final stable hundreds pass sees two zeros and keeps this wrong order. [Sorting permutation preservation](#sorting-permutation-preservation) still holds, but [sortedness](#sortedness) fails. Stability in the tens pass would have retained the units information.

With [counting sort](#counting-sort) as the [stable digit sort](#stable-digit-sort), each pass initializes $R$ counters, counts $n$ current [numerical digits](integer.md#numerical-digit), constructs their [prefix sums](arithmetic.md#prefix-sum), and places $n$ complete [sorting records](#sorting-record). Thus each pass costs $O(n+R)$, and $d$ passes cost $O(d(n+R))$ in [Big O notation](real-analysis.md#big-o-notation). Reuse the counters and two [arrays](data-structure.md#array-data-structure) of record references between passes: auxiliary [space complexity](theoretical-computer-science.md#space-complexity) is $O(n+R)$, rather than $O(d(n+R))$. Assume constant-cost [numerical digit](integer.md#numerical-digit) extraction, counter [arithmetic](arithmetic.md), [array](data-structure.md#array-data-structure) indexing and record-reference movement; the bound counts these operations, not the cost of copying arbitrarily large payloads or performing arbitrary-precision [integer arithmetic](arithmetic.md#integer-arithmetic).

The benefit is avoiding a counter for every possible whole [sort key](#sort-key): width $d$ has $R^d$ possibilities, while each pass needs only $R$ counters. A larger [radix](integer.md#radix) reduces the number of passes for a fixed key range but enlarges the counter [array](data-structure.md#array-data-structure). The [comparison sorting lower bound](#comparison-sorting-lower-bound) does not apply to these direct [array indices](data-structure.md#array-index); they reveal more than a two-way comparison. Nor does fixing $R$ make $d$ disappear: growing key width still increases work.

#### Radix sort key encoding

↑ **Parent:** [Radix sort](#radix-sort)

An encoding for [radix sort](#radix-sort) must make the intended [total order](set.md#total-order) of [sort keys](#sort-key) agree with the [lexicographic order](extremal-set-theory.md#lexicographic-order) of its fixed-width [numerical digit](integer.md#numerical-digit) [tuples](set-theory.md#finite-tuple). The [positional notation](integer.md#positional-notation) for bounded nonnegative [integers](integer.md) has this property. At the most significant differing position $m$, a one-unit [numerical digit](integer.md#numerical-digit) difference contributes $R^m$, while all lower positions together contribute at most

$$
(R-1)\sum_{j=0}^{m-1}R^j=R^m-1.
$$

This [geometric series](sequence-and-series.md#geometric-series) shows why lower [numerical digits](integer.md#numerical-digit) cannot reverse that comparison. Leading zero padding works here because it preserves [place values](integer.md#place-value) and the represented [integer](integer.md).

For signed [integers](integer.md) in a known [integer interval](integer.md#integer-interval) $L\le x\le U$, encode $e(x)=x-L$ and choose $d$ with $U-L<R^d$. This [order-preserving function](set.md#order-preserving-function) is also [injective](algebra.md#injective-function): $x<y$ exactly when $e(x)<e(y)$. For $-8\le x\le7$, the four-[bit](information-theory.md#bit) encodings of $-8,-3,-1,0,4,7$ are $0000,0101,0111,1000,1100,1111$ after adding eight. Restore the original signed [sort keys](#sort-key) when displaying the complete [sorting records](#sorting-record); the encoding need not replace their data. Sorting the unsigned values of raw [two's complement](programming-language.md#two-s-complement) [bit](information-theory.md#bit) patterns would put nonnegative [integers](integer.md) before negative ones, so their representation alone is not this ordered encoding.

For variable-length [strings](foundations-of-mathematics.md#string), first specify the [alphabet](information-theory.md#alphabet) order and whether a proper prefix precedes its extensions. As an original construction, use $a<b$, let every [string](foundations-of-mathematics.md#string) have length at most three, encode $a$ as one and $b$ as two, and append zeros to width three. Zero is reserved for an end marker strictly below every real symbol. The [strings](foundations-of-mathematics.md#string) $\varepsilon,a,aa,ab,b$ encode as $000,100,110,120,200$ in [radix](integer.md#radix) three, which preserves their [lexicographic order](extremal-set-theory.md#lexicographic-order). A differing real symbol decides the comparison; at a prefix boundary, the shorter [string](foundations-of-mathematics.md#string)'s zero comes before the extension's one or two. Left padding would instead encode $b$ as $002$ and $aa$ as $011$, reversing $aa<b$. Padding raw [bytes](computer-memory.md#byte) with zero also fails if zero is an allowed data symbol: distinct [strings](foundations-of-mathematics.md#string) can then receive the same encoding. A reserved end marker and an explicit symbol ordering are essential; byte order alone does not establish a desired human text order.

<a id="image-stable-ties-preserve-lower-digits-suitable-encodings-preserve-the-intended-order"></a>
![](radix-sort-stability-and-key-encoding.png)

**[Figure 23](#image-stable-ties-preserve-lower-digits-suitable-encodings-preserve-the-intended-order). Stable ties preserve lower digits; suitable encodings preserve the intended order**. Original counterexample above: reversing a tens tie destroys the units order and a later stable hundreds pass cannot repair it. Below: signed [integer](integer.md) offsets and a reserved end marker for bounded [strings](foundations-of-mathematics.md#string) produce increasing fixed-width encodings. All entries are exact constructed examples.

### Stable sorting

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)

[Stable sorting](#stable-sorting) preserves the original relative order of entries with equal keys. The entries may carry different names or other information even when their keys coincide. For example, sorting records $(2,\mathrm{Ada}),(1,\mathrm{Bo}),(2,\mathrm{Cy})$ by the numerical key gives $(1,\mathrm{Bo}),(2,\mathrm{Ada}),(2,\mathrm{Cy})$: Ada remains before Cy. This is useful when a previous ordering contains information worth retaining, such as arrival order among equally ranked requests.

### Merge sort

↑ **Parent:** [Sorting algorithm](#sorting-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Merge_sort)

[Merge sort](#merge-sort) is a [divide-and-conquer algorithm](#divide-and-conquer-algorithm) that sorts a finite [array](data-structure.md#array-data-structure) by splitting it into contiguous halves, sorting each half using [recursion](#recursion-computer-science), and combining the two [sorted arrays](data-structure.md#sorted-array) with the [merge algorithm](#merge-algorithm). An empty or one-entry [array](data-structure.md#array-data-structure) is returned immediately. For length $n\geq2$, put the first $\lfloor n/2\rfloor$ entries on the left and the remaining $\lceil n/2\rceil$ on the right; the brackets are the [floor function](calculus.md#floor-function) and [ceiling function](calculus.md#ceiling-function). Always choose the left head on equal keys to obtain [stable sorting](#stable-sorting). This is the split, sort, combine structure taught in the MIT lecture notes.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; MIT 6.006 (2011), lecture 3: merge sort](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-3-insertion-sort-merge-sort)

Take the concrete [input](theoretical-computer-science.md#input-computer-science) [array](data-structure.md#array-data-structure)

$$
A=(7,2_a,5,2_b,9,1,4,3).
$$

The tags identify the entries originally at indices $1$ and $3$, counting from zero. Both keys are $2$; the tags are never compared. Reading downward in the figure follows the splits, then the returned [sorted arrays](data-structure.md#sorted-array). Arrows show dependencies; the level layout groups independent calls rather than giving their chronological execution order.

<a id="image-merge-sort-splits-into-base-cases-and-returns-sorted-arrays"></a>
![](merge-sort-split-and-merge.png)

**[Figure 24](#image-merge-sort-splits-into-base-cases-and-returns-sorted-arrays). Merge sort splits into base cases and returns sorted arrays**. The tagged keys 2a and 2b retain their original order through [stable sorting](#stable-sorting). The [merge algorithm](#merge-algorithm) makes 4, 6 and 7 head comparisons on the three returning levels, for 17 in total.

The first two halves are $(7,2_a,5,2_b)$ and $(9,1,4,3)$. Their pairs split into one-entry base cases. Applying the [merge algorithm](#merge-algorithm) gives the following fully worked return levels; each number in the last column counts only comparisons between two available heads.

| Returning level | Resulting [sorted arrays](data-structure.md#sorted-array) | Head comparisons |
| --- | --- | --- |
| Pairs | $(2_a,7)$, $(2_b,5)$, $(1,9)$, $(3,4)$ | $1+1+1+1=4$ |
| Halves | $(2_a,2_b,5,7)$, $(1,3,4,9)$ | $3+3=6$ |
| Whole [array](data-structure.md#array-data-structure) | $(1,2_a,2_b,3,4,5,7,9)$ | $7$ |

In the left-half [merge algorithm](#merge-algorithm), the head pairs are $(2_a,2_b)$, $(7,2_b)$ and $(7,5)$; it takes $2_a,2_b,5$, then appends $7$. In the final [merge algorithm](#merge-algorithm), the head pairs are $(2_a,1)$, $(2_a,3)$, $(2_b,3)$, $(5,3)$, $(5,4)$, $(5,9)$ and $(7,9)$. It takes $1,2_a,2_b,3,4,5,7$, then appends $9$. Thus this precise version makes $4+6+7=17$ head comparisons and, ignoring identity tags, returns $(1,2,2,3,4,5,7,9)$.

The elegance of [merge sort](#merge-sort) is that it creates exactly the structure its next step needs: two smaller [sorted arrays](data-structure.md#sorted-array) make the larger ordering inexpensive. Once the whole [array](data-structure.md#array-data-structure) is sorted, equal keys are adjacent and [binary search](#binary-search) can serve repeated queries. [Stable sorting](#stable-sorting) also retains information that the keys alone do not express. If the left-half [merge algorithm](#merge-algorithm) instead takes the right head on the $2_a=2_b$ tie, it returns $(2_b,2_a,5,7)$; the keys are sorted but [stable sorting](#stable-sorting) has failed.

For [time complexity](theoretical-computer-science.md#time-complexity), assume each key comparison, entry access and entry copy has constant cost. The [merge algorithm](#merge-algorithm) processes $n$ entries in $O(n)$ time. In [Big O notation](real-analysis.md#big-o-notation), the resulting [recurrence relation](sequence-and-series.md#recurrence-relation) is

$$
T(0),T(1)=O(1),\qquad T(n)=T(\lfloor n/2\rfloor)+T(\lceil n/2\rceil)+O(n)\quad(n\geq2).
$$

For $n=2^k$, the balanced levels contain $n$ entries each and there are $k=\log_2 n$ returning levels. Each costs $O(n)$, so the worst-case [time complexity](theoretical-computer-science.md#time-complexity) is $O(n\log n)$. For arbitrary $n$, there are at most $\lceil\log_2 n\rceil$ returning levels, each processing at most $n$ entries, giving the same bound. The worst-case number of head comparisons is also $O(n\log n)$. Here $\log_2$ is the base-two [logarithm](calculus.md#logarithm). The MIT notes give this level-by-level analysis for [merge sort](#merge-sort).[MIT 6.006 (2020), lecture 3, page 5: merge sort analysis](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/6d1ae5278d02bbecb5c4428928b24194_MIT6_006S20_lec3.pdf)

The conventional [array](data-structure.md#array-data-structure) implementation uses a reusable buffer of $n$ entries for the [merge algorithm](#merge-algorithm), together with $O(\log n)$ pending calls for [recursion](#recursion-computer-science). Its auxiliary [space complexity](theoretical-computer-science.md#space-complexity) is therefore $O(n)$, beyond the original [array](data-structure.md#array-data-structure). This bound describes that implementation. A [linked list](data-structure.md#linked-list) permits a [merge algorithm](#merge-algorithm) that reconnects existing nodes; its storage accounting differs from copying [array](data-structure.md#array-data-structure) entries into a buffer.

For a short [algorithm correctness](#algorithm-correctness) outline, the empty and one-entry base cases are sorted. Assuming [recursion](#recursion-computer-science) correctly sorts both shorter halves, the [merge algorithm](#merge-algorithm) returns all their entries in order. Equal keys within a half keep their relative order by the same argument applied to the smaller call; across halves, every left entry originally preceded every right entry, so taking left first preserves [stable sorting](#stable-sorting). Both half-lengths decrease for $n\geq2$, establishing termination.

#### FIFO natural merge sort workspace bound

↑ **Parent:** [Merge sort](#merge-sort)

Repeatedly removing the first two [maximal initial runs](#maximal-initial-run) and appending their sorted merge uses $\Theta(n\log n)$ total fresh output cells in the worst case if obsolete cells are never reused. Group merges into rounds that consume the runs present at the start: the run count is at least halved up to rounding, and each round writes at most $2n$ values. A tight-order family consists of $2^h$ copies of $[0,1]$: run boundaries never coalesce and every merging level writes $n=2^{h+1}$ entries. Its final append-only endpoint is exactly $n\log_2 n$.

#### Sorted run

↑ **Parent:** [Merge sort](#merge-sort)

A contiguous nondecreasing segment of a [sequence](sequence-and-series.md#sequence). Adjacent [sorted runs](#sorted-run) can be merged in time linear in their combined lengths.

##### Maximal initial run

↑ **Parent:** [Sorted run](#sorted-run)

The longest nondecreasing prefix of a specified segment. For a nonempty segment $u[a..b)$, its endpoint is the first $c$ with $a<c<b$ and $u[c-1]>u[c]$, or $b$ if no such descent exists. Scanning adjacent pairs takes time proportional to the returned run length. An empty segment has an empty [maximal initial run](#maximal-initial-run).

## Merge algorithm

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Merge_algorithm)

The [merge algorithm](#merge-algorithm) combines two finite sorted [sequences](sequence-and-series.md#sequence) under the same [total order](set.md#total-order), retaining every entry exactly once. Keep a position at the first unconsumed entry, or "head", of each [input](theoretical-computer-science.md#input-computer-science). While both heads exist, compare their keys, append the smaller head to the [output](theoretical-computer-science.md#output-computing), and advance only that head's position. On equality take the left head. Once either [sequence](sequence-and-series.md#sequence) is exhausted, append the other remainder without further key comparisons. Empty [inputs](theoretical-computer-science.md#input-computer-science) therefore require no head comparisons. The MIT notes illustrate this two-head combination step.[6.006 Introduction to Algorithms, Fall 2011 by Massachusetts Institute of Technology, 6.006 course staff; MIT 6.006 (2011), lecture 3: merging sorted arrays](computer-science-bibliography.md#6-006-introduction-to-algorithms-fall-2011-by-massachusetts-institute-of-technology-6-006-course-staff/lecture-3-insertion-sort-merge-sort)

For example, the [merge algorithm](#merge-algorithm) applied to $(1,4,7)$ and $(2,3,8,9)$ returns $(1,2,3,4,7,8,9)$:

<a id="image-five-head-comparisons-in-the-merge-algorithm"></a>
![](merge-two-sorted-sequences.png)

**[Figure 25](#image-five-head-comparisons-in-the-merge-algorithm). Five head comparisons in the merge algorithm**. Orange heads are chosen and arrows lead to the next [output](theoretical-computer-science.md#output-computing) entry. The compared head pairs are (1,2), (4,2), (4,3), (4,8) and (7,8). The left [sequence](sequence-and-series.md#sequence) then runs out; append (8,9) without further key comparisons.

The head pairs $(1,2)$, $(4,2)$, $(4,3)$, $(4,8)$ and $(7,8)$ select $1,2,3,4,7$ respectively. After the fifth comparison the left [sequence](sequence-and-series.md#sequence) is empty, so $(8,9)$ is appended. Seven entries are written, but only five head comparisons occur: tests for exhaustion and appending the remainder are separate operations. This distinction makes the example's count smaller than the bound $3+4-1=6$.

For nonempty [inputs](theoretical-computer-science.md#input-computer-science) of lengths $m,n$, each head comparison consumes exactly one entry. After $m+n-1$ such removals at most one entry remains, so both heads cannot still exist. Hence the [merge algorithm](#merge-algorithm) uses at most $m+n-1$ head comparisons. The bound can be attained: $(1,3,5)$ and $(2,4,6,7)$ require six head comparisons before the left [sequence](sequence-and-series.md#sequence) is exhausted. With constant-cost comparisons, access and copying, writing all $m+n$ entries gives [time complexity](theoretical-computer-science.md#time-complexity) $O(m+n)$ in [Big O notation](real-analysis.md#big-o-notation). Writing a separate [output](theoretical-computer-science.md#output-computing) [array](data-structure.md#array-data-structure) needs $m+n$ entry slots; the two positions require only constant additional storage.

The [merge algorithm](#merge-algorithm) is useful whenever two already ordered collections must become one: it reads each [input](theoretical-computer-science.md#input-computer-science) only forwards. This works with [arrays](data-structure.md#array-data-structure) and [linked lists](data-structure.md#linked-list), without needing access to arbitrary middle positions. Choosing left on ties preserves each [input](theoretical-computer-science.md#input-computer-science)'s internal order and places equal left entries before equal right entries, which is the combination rule needed for [stable sorting](#stable-sorting) in [merge sort](#merge-sort).

The [loop invariant](#loop-invariant) behind [algorithm correctness](#algorithm-correctness) is that the emitted prefix is sorted, contains exactly the consumed entries, and every emitted key is at most every unconsumed key. Each sorted [sequence](sequence-and-series.md#sequence) has its smallest remaining key at its head, so the smaller of the two heads is safe to append. The invariant survives each removal; when one [sequence](sequence-and-series.md#sequence) ends, the other sorted remainder is safe to append in full. Each comparison removes an entry, so termination follows from the finite [input](theoretical-computer-science.md#input-computer-science) lengths.

// Target: computer-science.bigb

### In-place merge

↑ **Parent:** [Merge algorithm](#merge-algorithm)

Combining adjacent [sorted runs](#sorted-run) within their existing [array](data-structure.md#array-data-structure) segment. A simple constant-auxiliary-space version moves the smaller second-run head before the first-run head by shifting the intervening block one place right. The finished prefix is always a merge of the consumed portions. This can use quadratic [running time](#running-time); minimizing storage does not automatically preserve the linear cost of a disjoint-output merge.

### Locally finite sorted-stream merge

↑ **Parent:** [Merge algorithm](#merge-algorithm)

Compare the heads of two increasing [lazy lists](data-structure.md#lazy-list), emit the smaller and advance its input, or emit one copy and advance both when the heads are equal. This preserves strict order and removes duplicates. To enumerate the entire union as a [list](data-structure.md#list-abstract-data-type), each requested element must have finitely many smaller elements in the union. Without this condition, an increasing sequence tending to one can permanently precede an input element equal to two. For increasing [integer](integer.md) streams bounded below, finiteness below each candidate guarantees that no candidate is starved.

### K-way merge algorithm

↑ **Parent:** [Merge algorithm](#merge-algorithm)

## Binary search

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_search)

[Binary search](#binary-search) finds a target $x$ in a [sorted array](data-structure.md#sorted-array) $A$ by inspecting the middle of the remaining candidate range. If the middle entry is smaller than $x$, every entry to its left is also too small; if larger, every entry to its right is too large. One comparison therefore rules out many entries. Equal entries are allowed; this version returns any matching index, without promising the first occurrence.

Use indices starting at zero and inclusive endpoints $L,R$. Initially $L=0$, $R=n-1$, where $n$ is the [array](data-structure.md#array-data-structure) length. While $L\leq R$, choose

$$
m=L+\left\lfloor\frac{R-L}{2}\right\rfloor.
$$

The brackets denote the [floor function](calculus.md#floor-function). Compare $A_m$ with $x$: return $m$ on equality; set $L=m+1$ if $A_m<x$; otherwise set $R=m-1$. If $L>R$, report absence. The updates exclude the already inspected middle entry. This also handles an empty [array](data-structure.md#array-data-structure), whose initial endpoints are $0,-1$. Sedgewick and Wayne specify a [sorted array](data-structure.md#sorted-array) as [input](theoretical-computer-science.md#input-computer-science) and return a matching index or $-1$ for absence.[Sedgewick and Wayne: BinarySearch API](https://algs4.cs.princeton.edu/code/javadoc/edu/princeton/cs/algs4/BinarySearch.html)

For a fully worked example, take the [sorted array](data-structure.md#sorted-array)

$$
A=(2,5,8,12,16,23,38,56,72,91,104,130,160,205,260).
$$

Search for $x=23$:

| Step | Candidate indices | Middle index and value | Consequence |
| --- | --- | --- | --- |
| 1 | $0\ldots14$ | $m=7$, $A_7=56$ | $23<56$: retain $0\ldots6$. |
| 2 | $0\ldots6$ | $m=3$, $A_3=12$ | $23>12$: retain $4\ldots6$. |
| 3 | $4\ldots6$ | $m=5$, $A_5=23$ | Return index $5$. |

For $x=24$, the first two steps agree. Next $24>23$ retains only index $6$; inspecting $A_6=38$ sets $R=5$. Now $L=6>5=R$, so the answer is "absent" after four comparisons.

<a id="image-binary-search-retains-only-candidates-compatible-with-every-comparison"></a>
![](binary-search-intervals.png)

**[Figure 26](#image-binary-search-retains-only-candidates-compatible-with-every-comparison). Binary search retains only candidates compatible with every comparison**. Blue cells are current candidates, orange marks the middle entry, and green marks a match. Both searches use the same fifteen-entry sorted array.

The [loop invariant](#loop-invariant) is: the [array](data-structure.md#array-data-structure) stays sorted, $0\leq L\leq R+1\leq n$, and every index containing $x$ lies between $L$ and $R$. It holds initially. The [sorted array](data-structure.md#sorted-array) property justifies each exclusion. Returning on equality gives a match; an empty candidate range implies absence. Crucially, this [loop invariant](#loop-invariant) allows $x$ to be absent from the beginning.

For a nonempty range of size $s=R-L+1$, an unsuccessful comparison leaves at most $\lfloor s/2\rfloor$ candidates. Thus sizes satisfy $s_k\leq\lfloor n/2^k\rfloor$ after $k$ unsuccessful comparisons. This proves termination and, for $n\geq1$, at most $\lfloor\log_2 n\rfloor+1$ middle-entry comparisons. The final singleton still needs inspection: $n=1$ requires one comparison, not zero. For $n=15$, the bound is four. This is the halving argument behind logarithmic [time complexity](theoretical-computer-science.md#time-complexity).[Princeton COS 126: binary search analysis](https://www.cs.princeton.edu/courses/archive/fall24/cos126/static/lectures/42Algorithms.pdf)

A [decision tree](theoretical-computer-science.md#decision-tree) with $q$ binary tests has at most $2^q$ leaves. Distinguishing $n$ possible matching positions therefore requires $q\geq\lceil\log_2 n\rceil$. This lower bound counts binary tests, whereas the bound above counts three-way comparisons.

### Lower-bound binary search invariant

↑ **Parent:** [Binary search](#binary-search)

In a nondecreasing [array](data-structure.md#array-data-structure), the first position whose entry is at least $x$ is found by maintaining a half-open unresolved interval $[l,h)$. Entries before $l$ are smaller than $x$; entries from $h$ onward are at least $x$. Initially $l=c_0,h=c_1$. At midpoint $m$, replace $l$ by $m+1$ if $A[m]<x$, and otherwise replace $h$ by $m$. [Monotonicity](calculus.md#monotonic-function) preserves the [loop invariant](#loop-invariant), and $h-l$ decreases. On exit $l=h$ is the first qualifying position, or $c_1$ if no such entry exists. Repeated values and endpoint cuts require no additional case.

### Minimum search in a rotated distinct array

↑ **Parent:** [Binary search](#binary-search)

In a nonempty rotation of a strictly increasing [array](data-structure.md#array-data-structure), keep an inclusive interval containing its minimum. Compare its midpoint with its right endpoint. If the midpoint is larger, the minimum lies strictly to the right of the midpoint; otherwise the midpoint-to-right segment is increasing and the minimum lies at or left of the midpoint. The interval at least halves until one index remains. The cyclic predecessor of this minimum holds the maximum, so both extrema are found with $O(\log n)$ comparisons. Distinctness makes the two-way comparison decisive.

### Equal-range search

↑ **Parent:** [Binary search](#binary-search)

Find both the [lower-bound search](#lower-bound-search) boundary $i$ and the [upper-bound search](#upper-bound-search) boundary $j$ of a key $x$ in a [sorted array](data-structure.md#sorted-array). Every entry in $[i,j)$ is at least and at most $x$, so all are equal to $x$. Values immediately outside this interval, when present, are strictly smaller or strictly larger; the interval is consequently maximal. An absent key gives $i=j$ at its insertion position. Two [binary searches](#binary-search) give total [time complexity](theoretical-computer-science.md#time-complexity) $O(\log(N+1))$ under constant-cost comparison and indexed access.

### Upper-bound search

↑ **Parent:** [Binary search](#binary-search)

For a [sorted array](data-structure.md#sorted-array) $a[0..N)$, find the unique boundary $p\in[0,N]$ with $a[0..p)\leq x<a[p..N)$. A [binary search](#binary-search) maintains $0\leq l\leq r\leq N$, an excluded prefix $a[0..l)\leq x$, and an excluded suffix $x<a[r..N)$. At an interior midpoint $m$, replace $l$ by $m+1$ when $a(m)\leq x$, and otherwise replace $r$ by $m$. [Sortedness](#sortedness) preserves the [loop invariant](#loop-invariant); the width $r-l$ is a decreasing [loop variant](#loop-variant). Termination at $l=r$ gives the boundary, including $p=0$ and $p=N$. The [time complexity](theoretical-computer-science.md#time-complexity) is $O(\log(N+1))$ with constant-cost comparisons and indexed access. Unlike searching for $x+1$, this formulation does not risk [integer overflow](programming-language.md#integer-overflow) at the largest representable key.

### Missing-value search by deficient value intervals

↑ **Parent:** [Binary search](#binary-search)

Suppose a candidate [integer interval](integer.md#integer-interval) contains $W$ possible values and an active [array](data-structure.md#array-data-structure) segment contains exactly all occurrences from that interval, with $m<W$ entries. The [pigeonhole principle](combinatorics.md#pigeonhole-principle) guarantees a missing value. Split the value interval into widths $W_L,W_R$ and use [array partitioning](#two-way-array-partition) to obtain occurrence counts $m_L,m_R$. If $m_L<W_L$, retain the left side. Otherwise $m_R=m-m_L<W-W_L=W_R$, so retain the right side. This works with duplicate entries because it needs only the inequality between occurrences and possible values.

Balancing the value widths gives $W_{i+1}\leq\lceil W_i/2\rceil$, while the active scan length remains less than $W_i$. The total work is bounded by a [geometric series](sequence-and-series.md#geometric-series) and logarithmic loop overhead, hence $O(W_0)$ [time complexity](theoretical-computer-science.md#time-complexity). On reaching width one, the retained occurrence count is zero, proving that the sole candidate is absent globally. This is a [binary search](#binary-search) over deficient value intervals, with local in-place [array partitioning](#two-way-array-partition), rather than repeated full-array scans.

### Average successful search in a perfect binary search tree

↑ **Parent:** [Binary search](#binary-search)

For $n=2^k-1$ distinct keys and a uniformly chosen present target, early-return [binary search](#binary-search) takes mean $k-1+k/n$ iterations. There are $2^d$ targets needing $d+1$ probes, so sum $(d+1)2^d$ over depths zero through $k-1$ and divide by $n$. A boundary search that always closes the interval takes exactly $k$ iterations. Their expected difference is $1-k/n<1$, even though an individual shallow target can save many probes.

### Descending boundary search

↑ **Parent:** [Binary search](#binary-search)

For a nonincreasing [array](data-structure.md#array-data-structure), maintain indices $0\leq a\leq b\leq n$ such that entries before $a$ exceed the target and entries from $b$ onward are at most the target. Probe the middle of the half-open interval. A value above the target advances $a$ past that index; otherwise [set](set.md) $b$ to that index. The interval length decreases geometrically. At termination the common boundary is the first possible match, so one guarded equality test decides presence even with duplicates.

### Sign-bracketing binary search

↑ **Parent:** [Binary search](#binary-search)

Suppose [integer](integer.md) endpoints satisfy $l<r$ and $f(l)\leq0<f(r)$. Repeatedly test an interior midpoint and replace the endpoint with its matching sign. The [loop invariant](#loop-invariant) is the ordered opposite-sign bracket. The positive [integer](integer.md) width is a [loop variant](#loop-variant), and at termination $r=l+1$. Thus an adjacent sign transition can be located in $O(\log(r-l))$ evaluations without assuming that $f$ is monotone. If $f$ extends continuously between the endpoints, the [intermediate value theorem](calculus.md#intermediate-value-theorem) associates the sign bracket with a zero. This is different from finding the first true position of a globally monotone predicate.

### Distinct-index two-sum by suffix lower bounds

↑ **Parent:** [Binary search](#binary-search)

For each candidate first index $i$ in a [sorted array](data-structure.md#sorted-array), use [lower-bound search](#lower-bound-search) for $t-a(i)$ only in the suffix starting at $i+1$. A matching result is automatically at a different position. The outer [loop invariant](#loop-invariant) excludes all solutions whose smaller index precedes $i$; an unsuccessful suffix search extends this exclusion by one. Exhaustion proves absence of any pair. Searching all suffixes gives $O(N\log(N+1))$ [running time](#running-time) and constant [auxiliary space](#auxiliary-space). Compute the complement in a sufficiently wide type to avoid [integer overflow](programming-language.md#integer-overflow) before comparison.

### Lower-bound search

↑ **Parent:** [Binary search](#binary-search)

For a nondecreasing [sorted array](data-structure.md#sorted-array) $a[0..N)$ and target $x$, find the unique position $p\in[0,N]$ such that every earlier value is below $x$ and every later value is at least $x$. Equivalently, $p=\min(\{i\in[0,N):a(i)\geq x\}\cup\{N\})$. Uniqueness follows because, if $p<q$ both satisfied the partition, $a(p)$ would have to be both at least $x$ and below $x$. A half-open search interval maintains an excluded prefix of smaller values and an excluded suffix of greater-or-equal values. Allowing the sentinel $N$ handles an empty array or a target beyond its last entry.

## Karatsuba multiplication

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Karatsuba_multiplication)

[Karatsuba multiplication](#karatsuba-multiplication) is a [divide-and-conquer algorithm](#divide-and-conquer-algorithm) for [multiplication](arithmetic.md#multiplication) of [integers](integer.md). Splitting each operand into two blocks seems to require four smaller products; the [Karatsuba three-product identity](#karatsuba-three-product-identity) recovers the two cross terms together from just three products. Repeating that saving through [recursion](#recursion-computer-science) changes the [time complexity](theoretical-computer-science.md#time-complexity) from quadratic to $O(n^{\log_2 3})$, where $n$ counts digits in a fixed [positional notation](integer.md#positional-notation). The exponent is about $1.585$: the benefit comes from the [algorithm](algorithm.md), even though each splitting step needs more [addition](arithmetic.md#addition) and [subtraction](arithmetic.md#subtraction).

The [Karatsuba worked multiplication](#karatsuba-worked-multiplication) below computes $1234\cdot5678=7{,}006{,}652$ using $12\cdot56$, $34\cdot78$, and $46\cdot134$. The last operand already shows why “half-size” needs care: [Karatsuba carry handling](#karatsuba-carry-handling) and [Karatsuba recursion termination](#karatsuba-recursion-termination) account for the extra digit. [Karatsuba digit-operation cost](#karatsuba-digit-operation-cost) states the operation model; [Karatsuba practical crossover](#karatsuba-practical-crossover) explains why the asymptotic saving alone does not select a useful threshold.

The original 1962 paper presents a [binary numeral system](integer.md#binary-numeral-system) automaton construction: its Theorem 2 and proof reduce [multiplication](arithmetic.md#multiplication) to taking [squares of numbers](arithmetic.md#square-of-a-number), then reduce a larger [square of a number](arithmetic.md#square-of-a-number) to three smaller [squares of numbers](arithmetic.md#square-of-a-number). Its footnote explicitly addresses the extra digit in a sum of halves. The sequential [time complexity](theoretical-computer-science.md#time-complexity) analysis below uses a different operation model from that paper's automaton size and depth bounds, including its [Boolean circuit](theoretical-computer-science.md#boolean-circuit) realization without feedback.[Karatsuba and Ofman, Multiplication of many-digital numbers by automatic computers, original Russian article, 1962, pp. 293–294: Theorem 2, its proof, and the footnote on p. 294](computer-science-bibliography.md#multiplication-of-many-digital-numbers-by-automatic-computers-by-a-karatsuba-and-yu-ofman)

### Karatsuba operand splitting

↑ **Parent:** [Karatsuba multiplication](#karatsuba-multiplication)

Fix an [integer](integer.md) base $B\geq2$. Let $x,y\geq0$ have at most $n$ digits in [positional notation](integer.md#positional-notation), treating zero as one digit. For $n>1$, set $m=\lceil n/2\rceil$ using the [ceiling function](calculus.md#ceiling-function), and $q=B^m$. [Euclidean division](integer.md#euclidean-division) gives

$$
a=\lfloor x/q\rfloor,\quad b=x-aq,\qquad c=\lfloor y/q\rfloor,\quad d=y-cq,
$$

where $0\leq b,d<q$ and $0\leq a,c<B^{n-m}$. The [floor function](calculus.md#floor-function) selects the high block; the remainder selects the low block. Both operands must use the same $q$, including when their actual digit lengths differ.

For odd $n$, the low block has $m$ digit positions and the high block has $n-m=m-1$. Leading zero padding aligns a shorter operand without changing its [integer](integer.md) value. Padding to a power-of-two length is optional: the split itself works for every $n$. If power-of-two padding is used, the padded length is less than twice the original length, so it changes only a constant factor in the [asymptotic analysis](real-analysis.md#asymptotic-analysis).

### Karatsuba three-product identity

↑ **Parent:** [Karatsuba multiplication](#karatsuba-multiplication)

Compute exactly three smaller products,

$$
p_2=ac,\qquad p_0=bd,\qquad p_s=(a+b)(c+d).
$$

The [distributive property](algebraic-operation.md#distributive-property) gives $p_s=ac+ad+bc+bd$, so the cross coefficient is $h=p_s-p_2-p_0=ad+bc$. Recombine by

$$
xy=p_2q^2+hq+p_0,\qquad q=B^m.
$$

The saving is that $ad$ and $bc$ are never separately multiplied. Multiplying a digit block by $q$ or $q^2$ shifts its position in [positional notation](integer.md#positional-notation); it does not require another general [integer](integer.md) [multiplication](arithmetic.md#multiplication). [Addition](arithmetic.md#addition) of the shifted results still requires [Karatsuba carry handling](#karatsuba-carry-handling).

<a id="image-three-products-recover-the-karatsuba-cross-coefficient"></a>
![](karatsuba-three-product-dataflow.png)

**[Figure 27](#image-three-products-recover-the-karatsuba-cross-coefficient). Three products recover the Karatsuba cross coefficient**. The arrows carry exact [integer](integer.md) values for the [Karatsuba worked multiplication](#karatsuba-worked-multiplication). Only the three coloured product boxes require recursive [multiplication](arithmetic.md#multiplication); the lower boxes use [subtraction](arithmetic.md#subtraction), digit shifts and [addition](arithmetic.md#addition).

### Karatsuba worked multiplication

↑ **Parent:** [Karatsuba multiplication](#karatsuba-multiplication)

Use [decimal expansion](integer.md#decimal-expansion), $B=10$, $n=4$, $m=2$, and $q=100$. The [Karatsuba operand splitting](#karatsuba-operand-splitting) is $1234=12\cdot100+34$, $5678=56\cdot100+78$. The [Karatsuba three-product identity](#karatsuba-three-product-identity) gives

$$
\begin{aligned}
p_2&=12\cdot56=672,\\
p_0&=34\cdot78=2652,\\
p_s&=(12+34)(56+78)=46\cdot134=6164,\\
h&=6164-672-2652=2840,\\
xy&=672\cdot10000+2840\cdot100+2652=7{,}006{,}652.
\end{aligned}
$$

The third product has a three-digit operand. A small-input base case can evaluate these three products directly, or a smaller threshold can continue [recursion](#recursion-computer-science). Either choice preserves the identity; only the operation count changes.

The same [Karatsuba operand splitting](#karatsuba-operand-splitting) handles $123\cdot45$: choose $n=3$, $m=2$, and write $123=1\cdot100+23$, $45=0\cdot100+45$. Then $p_2=0$, $p_0=1035$, $p_s=24\cdot45=1080$, and $h=45$, giving $4500+1035=5535$. A zero high block and unequal lengths require no new algebraic rule.

### Karatsuba carry handling

↑ **Parent:** [Karatsuba multiplication](#karatsuba-multiplication)

The blocks in the [Karatsuba three-product identity](#karatsuba-three-product-identity) are [integers](integer.md), not single digits: $p_0$ can need $2m$ positions and $h$ can exceed $q-1$. Concatenating the displayed blocks therefore fails. Accumulate their shifted values with ordinary [addition](arithmetic.md#addition), normalizing each digit position by [Euclidean division](integer.md#euclidean-division): a coefficient $v$ becomes the digit $v\bmod B$, with carry $\lfloor v/B\rfloor$ passed to the next position. [Subtraction](arithmetic.md#subtraction) likewise propagates borrows. Although $h\geq0$ for these nonnegative [integers](integer.md), intermediate digitwise [subtraction](arithmetic.md#subtraction) can still borrow.

In the four-digit [Karatsuba worked multiplication](#karatsuba-worked-multiplication), grouping by base $q=100$ gives unnormalized coefficients $[672,2840,2652]$, written from high to low. Normalize from the right: $2652=26\cdot100+52$; $2840+26=2866=28\cdot100+66$; $672+28=700=7\cdot100+0$. The final groups are $[7,00,66,52]$, yielding $7{,}006{,}652$. The zero group must retain its two positions.

Since $a,b,c,d<B^m$, their sums are less than $2B^m\leq B^{m+1}$ and can need $m+1$ digits. Allocate that extra digit before the third recursive product; discarding it can change the answer. The GMP manual describes this sum growth and uses a difference-based form to avoid it.[GNU MP 6.3.0 manual, §15.1.2 Karatsuba Multiplication: sum-based middle product can exceed k limbs; absolute differences and their signs](computer-science-bibliography.md#gnu-mp-6-3-0-manual/karatsuba-multiplication)

### Karatsuba recursion termination

↑ **Parent:** [Karatsuba multiplication](#karatsuba-multiplication)

For the sum-based [Karatsuba three-product identity](#karatsuba-three-product-identity), a safe fixed base-case threshold is three digits or more. Return zero directly if either operand is zero; at or below the threshold, use ordinary digit-by-digit [multiplication](arithmetic.md#multiplication). Otherwise split by the maximum current operand length and invoke [Karatsuba multiplication](#karatsuba-multiplication) on $(a,c)$, $(b,d)$, and $(a+b,c+d)$.

Each recursive operand has at most $\lceil n/2\rceil+1$ digits. This is strictly less than $n$ for $n\geq4$, proving termination. A rule stopping only at one digit does not supply this guarantee: in base two, $3=11_2$ splits into $1,1$, whose sum is $2=10_2$, still two digits. An implementation must choose a sufficient threshold or explicitly handle such nonshrinking calls. Leading zero padding must not be repeatedly added in a way that defeats the decreasing size measure.

For signed [integers](integer.md), multiply absolute values with the same nonnegative procedure and restore the sign afterwards. This changes the representation bookkeeping, rather than the three-product identity.

### Karatsuba digit-operation cost

↑ **Parent:** [Karatsuba multiplication](#karatsuba-multiplication)

Count a fixed-base digit [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction), digit copy, or single-digit [multiplication](arithmetic.md#multiplication) as constant cost. Base $B$ stays fixed as $n$ grows; an entire arbitrary-length [integer](integer.md) [multiplication](arithmetic.md#multiplication) is not one constant-cost step. With this model, splitting, sum formation, shifts and recombination require $O(n)$ digit operations. Ordinary digit-by-digit [multiplication](arithmetic.md#multiplication) forms $n^2$ digit products for two $n$-position operands. The GMP base-case description uses this rectangular product arrangement.[GNU MP 6.3.0 manual, §15.1.1 Basecase Multiplication: rectangular cross-products and O(NM) cost](computer-science-bibliography.md#gnu-mp-6-3-0-manual/basecase-multiplication)

The ideal equal-half [recurrence relation](sequence-and-series.md#recurrence-relation) is

$$
T(n)=3T(n/2)+O(n).
$$

For $n=2^k$, level $j$ has $3^j$ calls of size $n/2^j$. If each internal call incurs exactly $\alpha$ times its size in additional digit work, that level contributes $\alpha n(3/2)^j$. There are $3^k=n^{\log_2 3}$ leaves. The [geometric series](sequence-and-series.md#geometric-series) of internal work is

$$
\alpha n\sum_{j=0}^{k-1}(3/2)^j=2\alpha(3^k-2^k).
$$

Thus fixed positive leaf cost plus this internal work grows on the order of $n^{\log_2 3}$. In [Big O notation](real-analysis.md#big-o-notation), $T(n)=O(n^{\log_2 3})$. Removing one of four products at every level matters much more than saving just one at the root.

<a id="image-karatsuba-recursion-levels-and-an-explicitly-stipulated-cost-comparison"></a>
![](karatsuba-recursion-digit-cost.png)

**[Figure 28](#image-karatsuba-recursion-levels-and-an-explicitly-stipulated-cost-comparison). Karatsuba recursion levels and an explicitly stipulated cost comparison**. Left: the ideal equal-half [recursion](#recursion-computer-science) for $n=8$, with three children per internal call. Right: model counts for $n=2^k$, one unit per leaf and internal overhead $\alpha s$ for size $s$ with $\alpha=1$. The resulting count is $3\cdot3^k-2\cdot2^k$, compared with $n^2$ ordinary digit products. This illustrates the [recurrence relation](sequence-and-series.md#recurrence-relation); its constants and crossover are stipulated, rather than measured execution times.

The literal sum-based implementation instead admits the upper bound

$$
T(n)\leq3T(\lceil n/2\rceil+1)+Cn
$$

for a nondecreasing worst-case cost envelope above a fixed base-case threshold. The extra digit does not change the exponent: since $\lceil n/2\rceil+1\leq n/2+3/2$, subtracting three from the size makes each child's adjusted size at most half its parent's. Stop this comparison at any fixed threshold greater than three; its [recursion](#recursion-computer-science) depth is $\log_2 n+O(1)$ and the level-work sum is bounded by the same [geometric series](sequence-and-series.md#geometric-series) up to constant factors. Exact call counts can depend on carries, zero shortcuts and the threshold, so they need not equal the ideal $3^j$ at each depth.

### Karatsuba practical crossover

↑ **Parent:** [Karatsuba multiplication](#karatsuba-multiplication)

[Karatsuba digit-operation cost](#karatsuba-digit-operation-cost) explains eventual scaling, while a practical base-case threshold depends on the costs of [addition](arithmetic.md#addition), [subtraction](arithmetic.md#subtraction), copying and function calls relative to small [integer](integer.md) [multiplication](arithmetic.md#multiplication). Using $M(n)=An^2+Dn+E$ for a base-case cost, one Karatsuba level costs $3M(n/2)+Fn+G$: the quadratic coefficient falls to $3A/4$, but the linear contribution includes $3Dn/2+Fn$. Small operands can therefore cost more despite the smaller exponent. This comparison and the effect of implementation improvements on the threshold are described in the GMP manual.[GNU MP 6.3.0 manual, §15.1.2 Karatsuba Multiplication: final paragraphs comparing M(N) and K(N), and effects of base-case speedups on thresholds](computer-science-bibliography.md#gnu-mp-6-3-0-manual/karatsuba-multiplication)

The plotted crossover belongs only to the stipulated constants in its caption; its ordinary-method curve counts digit products alone, while the Karatsuba curve includes the chosen internal overhead. Selecting a threshold for real software requires measuring the actual implementation on its intended machine. With base $B=2^w$ for a fixed machine digit width $w$, the same analysis counts machine digits; it does not establish a universal crossover in decimal digits, [bits](information-theory.md#bit), or elapsed time.

## Randomized algorithm

↑ **Parent:** [Algorithm](algorithm.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Randomized_algorithm)

A randomized algorithm makes some choices using random bits.

For a fixed [input](theoretical-computer-science.md#input-computer-science), the random [bits](information-theory.md#bit) can change the path taken by a [randomized algorithm](#randomized-algorithm), its [output](theoretical-computer-science.md#output-computing), or its running time. Specify the distribution of those choices and which guarantee is required: [one-sided error](#one-sided-error) permits mistakes of only one kind, whereas [ZPP](#zpp) requires a correct answer and bounds the expected running time. [Polynomial identity testing](#polynomial-identity-testing) makes this distinction concrete: choosing different [field](algebra.md#field) elements changes whether a nonidentity is detected.

A [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution) must be implemented faithfully. To choose uniformly from $\{0,1,2,3,4\}$ using fair [independent](random-variable.md#independent-random-variables) [bits](information-theory.md#bit), read three [bits](information-theory.md#bit) as a number from zero to seven, discard five through seven, and repeat until a permitted value appears. Each retained value has the same chance. Taking the three-bit number modulo five instead would give zero, one and two twice as many preimages as three and four, invalidating a calculation that assumes equal chances.

### Uniform balanced binary sequence sampling

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)

A balanced [binary sequence](sequence-and-series.md#bitstream) of length $2n$ has $n$ entries of each kind. Uniformly sample an $n$-element [subset](set.md#subset) of the positions and place the first kind there. If $2n$ is a power of two, repeatedly draw uniform positions using $\log_2(2n)$ fair random [bits](information-theory.md#bit), reject previously selected positions, and stop after $n$ distinct positions. Each new position is uniform among those remaining, making every $n$-element [subset](set.md#subset) equally likely. The expected number of draws is $\sum_{s=0}^{n-1}2n/(2n-s)<2n$, giving $O(n\log n)$ expected random [bits](information-theory.md#bit).

### Derandomization

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Derandomization)

Derandomization converts a randomized construction or algorithm into a deterministic one while preserving its desired guarantee. The [method of conditional probabilities](#method-of-conditional-probabilities) does this by maintaining a computable [conditional expectation](measure-theory.md#conditional-expectation) until all choices are fixed.

#### Method of conditional probabilities

↑ **Parent:** [Derandomization](#derandomization)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_conditional_probabilities)

The method of conditional probabilities turns an [expected value](expected-value.md) guarantee into a deterministic construction. For a maximization [objective function](mathematical-optimization.md#objective-function), fix one choice at a time, always keeping the [conditional expectation](measure-theory.md#conditional-expectation) of the final value at least as large as before. Once every choice is fixed, that [conditional expectation](measure-theory.md#conditional-expectation) is the actual value. The useful ingredient is a way to evaluate the [conditional expectations](measure-theory.md#conditional-expectation) efficiently.

No actual random choices are needed during this construction. The [probability distribution](probability-distribution.md) describes hypothetical completions used in the analysis; the algorithm compares their [conditional expectations](measure-theory.md#conditional-expectation) and commits deterministically. For [maximum cut](graph-theory.md#maximum-cut), this converts the [random cut lower bound](graph-theory.md#random-cut-lower-bound) into a [cut of a graph](graph-theory.md#cut-graph-theory) containing at least half the [edges](graph-theory.md#edge-of-a-graph). A [maximum cut](graph-theory.md#maximum-cut) can still be larger, as the [conditional expectations cut example](#conditional-expectations-cut-example) shows.

##### Conditional expectation of a monochromatic clique count

↑ **Parent:** [Method of conditional probabilities](#method-of-conditional-probabilities)

In a partially fixed two-colour [edge coloring](graph-coloring.md#edge-coloring) of a [complete graph](graph-theory.md#complete-graph), complete all unassigned [edges](graph-theory.md#edge-of-a-graph) independently and fairly. For a fixed [clique](graph-theory.md#clique-graph-theory) with $r$ unassigned [edges](graph-theory.md#edge-of-a-graph), its [conditional probability](probability-theory.md#conditional-probability) of becoming [monochromatic](ramsey-theory.md#monochromatic-set) is zero if both colours already occur; $2^{-r}$ if a colour is fixed and no conflicting colour occurs; and $2^{1-r}$ if none is fixed. Sum these [conditional probabilities](probability-theory.md#conditional-probability) over the [cliques](graph-theory.md#clique-graph-theory) to obtain a computable [conditional expectation](measure-theory.md#conditional-expectation). Fix each next [edge](graph-theory.md#edge-of-a-graph) to a colour that does not increase this [conditional expectation](measure-theory.md#conditional-expectation), yielding a deterministic minimization construction.

##### Conditional expectation choice invariant

↑ **Parent:** [Method of conditional probabilities](#method-of-conditional-probabilities)

Let $Z=Z(X_1,\ldots,X_n)$ be a real-valued [objective function](mathematical-optimization.md#objective-function) of finitely many choices, with finite [expected value](expected-value.md). Suppose a prefix $P=(X_1=x_1,\ldots,X_i=x_i)$ has positive [probability](probability-theory.md#probability). Write $q(P)=\mathbb E[Z\mid P]$. If the next choice is a fair [bit](information-theory.md#bit), the [law of total expectation](measure-theory.md#law-of-total-expectation) gives

$$
q(P)=\frac{q(P,0)+q(P,1)}2.
$$

At least one child is at least this average. Choose a child with the larger value, using a fixed rule for ties. The resulting [loop invariant](#loop-invariant) is $q(P)\geq\mathbb E Z$. At a complete assignment $x$, there is only one completion left, so $q(x)=Z(x)$ and therefore $Z(x)\geq\mathbb E Z$.

For a biased choice or more than two possibilities, use the corresponding weighted average:

$$
q(P)=\sum_{a:\,p_a>0}p_aq(P,a),\qquad p_a=\mathbb P(X_{i+1}=a\mid P).
$$

Some positive-[probability](probability-theory.md#probability) child is at least the weighted average. For minimization, choose a child at most the current [conditional expectation](measure-theory.md#conditional-expectation) and reverse the invariant. The averaging identity is the same in both directions.[Jeff Erickson, Discrete Probability, §1.2.2, printed pp. 6–7: conditional expectation decomposition and linearity; authorship stated on the author's Algorithms notes page](computer-science-bibliography.md#discrete-probability-by-jeff-erickson)

The word "probabilities" in the method's name also covers an [indicator random variable](expected-value.md#indicator-random-variable) for an undesirable outcome: keeping its [conditional expectation](measure-theory.md#conditional-expectation), which is its [conditional probability](probability-theory.md#conditional-probability), strictly below one eventually forces that indicator to be zero. Optimizing an ordinary numerical [objective function](mathematical-optimization.md#objective-function) is the [method of conditional expectations](#method-of-conditional-probabilities) formulation used below.

##### Conditional expectations for maximum cut

↑ **Parent:** [Method of conditional probabilities](#method-of-conditional-probabilities)

Let $G=(V,E)$ be a finite undirected [simple graph](graph.md#simple-graph), with $n=|V|$ [vertices](graph.md#vertex-graph-theory) and $m=|E|$ [edges](graph-theory.md#edge-of-a-graph). A [cut of a graph](graph-theory.md#cut-graph-theory) assigns each [vertex](graph.md#vertex-graph-theory) a label zero or one; an [edge](graph-theory.md#edge-of-a-graph) crosses precisely when its endpoints have different labels. Its size is the number of crossing [edges](graph-theory.md#edge-of-a-graph). A [maximum cut](graph-theory.md#maximum-cut) maximizes that size.

For the analysis, assign [independent](random-variable.md#independent-random-variables) fair [bits](information-theory.md#bit) $X_v$ to the [vertices](graph.md#vertex-graph-theory). For each [edge](graph-theory.md#edge-of-a-graph) $uv$, the [indicator random variable](expected-value.md#indicator-random-variable) $I_{uv}=\mathbf1_{\{X_u\ne X_v\}}$ has [expected value](expected-value.md) $1/2$: exactly two of the four equally likely endpoint assignments cross. Thus [linearity of expectation](expected-value.md#linearity-of-expectation) gives the [random cut lower bound](graph-theory.md#random-cut-lower-bound):

$$
C=\sum_{uv\in E}I_{uv},\qquad \mathbb E C=\sum_{uv\in E}\frac12=\frac m2.
$$

[Linearity of expectation](expected-value.md#linearity-of-expectation) does not require the [indicator random variables](expected-value.md#indicator-random-variable) to be [independent](random-variable.md#independent-random-variables). What matters here is the stipulated distribution of the endpoint [bits](information-theory.md#bit).

###### Conditional expectation cut formula

↑ **Parent:** [Conditional expectations for maximum cut](#conditional-expectations-for-maximum-cut)

For any partial assignment $P$, let $f(P)$ count [edges](graph-theory.md#edge-of-a-graph) whose two endpoints are already fixed on opposite sides, and let $u(P)$ count [edges](graph-theory.md#edge-of-a-graph) with at least one unassigned endpoint. Under the remaining [independent](random-variable.md#independent-random-variables) fair [bits](information-theory.md#bit),

$$
q(P)=\mathbb E[C\mid P]=f(P)+\frac{u(P)}2.
$$

An [edge](graph-theory.md#edge-of-a-graph) with fixed equal labels contributes zero; fixed unequal labels contribute one. If one endpoint is unassigned, its fair [bit](information-theory.md#bit) disagrees with the fixed label with [probability](probability-theory.md#probability) $1/2$. If both endpoints are unassigned, their [independent](random-variable.md#independent-random-variables) fair [bits](information-theory.md#bit) disagree with [probability](probability-theory.md#probability) $1/2$ as well. Count each unresolved [edge](graph-theory.md#edge-of-a-graph) once, even when both endpoints are unassigned.

Process [vertices](graph.md#vertex-graph-theory) in a fixed order. Evaluate the [conditional expectation cut formula](#conditional-expectation-cut-formula) after setting the next label to zero and after setting it to one; retain the larger value, choosing zero on ties. The [conditional expectation choice invariant](#conditional-expectation-choice-invariant) ensures the final [cut of a graph](graph-theory.md#cut-graph-theory) has size at least $m/2$. This is a deterministic [approximation algorithm](mathematical-optimization.md#approximation-algorithm) for [maximum cut](graph-theory.md#maximum-cut).[CS 4820: Algorithms, Spring 2011; Cornell CS 4820, Lecture notes on randomized approximation algorithms, 2 May 2011, §1.1.2, printed pp. 2–3: conditional expectations, Algorithms 1–2 and the half-total-edge-weight guarantee; no individual byline stated](computer-science-bibliography.md#cs-4820-algorithms-spring-2011/lecture-notes-on-randomized-approximation-algorithms)

###### Conditional expectations cut example

↑ **Parent:** [Conditional expectations for maximum cut](#conditional-expectations-for-maximum-cut)

Consider the following original five-[vertex](graph.md#vertex-graph-theory) [simple graph](graph.md#simple-graph), where $AB$ denotes the undirected [edge](graph-theory.md#edge-of-a-graph) $\{A,B\}$:

$$
V=\{A,B,C,D,E\},\qquad E=\{AB,BC,CD,DE,EA,AC,BD\}.
$$

Its seven [edges](graph-theory.md#edge-of-a-graph) give initial [expected value](expected-value.md) $q(\varnothing)=7/2=3.5$. Use [vertex](graph.md#vertex-graph-theory) order $A,B,C,D,E$ and choose zero whenever the two child [conditional expectations](measure-theory.md#conditional-expectation) tie.

<a id="image-a-guaranteed-five-edge-cut-and-a-six-edge-maximum-cut-of-the-same-graph"></a>
![](conditional-expectations-graph-cut.png)

**[Figure 29](#image-a-guaranteed-five-edge-cut-and-a-six-edge-maximum-cut-of-the-same-graph). A guaranteed five-edge cut and a six-edge maximum cut of the same graph**. The [conditional expectations cut example](#conditional-expectations-cut-example) uses the same original [simple graph](graph.md#simple-graph) in both panels. Node colours and labels identify the two sides of each [cut of a graph](graph-theory.md#cut-graph-theory). Solid teal [edges](graph-theory.md#edge-of-a-graph) cross; dashed grey [edges](graph-theory.md#edge-of-a-graph) do not. The deterministic choices on the left give five crossing [edges](graph-theory.md#edge-of-a-graph); the assignment on the right gives six. Crossings of drawn lines are not additional [vertices](graph.md#vertex-graph-theory).

The complete decision ledger is below. A prefix lists fixed labels in [vertex](graph.md#vertex-graph-theory) order; all later labels remain hypothetically [independent](random-variable.md#independent-random-variables) fair [bits](information-theory.md#bit). Each candidate entry is the [conditional expectation](measure-theory.md#conditional-expectation) of the final [cut of a graph](graph-theory.md#cut-graph-theory), including the contribution of unresolved [edges](graph-theory.md#edge-of-a-graph).

| Prefix before choice | Next [vertex](graph.md#vertex-graph-theory) | Set to 0 | Set to 1 | Chosen label | Retained [conditional expectation](measure-theory.md#conditional-expectation) |
| --- | --- | --- | --- | --- | --- |
| Empty | $A$ | $3.5$ | $3.5$ | $0$ | $3.5$ |
| $0$ | $B$ | $3$ | $4$ | $1$ | $4$ |
| $01$ | $C$ | $4$ | $4$ | $0$ | $4$ |
| $010$ | $D$ | $4$ | $4$ | $0$ | $4$ |
| $0100$ | $E$ | $3$ | $5$ | $1$ | $5$ |

For example, after $A=0,B=1$, [edge](graph-theory.md#edge-of-a-graph) $AB$ is fixed crossing and the other six [edges](graph-theory.md#edge-of-a-graph) are unresolved, giving $1+6/2=4$. Setting $C=0$ fixes $BC$ crossing and $AC$ noncrossing, leaving four unresolved [edges](graph-theory.md#edge-of-a-graph): $2+4/2=4$. Setting $C=1$ instead fixes $AC$ crossing and $BC$ noncrossing, giving the same [conditional expectation](measure-theory.md#conditional-expectation).

<a id="image-conditional-expected-cut-values-along-every-chosen-branch"></a>
![](conditional-expectations-choice-ledger.png)

**[Figure 30](#image-conditional-expected-cut-values-along-every-chosen-branch). Conditional expected cut values along every chosen branch**. At each step, both candidate values are computed by the [conditional expectation cut formula](#conditional-expectation-cut-formula). The highlighted cell is chosen; ties choose zero. Below, the retained [conditional expectation](measure-theory.md#conditional-expectation) follows $3.5,3.5,4,4,4,5$, starting before any label is fixed. The last value is the actual size of the resulting [cut of a graph](graph-theory.md#cut-graph-theory), rather than an average over remaining choices.

The final labels are $(0,1,0,0,1)$, so the two sides are $\{A,C,D\}$ and $\{B,E\}$. The five crossing [edges](graph-theory.md#edge-of-a-graph) are $AB,BC,DE,EA,BD$; $AC,CD$ do not cross. This exceeds $m/2=3.5$, and hence also the rounded-up guarantee of four [edges](graph-theory.md#edge-of-a-graph).

It is not a [maximum cut](graph-theory.md#maximum-cut). Labels $(0,1,1,0,1)$ cross all [edges](graph-theory.md#edge-of-a-graph) except $BC$, giving six. Seven are impossible because the [triangle in a graph](graph.md#triangle-in-a-graph) $ABC$ cannot have all three [edges](graph-theory.md#edge-of-a-graph) crossing a two-sided [cut of a graph](graph-theory.md#cut-graph-theory). An independent enumeration of all $2^5=32$ complete label assignments gives the following distribution, counting an assignment and its label-swapped counterpart separately:

| Size of [cut of a graph](graph-theory.md#cut-graph-theory) | Number of label assignments |
| --- | --- |
| $0$ | $2$ |
| $1$ | $0$ |
| $2$ | $2$ |
| $3$ | $12$ |
| $4$ | $10$ |
| $5$ | $4$ |
| $6$ | $2$ |
| $7$ | $0$ |

The weighted sum is $112$, so the average is $112/32=3.5$, agreeing with [linearity of expectation](expected-value.md#linearity-of-expectation). Choosing $C=0$ in the earlier tie discards the remaining size-six completion while preserving the average of four. The method protects an [expected value](expected-value.md) guarantee; it need not preserve the best possible completion.

###### Conditional expectations algorithm cost

↑ **Parent:** [Conditional expectations for maximum cut](#conditional-expectations-for-maximum-cut)

Directly scanning all $m$ [edges](graph-theory.md#edge-of-a-graph) to evaluate each child of each of $n$ choices takes $O(nm+n)$ elementary operations, in [Big O notation](real-analysis.md#big-o-notation). There is a faster implementation. When assigning [vertex](graph.md#vertex-graph-theory) $v$, let $d_0$ and $d_1$ count its already assigned [graph neighbours](graph-theory.md#neighbour-of-a-vertex) labelled zero and one. Contributions from [edges](graph-theory.md#edge-of-a-graph) not incident to $v$ are unchanged, and contributions from [edges](graph-theory.md#edge-of-a-graph) to unassigned [graph neighbours](graph-theory.md#neighbour-of-a-vertex) stay $1/2$ for either choice. Therefore

$$
q(P,v=0)-q(P,v=1)=d_1-d_0.
$$

Choose zero if $d_1\geq d_0$, otherwise one: put $v$ on the side with fewer already assigned [graph neighbours](graph-theory.md#neighbour-of-a-vertex). With [adjacency lists](data-structure.md#adjacency-list), scanning each [vertex](graph.md#vertex-graph-theory)'s list once costs $O(n+m)$ operations overall and uses $O(n+m)$ storage including the [graph](graph.md). These bounds count operations on labels and counters that fit in machine words of $O(\log(n+m+2))$ [bits](information-theory.md#bit). Multiplying the [conditional expectation cut formula](#conditional-expectation-cut-formula) by two also permits exact integer comparisons without rounding.

If $\operatorname{OPT}$ is the size of a [maximum cut](graph-theory.md#maximum-cut), then $\operatorname{OPT}\leq m$. The constructed [cut of a graph](graph-theory.md#cut-graph-theory) thus has size at least $m/2\geq\operatorname{OPT}/2$, an [approximation ratio](mathematical-optimization.md#approximation-ratio) of $1/2$ in the maximization convention. The five-versus-six example illustrates the gap between this guarantee and exact optimization.

For a general [randomized algorithm](#randomized-algorithm), the averaging proof alone does not establish efficient [derandomization](#derandomization). One needs a polynomial number of commitments, an efficient way to find a suitable child at each step, and manageable representations and evaluation costs for the relevant [conditional expectations](measure-theory.md#conditional-expectation). Those evaluations can themselves be hard. Enumerating all completions verifies this small example, but would take exponentially many assignments as $n$ grows. The [polynomial-time algorithm](theoretical-computer-science.md#polynomial-time-algorithm) here comes from the local [conditional expectation cut formula](#conditional-expectation-cut-formula), not from that enumeration.

### Probabilistic Turing machine

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probabilistic_Turing_machine)

A probabilistic Turing machine is a [Turing machine](theoretical-computer-science.md#turing-machine) whose transitions may depend on independent random bits.

### One-sided error

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)

A randomized decision algorithm has one-sided error when one answer is always correct and only the other answer can be mistaken.

The guarantee concerns each fixed [input](theoretical-computer-science.md#input-computer-science), with [probability](probability-theory.md#probability) taken over the choices of the [randomized algorithm](#randomized-algorithm). Always state which answer is protected. In [polynomial identity testing](#polynomial-identity-testing), call an [input](theoretical-computer-science.md#input-computer-science) positive when its [polynomial](polynomial.md) is identically zero, and let acceptance mean claiming an identity. Then the possibilities are:

| Actual [polynomial](polynomial.md) | Accept: claim identity | Reject: claim nonidentity |
| --- | --- | --- |
| Identically zero | Always correct; every trial accepts. | Impossible with exact [polynomial evaluation](polynomial.md#polynomial-evaluation). |
| Nonzero | Possible mistake if the chosen point is a zero. | Always correct; the point is a witness. |

Thus a zero [polynomial evaluation](polynomial.md#polynomial-evaluation) can leave uncertainty, but a nonzero [polynomial evaluation](polynomial.md#polynomial-evaluation) settles the question. An error bound for a fixed nonzero [polynomial](polynomial.md) is not the [conditional probability](probability-theory.md#conditional-probability) that a particular accepted [input](theoretical-computer-science.md#input-computer-science) is an identity; that latter question would need a distribution on the [inputs](theoretical-computer-science.md#input-computer-science) as well.

In [computational complexity theory](theoretical-computer-science.md#computational-complexity-theory), a [polynomial-time algorithm](theoretical-computer-science.md#polynomial-time-algorithm) with this orientation and false acceptance [probability](probability-theory.md#probability) at most $1/2$ establishes membership in [co-RP](#co-rp). Reversing the question to ask whether the [polynomial](polynomial.md) is nonzero gives the [RP](#rp-complexity) orientation: negative instances are always rejected. The [random evaluation test for a polynomial identity](#random-evaluation-test-for-a-polynomial-identity) explains the required [field](algebra.md#field), [total degree](polynomial.md#total-degree-of-a-polynomial), sampling and evaluation assumptions.

#### RP (complexity)

↑ **Parent:** [One-sided error](#one-sided-error)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/RP_(complexity))

$\mathbf{RP}$ contains decision problems with a polynomial-time randomized algorithm that rejects every negative instance and accepts every positive instance with probability at least one half.

#### co-RP

↑ **Parent:** [One-sided error](#one-sided-error)

$\mathbf{co\text{-}RP}$ consists of complements of languages in [RP](#rp-complexity). Its algorithms always accept positive instances and reject negative instances with probability at least one half.

### ZPP

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/ZPP)

$\mathbf{ZPP}=\mathbf{RP}\cap\mathbf{co\text{-}RP}$. Equivalently, it consists of problems having an always-correct randomized algorithm with polynomial expected running time.

### Error reduction for a randomized algorithm

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)

Independent repetitions reduce a randomized algorithm's error probability while preserving polynomial running time.

The combining rule depends on the error orientation. For [one-sided error](#one-sided-error) with false acceptance [probability](probability-theory.md#probability) at most $p<1$, reject as soon as any trial rejects and accept only if every trial accepts. For $k$ [independent](random-variable.md#independent-random-variables) trials on the same fixed negative [input](theoretical-computer-science.md#input-computer-science), false acceptance has [probability](probability-theory.md#probability) at most $p^k$. The protected positive [inputs](theoretical-computer-science.md#input-computer-science) still always accept. If false rejection is the possible mistake instead, accept as soon as any trial accepts. This uses the decisive answer rather than a majority vote.

For constant $p<1$, $k$ grows only logarithmically in $1/\varepsilon$ to achieve error at most $\varepsilon$. A polynomial number of trials preserves a [polynomial-time algorithm](theoretical-computer-science.md#polynomial-time-algorithm)'s running-time bound. Independence matters: repeating one answer, or evaluating at the same random point each time, supplies no new evidence. The [independent repetition of a polynomial identity test](#independent-repetition-of-a-polynomial-identity-test) gives an exact $25$-outcome example.

### Polynomial identity testing

↑ **Parent:** [Randomized algorithm](#randomized-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Polynomial_identity_testing)

Polynomial identity testing asks whether a polynomial represented implicitly, such as by an arithmetic circuit or a remainder computation, is the zero polynomial.

Here zero means that every [coefficient](vector-space.md#coefficient) vanishes after collecting equal [monomials](polynomial.md#monomial) in the [polynomial ring](commutative-algebra.md#polynomial-ring). Testing equality of two [polynomials](polynomial.md) $A,B$ amounts to testing $P=A-B$ for zero. An [arithmetic circuit](theoretical-computer-science.md#arithmetic-circuit) can permit cheap [polynomial evaluation](polynomial.md#polynomial-evaluation) even when expanding all [monomials](polynomial.md#monomial) is expensive. The [random evaluation test for a polynomial identity](#random-evaluation-test-for-a-polynomial-identity) exploits this: one nonzero value disproves the [polynomial identity](polynomial.md#polynomial-identity), while a known [total degree](polynomial.md#total-degree-of-a-polynomial) limits how often a nonzero [polynomial](polynomial.md) can evade detection.[CPSC 536N: Randomized Algorithms; Lecture 9: Polynomial Identity Testing by the Schwartz-Zippel Lemma, §1: formal zero means all coefficients vanish; representations and evaluation access](computer-science-bibliography.md#cpsc-536n-randomized-algorithms/lecture-9-polynomial-identity-testing-by-the-schwartz-zippel-lemma)

For example, for an [integer](integer.md) $n\ge1$, $\prod_{i=1}^n(1+x_i)$ has $2^n$ distinct [monomials](polynomial.md#monomial), one for each [subset](set.md#subset) of the $n$ [variables](mathematics.md#variable-mathematics). Its factored expression needs only $n$ [additions](arithmetic.md#addition) and $n-1$ [multiplications](arithmetic.md#multiplication) for one [polynomial evaluation](polynomial.md#polynomial-evaluation). Evaluating the compact expression avoids creating its expanded list of [coefficients](vector-space.md#coefficient). The saving is especially attractive in many [variables](mathematics.md#variable-mathematics); it does not make a zero result into a proof of identity.

#### Polynomial identity testing over a finite field

↑ **Parent:** [Polynomial identity testing](#polynomial-identity-testing)

Work in the [finite field](algebra.md#finite-field) $\mathbb F_5=\{0,1,2,3,4\}$, using [modular arithmetic](modular-arithmetic.md) modulo five. Consider the two original [polynomial](polynomial.md) examples

$$
F(x)=(x+1)^2-x^2-2x-1,\qquad G(x)=(x-1)(x-2).
$$

The [distributive property](algebraic-operation.md#distributive-property) gives $(x+1)^2=x^2+2x+1$, so all [coefficients](vector-space.md#coefficient) of $F$ cancel: $F$ is identically zero. In contrast, $G=x^2-3x+2=x^2+2x+2$ in this [finite field](algebra.md#finite-field), with nonzero leading [coefficient](vector-space.md#coefficient). Its [roots of a polynomial](polynomial.md#root-of-a-polynomial) are exactly one and two: a product in a [field](algebra.md#field) is zero only if a factor is zero.

The complete [polynomial evaluations](polynomial.md#polynomial-evaluation), displayed as representatives modulo five, are

$$
\begin{array}{c|ccccc}
a&0&1&2&3&4\\\hline
F(a)&0&0&0&0&0\\
G(a)&2&0&0&2&1
\end{array}.
$$

In particular, $G(3)=(3-1)(3-2)=2$ is a nonzero witness, which disproves identity without examining other points. At one or two, a zero value fails to reveal that $G$ is nonzero. A [random variable](random-variable.md) $a$ with a [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution) $\mathbb F_5$ hits those two [polynomial roots](polynomial.md#root-of-a-polynomial) with [probability](probability-theory.md#probability) $2/5$.

<a id="image-exact-evaluations-distinguish-a-zero-polynomial-from-a-nonzero-polynomial-with-two-roots"></a>
![](polynomial-identity-evaluation-outcomes.png)

**[Figure 31](#image-exact-evaluations-distinguish-a-zero-polynomial-from-a-nonzero-polynomial-with-two-roots). Exact evaluations distinguish a zero polynomial from a nonzero polynomial with two roots**. Every element of the [finite field](algebra.md#finite-field) $\mathbb F_5$ is shown. The upper row always accepts the identity $F=0$. In the lower row, the two orange zero values falsely accept $G=0$; the three blue nonzero values correctly reject it. These are all possible outcomes, not sampled frequencies.

A crucial limit appears with $H(x)=x^5-x$. Its [coefficients](vector-space.md#coefficient) make it a nonzero [polynomial](polynomial.md) of [polynomial degree](polynomial.md#degree-of-a-polynomial) five in $\mathbb F_5[x]$, yet direct [polynomial evaluation](polynomial.md#polynomial-evaluation) gives zero at all five [field](algebra.md#field) elements: the values before reduction are $0,0,30,240,1020$, all divisible by five. Thus $H$ induces the same [polynomial function](polynomial.md#polynomial-function) as the zero [polynomial](polynomial.md). Any number of trials restricted to $\mathbb F_5$ will falsely accept this identity. This is compatible with the [Schwartz-Zippel lemma](combinatorics.md#schwartz-zippel-lemma): the ratio of [polynomial degree](polynomial.md#degree-of-a-polynomial) to sampling-set size is $5/5=1$, which gives no useful guarantee.

When a [polynomial](polynomial.md)'s representation permits [polynomial evaluation](polynomial.md#polynomial-evaluation) over a larger [field extension](algebra.md#field-extension), a larger sampling [set](set.md) can restore the useful degree ratio. Access only to the induced [polynomial function](polynomial.md#polynomial-function) on the original [finite field](algebra.md#finite-field) cannot distinguish $H$ from zero.[CPSC 536N: Randomized Algorithms; Lecture 9: Polynomial Identity Testing by the Schwartz-Zippel Lemma, §1.4: formal nonzero polynomials can vanish everywhere on a finite field; extension-field evaluations need a suitable representation](computer-science-bibliography.md#cpsc-536n-randomized-algorithms/lecture-9-polynomial-identity-testing-by-the-schwartz-zippel-lemma)

#### Random evaluation test for a polynomial identity

↑ **Parent:** [Polynomial identity testing](#polynomial-identity-testing)

Let $P$ be a nonzero [multivariate polynomial](polynomial.md#multivariate-polynomial) over a [field](algebra.md#field) $K$, with [total degree](polynomial.md#total-degree-of-a-polynomial) at most $d\ge0$. Choose a nonempty [finite set](set.md#finite-set) $S\subseteq K$. For [independent random variables](random-variable.md#independent-random-variables) $a_1,\ldots,a_n$, each with a [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution) on $S$, the [Schwartz-Zippel lemma](combinatorics.md#schwartz-zippel-lemma) gives

$$
\mathbb P\bigl(P(a_1,\ldots,a_n)=0\bigr)\le\min\{1,d/|S|\}.
$$

Nonzeroness is essential; the zero [polynomial](polynomial.md) always evaluates to zero. The [total degree](polynomial.md#total-degree-of-a-polynomial) sums exponents within each [monomial](polynomial.md#monomial), rather than taking their maximum: $x^2y^3+y$ has [total degree](polynomial.md#total-degree-of-a-polynomial) five. The [field](algebra.md#field) need not be finite, but $S$ must be finite. The estimate reduces error only when $d/|S|<1$.[CMPT 710 and CMPT 407 - Computational Complexity - Fall 2007; CMPT 710 - Complexity Theory: Lecture 18, §3.1, pp. 3–4: Lemma 4 and its inductive proof](computer-science-bibliography.md#cmpt-710-and-cmpt-407-computational-complexity-fall-2007/cmpt-710-complexity-theory-lecture-18)

The proof begins with the [root bound for a polynomial](polynomial.md#lagrange-root-bound-over-a-field). For several [variables](mathematics.md#variable-mathematics), write $P=\sum_{j=0}^m Q_j(x_1,\ldots,x_{n-1})x_n^j$, with $Q_m\ne0$. The [total degree](polynomial.md#total-degree-of-a-polynomial) of $Q_m$ is at most $d-m$. By [induction](foundations-of-mathematics.md#mathematical-induction), $Q_m$ vanishes with [probability](probability-theory.md#probability) at most $(d-m)/|S|$. Otherwise the remaining univariate [polynomial](polynomial.md) has at most $m$ [polynomial roots](polynomial.md#root-of-a-polynomial). Adding the two contributions gives $d/|S|$.[CMPT 710 and CMPT 407 - Computational Complexity - Fall 2007; CMPT 710 - Complexity Theory: Lecture 18, §3.1, pp. 3–4: split by the leading coefficient in the last variable](computer-science-bibliography.md#cmpt-710-and-cmpt-407-computational-complexity-fall-2007/cmpt-710-complexity-theory-lecture-18)

The [algorithm](algorithm.md) samples a point, performs exact [polynomial evaluation](polynomial.md#polynomial-evaluation), rejects the identity if the value is nonzero, and otherwise accepts. The lemma bounds false acceptance for every fixed nonzero [input](theoretical-computer-science.md#input-computer-science). For the [polynomial identity testing over a finite field](#polynomial-identity-testing-over-a-finite-field) example, $G$ has $d=2$ and $|S|=5$, so its exact $2/5$ error attains the bound. Numerical near-zero values from [floating-point arithmetic](floating-point-arithmetic.md) do not satisfy this exact algebraic contract. A [polynomial-time algorithm](theoretical-computer-science.md#polynomial-time-algorithm) claim additionally needs efficient sampling and evaluation, including the [bit](information-theory.md#bit) cost of representing and operating on [field](algebra.md#field) elements. Counting [field](algebra.md#field) operations alone does not establish that cost.

#### Independent repetition of a polynomial identity test

↑ **Parent:** [Polynomial identity testing](#polynomial-identity-testing)

Repeat the [random evaluation test for a polynomial identity](#random-evaluation-test-for-a-polynomial-identity) with fresh [independent random variables](random-variable.md#independent-random-variables), keeping the same fixed [polynomial](polynomial.md). Reject as soon as any [polynomial evaluation](polynomial.md#polynomial-evaluation) is nonzero; accept only if all $k$ values vanish. An identity is always accepted, preserving [one-sided error](#one-sided-error). If a nonzero [polynomial](polynomial.md) has single-trial false acceptance [probability](probability-theory.md#probability) $p_1$, [independence](random-variable.md#independent-random-variables) gives $p_k=p_1^k$. The [Schwartz-Zippel lemma](combinatorics.md#schwartz-zippel-lemma) bounds this by $(d/|S|)^k$ when $d<|S|$.

For $G(x)=(x-1)(x-2)$ over the [finite field](algebra.md#finite-field) $\mathbb F_5$, two uniform [independent](random-variable.md#independent-random-variables) choices $(a,b)$ have $25$ equally likely ordered outcomes, each with [probability](probability-theory.md#probability) $1/25$. Both [polynomial evaluations](polynomial.md#polynomial-evaluation) are zero only at $(1,1),(1,2),(2,1),(2,2)$. Hence false acceptance falls from $2/5$ in one trial to $4/25$ in two trials, and correct rejection rises from $3/5$ to $21/25$.

<a id="image-four-of-the-twenty-five-independent-pairs-falsely-accept-the-nonidentity"></a>
![](polynomial-identity-independent-trials.png)

**[Figure 32](#image-four-of-the-twenty-five-independent-pairs-falsely-accept-the-nonidentity). Four of the twenty-five independent pairs falsely accept the nonidentity**. The orange cells have both coordinates among the [polynomial roots](polynomial.md#root-of-a-polynomial) one and two of $G(x)=(x-1)(x-2)$ in the [finite field](algebra.md#finite-field) $\mathbb F_5$. Every blue cell supplies at least one nonzero witness. The full grid enumerates exact outcomes under [independence](random-variable.md#independent-random-variables) and a [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution); it is not a simulation.

If the second choice reuses the first, the pair is $(a,a)$ and only five diagonal outcomes are possible. Two still falsely accept, so the error remains $2/5$. Choosing fresh [independent](random-variable.md#independent-random-variables) points is precisely what makes the full $25$-cell grid and the product of [probabilities](probability-theory.md#probability) valid. For a target error $0<\varepsilon<1$, this example needs

$$
k\ge\left\lceil\frac{\log(1/\varepsilon)}{\log(5/2)}\right\rceil.
$$

The [ceiling function](calculus.md#ceiling-function) makes the trial count an [integer](integer.md). Four trials give $(2/5)^4=16/625>1/100$, while six give $64/15625<1/100$; five still give $32/3125>1/100$, so six is the first count below one percent. This is an exact error guarantee for each run on $G$, rather than an observed success rate.

## ↑ Ancestors (2)

1. [Computer science](computer-science.md)
2. [Codex Wiki](README.md)

## ← Incoming links (143)

- [AC-3](theoretical-computer-science.md#ac-3)
- [Adversary argument](#adversary-argument)
- [Algorithm](algorithm.md)
- [Algorithm correctness](#algorithm-correctness)
- [Algorithm design](#algorithm-design)
- [Analysis of algorithms](#analysis-of-algorithms)
- [Associativity of matrix multiplication](vector-space.md#associativity-of-matrix-multiplication)
- [Auxiliary space](#auxiliary-space)
- [Bareiss algorithm](numerical-linear-algebra.md#bareiss-algorithm)
- [Binary long division](integer.md#binary-long-division)
- [Binary powering multiplication count](number-theory.md#binary-powering-multiplication-count)
- [Bit complexity](theoretical-computer-science.md#bit-complexity)
- [Brent cycle-finding algorithm](#brent-cycle-finding-algorithm)
- [Bresenham's line algorithm](computer-graphics.md#bresenham-s-line-algorithm)
- [Brouwer fixed-point theorem](topological-analysis.md#brouwer-fixed-point-theorem)
- [Brute-force search](#brute-force-search)
- [Cached cell value](spreadsheet.md#cached-cell-value)
- [Catastrophic cancellation](floating-point-arithmetic.md#catastrophic-cancellation)
- [Chaikin subdivision](computer-aided-geometric-design.md#chaikin-subdivision)
- [Christos Papadimitriou](computer-science.md#christos-papadimitriou)
- [Clique (graph theory)](graph-theory.md#clique-graph-theory)
- [Combinatorics](combinatorics.md)
- [Competitive programming](computer-science.md#competitive-programming)
- [Computable colouring](ramsey-theory.md#computable-colouring)
- [Computer science](computer-science.md)
- [Condensation graph](graph-theory.md#condensation-graph)
- [Conway Game of Life](computer-science.md#conway-game-of-life)
- [Cooley-Tukey FFT algorithm](discrete-fourier-transform.md#cooley-tukey-fft-algorithm)
- [Coordinate compression](#coordinate-compression)
- [Cut vertex](graph-theory.md#cut-vertex)
- [Data structure](data-structure.md)
- [De Casteljau's algorithm](computer-aided-geometric-design.md#de-casteljau-s-algorithm)
- [Decidable theory](mathematical-logic.md#decidable-theory)
- [Destructive inorder traversal by right rotations](data-structure.md#destructive-inorder-traversal-by-right-rotations)
- [Dijkstra algorithm](shortest-path-problem.md#dijkstra-algorithm)
- [Dynamic program](mathematical-optimization.md#dynamic-program)
- [Dynamic programming](mathematical-optimization.md#dynamic-programming)
- [Exponentiation by squaring](number-theory.md#exponentiation-by-squaring)
- [Fast Fourier transform](discrete-fourier-transform.md#fast-fourier-transform)
- [Fixed-parameter tractability](theoretical-computer-science.md#fixed-parameter-tractability)
- [Floating-point arithmetic](floating-point-arithmetic.md)
- [Floor and ceiling functions](calculus.md#floor-and-ceiling-functions)
- [Floor quotient grouping](calculus.md#floor-quotient-grouping)
- [Functional programming, data structures and algorithms, procedural programming, and digital hardware examination paper by the University of Oxford (2003)](computer-science-bibliography.md#functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-examination-paper-by-the-university-of-oxford-2003)
- [Gaussian elimination](numerical-linear-algebra.md#gaussian-elimination)
- [Givens row-pair update](numerical-analysis.md#givens-row-pair-update)
- [Golden-section search](numerical-analysis.md#golden-section-search)
- [Greedy algorithm](#greedy-algorithm)
- [Huffman code](information-theory.md#huffman-code)
- [Increasing subsequence](combinatorics.md#increasing-subsequence)
- [Insertion sort](#insertion-sort)
- [Interval scheduling](#interval-scheduling)
- [Inverse Ackermann function](computability-theory.md#inverse-ackermann-function)
- [K-core of a graph](graph-theory.md#k-core-of-a-graph)
- [Kahan summation algorithm](floating-point-arithmetic.md#kahan-summation-algorithm)
- [Karatsuba multiplication](#karatsuba-multiplication)
- [Kruskal's algorithm worked example](tree-graph-theory.md#kruskal-s-algorithm-worked-example)
- [Lehmer prime-counting algorithm](number-theory.md#lehmer-prime-counting-algorithm)
- [Linear search](#linear-search)
- [Linked list](data-structure.md#linked-list)
- [Longest increasing subsequence](combinatorics.md#longest-increasing-subsequence)
- [Mathematical induction](foundations-of-mathematics.md#mathematical-induction)
- [Meet-in-the-middle algorithm](#meet-in-the-middle-algorithm)
- [Merit function](mathematical-optimization.md#merit-function)
- [Min\_25 sieve](#min-25-sieve)
- [Numerical analysis](numerical-analysis.md)
- [Numerical method](numerical-analysis.md#numerical-method)
- [One-row in-place Life update](computer-science.md#one-row-in-place-life-update)
- [Parameterized complexity](theoretical-computer-science.md#parameterized-complexity)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/advanced-data-structures-and-algorithms.md#2/d/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/databases.md#3/d/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/logic-and-proof.md#2/a/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/object-oriented-programming.md#1/b/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms.md#1/a/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2018/algorithms.md#2/f/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/algorithms.md#3/a/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence.md#2/a/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence.md#2/d/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence.md#2/g/solution)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence.md#3/f/solution)
- [Solution](past-exam-of-the-history-of-science-supplementary-subject-of-the-university-of-oxford/2022.md#1/solution)
- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2011.md#1/e/solution)
- [Solution](past-exam-of-the-integer-programming-course-of-the-university-of-oxford/2011.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-16.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-37.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-5.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38.md#5/c/solution)
- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2008.md#p/4/c/solution)
- [Solution](past-exam-of-the-probability-statistics-and-options-ii-course-of-the-university-of-oxford/2010.md#u/u2/b/iv/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware.md#4/a/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2003/functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware.md#5/c/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms.md#5/d/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2013/functional-programming-design-and-analysis-of-algorithms.md#6/b/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms.md#2/e/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms.md#6/d/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/functional-programming-design-and-analysis-of-algorithms.md#8/d/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming.md#6/b/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2016/imperative-programming.md#7/a/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms.md#4/d/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms.md#5/d/iii/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms.md#6/d/ii/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/functional-programming-design-and-analysis-of-algorithms.md#7/c/i/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit.md#2/c/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/functional-programming-design-and-analysis-of-algorithms-resit.md#7/b/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/imperative-programming-resit.md#1/e/solution)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/imperative-programming-resit.md#6/a/solution)
- [Path compression](data-structure.md#path-compression)
- [Paul W. Goldberg](computer-science.md#paul-w-goldberg)
- [Perfect elimination ordering](graph-theory.md#perfect-elimination-ordering)
- [Pigeonhole principle](combinatorics.md#pigeonhole-principle)
- [Positional notation](integer.md#positional-notation)
- [Potential method](theoretical-computer-science.md#potential-method)
- [Project Euler](project-euler.md)
- [Pseudo-polynomial time](theoretical-computer-science.md#pseudo-polynomial-time)
- [QR decomposition by Givens rotations](numerical-analysis.md#qr-decomposition-by-givens-rotations)
- [Random evaluation test for a polynomial identity](#random-evaluation-test-for-a-polynomial-identity)
- [Redelmeier's algorithm](#redelmeier-s-algorithm)
- [SAT solver](theoretical-computer-science.md#sat-solver)
- [Sieve of Eratosthenes](prime-number.md#sieve-of-eratosthenes)
- [Sliding-window algorithm](#sliding-window-algorithm)
- [Sorted-coordinate criterion for box containment](mathematical-optimization.md#sorted-coordinate-criterion-for-box-containment)
- [Sorting algorithm](#sorting-algorithm)
- [Spreadsheet circular reference](spreadsheet.md#spreadsheet-circular-reference)
- [Strictly increasing subsequence](combinatorics.md#strictly-increasing-subsequence)
- [Strong induction for factorization existence](foundations-of-mathematics.md#strong-induction-for-factorization-existence)
- [Tentative distance](shortest-path-problem.md#tentative-distance)
- [Time complexity](theoretical-computer-science.md#time-complexity)
- [Tiny-pivot roundoff in Gaussian elimination](numerical-linear-algebra.md#tiny-pivot-roundoff-in-gaussian-elimination)
- [Total variation distance](probability-and-statistics.md#total-variation-distance)
- [Uncountability obstruction to enumerating infinite Cartesian products](set-theory.md#uncountability-obstruction-to-enumerating-infinite-cartesian-products)
- [Undecidable decision problem](computability-theory.md#undecidable-decision-problem)
- [Unit-cost model](theoretical-computer-science.md#unit-cost-model)
- [Unit roundoff](floating-point-arithmetic.md#unit-roundoff)
- [Universal lossless shortening is impossible](data-compression.md#universal-lossless-shortening-is-impossible)
- [Verifying a satisfying assignment](theoretical-computer-science.md#verifying-a-satisfying-assignment)
- [Volker Strassen](mathematics.md#volker-strassen)
- [Xiaotie Deng](computer-science.md#xiaotie-deng)
- [Year 1 of the computer science and philosophy course of the University of Oxford](university-of-oxford.md#year-1-of-the-computer-science-and-philosophy-course-of-the-university-of-oxford)
- [Year 2 of the computer science and philosophy course of the University of Oxford](university-of-oxford.md#year-2-of-the-computer-science-and-philosophy-course-of-the-university-of-oxford)
- [Year 2 of the mathematics and computer science course of the University of Oxford](university-of-oxford.md#year-2-of-the-mathematics-and-computer-science-course-of-the-university-of-oxford)
