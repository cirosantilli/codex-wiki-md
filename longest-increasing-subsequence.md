# Longest increasing subsequence

↑ **Parent:** [Increasing subsequence](increasing-subsequence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Longest_increasing_subsequence)

A [longest increasing subsequence](longest-increasing-subsequence.md) is an [increasing subsequence](increasing-subsequence.md) of [maximum](maximum-of-a-subset-of-a-total-order.md) length. Write that length as $L(x)$, with $L(())=0$ for the empty [sequence](sequence.md); a nonempty input has $1\leq L(x)\leq n$. Several selections can attain the same [maximum](maximum-of-a-subset-of-a-total-order.md). Here $L$ uses the weak convention $\leq$; write $L_{<}(x)$ for the [maximum](maximum-of-a-subset-of-a-total-order.md) length of a [strictly increasing subsequence](strictly-increasing-subsequence.md). For $(2,2,2)$, these lengths are three and one respectively; for an input with distinct values they agree.

For $x=(4,1,3,2,2,5,0)$, the answer is $L(x)=4$, attained at indices $(2,4,5,6)$, while $L_{<}(x)=3$. One useful interpretation is the smallest number of deletions needed to make the surviving [sequence](sequence.md) nondecreasing:

$$
\text{minimum deletions}=n-L(x).
$$

Indeed, keeping a [longest increasing subsequence](longest-increasing-subsequence.md) attains this bound, and any valid remaining [sequence](sequence.md) is an [increasing subsequence](increasing-subsequence.md), so cannot have more than $L(x)$ terms. In this example the answer is $7-4=3$. This makes $L(x)$ a measure of how much order can be recovered without moving any observation.

**A table that ends at each position.** Let $d_i$ be the [maximum](maximum-of-a-subset-of-a-total-order.md) length of an [increasing subsequence](increasing-subsequence.md) ending specifically at position $i$. The [dynamic programming](dynamic-programming.md) [recurrence relation](recurrence-relation.md) is

$$
d_i=1+\max\bigl(\{0\}\cup\{d_j:1\leq j<i,\ x_j\leq x_i\}\bigr),\qquad L(x)=\max_{1\leq i\leq n}d_i\quad(n>0).
$$

The zero covers a selection consisting only of $x_i$. Otherwise its penultimate index is an eligible $j$; append $x_i$ to an optimal selection ending there. Fill entries in increasing index order. For [strictly increasing subsequences](strictly-increasing-subsequence.md), change the comparison to $x_j<x_i$. The strict version and reconstruction are developed in [University of Toronto, CSC373 tutorial 4 solutions (2018), exercise 2](https://www.cs.toronto.edu/~jepson/csc373/tutNotes/tutEx_DynProg_Soln.pdf); the weak version follows by allowing equality at the append step.

In the worked input, the weak table is $(1,1,2,2,3,4,1)$ and the strict table is $(1,1,2,2,2,3,1)$. At the second $2$, equality extends the first $2$ in the weak table. The final entry is only one, although the optimum is four: the best [increasing subsequence](increasing-subsequence.md) need not finish at the last input position. Record a maximizing predecessor $p_i=j$ whenever $d_i>1$. Following these stored indices from any position maximizing $d_i$, then reversing them, gives an actual [longest increasing subsequence](longest-increasing-subsequence.md). For the weak example the backward chain is $6,5,4,2$.

<a id="image-skipping-positions-and-allowing-equal-values-changes-the-optimum"></a>
![](increasing-subsequence-dp-witness.png)

**[Figure 7](#image-skipping-positions-and-allowing-equal-values-changes-the-optimum). Skipping positions and allowing equal values changes the optimum**. An original toy input, not measured data. The colored selection keeps indices $2,4,5,6$ and values $1,2,2,5$. The two [dynamic programming](dynamic-programming.md) rows give the best lengths ending at every position; the backward arrows reconstruct the weak [longest increasing subsequence](longest-increasing-subsequence.md).

Scanning all earlier positions for each $i$ uses [time complexity](time-complexity.md) $O(n^2)$ and [space complexity](space-complexity.md) $O(n)$ for lengths and predecessors, using [Big O notation](big-o-notation.md) and assuming constant-time comparisons and operations on indices.

**Keep the easiest ending to extend.** The faster [algorithm](algorithm-split.md) maintains a [minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md): $T_\ell$ is the smallest final value of any length-$\ell$ [increasing subsequence](increasing-subsequence.md) in the processed prefix. For equal lengths, a smaller ending permits every future extension allowed by a larger ending. Thus only one best ending per length is needed. The table is nondecreasing, since removing the last term of a length-$(\ell+1)$ selection gives $T_\ell\leq T_{\ell+1}$. Start with an empty table. On reading $v=x_i$, use [binary search](binary-search.md) to find the first entry strictly greater than $v$: replace it by $v$, or append $v$ if there is no such entry. Its position is one beyond the longest existing length whose ending is at most $v$. See [Liben-Nowell, Vee and Zhu, section 3.1 and Figure 1](https://cs.carleton.edu/faculty/dlibenno/papers/lis-lcs/lislcs.pdf).

Duplicates determine the [binary search](binary-search.md) rule: weak increase replaces the first $T_\ell>v$, whereas strict increase replaces the first $T_\ell\geq v$. In Python these positions are returned by `bisect_right(T, v)` and `bisect_left(T, v)` respectively, counting positions from zero. Replace an entry or append; do not insert and shift the remaining entries. The documented equality rules are in [Python documentation, bisect\_left and bisect\_right](https://docs.python.org/3/library/bisect.html). Each search takes $O(\log(n+1))$ comparisons, giving [time complexity](time-complexity.md) $O(n\log(n+1))$, conventionally $O(n\log n)$ for $n\geq2$, and [space complexity](space-complexity.md) $O(L(x))$ for the weak length alone.

<a id="image-two-binary-search-tie-rules-give-different-minimum-tail-tables"></a>
![](increasing-subsequence-tails-trace.png)

**[Figure 8](#image-two-binary-search-tie-rules-give-different-minimum-tail-tables). Two binary-search tie rules give different minimum-tail tables**. Original exact traces for the same toy input, not measured data. Each cell shows a tail value and the input index supplying it; the outlined cell was updated in that row. At the second $2$, the weak [algorithm](algorithm-split.md) appends and the strict [algorithm](algorithm-split.md) replaces. The final weak table has length four, but its supplier indices $7,4,5,6$ are not in increasing order.

**A length certificate needs separate reconstruction.** The final weak tail values are $(0,2,2,5)$, but they do not form an [increasing subsequence](increasing-subsequence.md) of this input: the zero occurs last. Each table entry certifies a selection of its own length; the entries need not come from one compatible selection. To recover a [longest increasing subsequence](longest-increasing-subsequence.md) during the fast [algorithm](algorithm-split.md), store a supplier index $q_\ell$ for each tail and a predecessor index for each input position. Before replacing slot $r$, save $p_i=q_{r-1}$, or no predecessor if $r=1$, then set $q_r=i$. Later replacements leave saved $p_i$ unchanged. Follow predecessors from the final $q_{L(x)}$ and reverse. This uses [space complexity](space-complexity.md) $O(n)$ and returns indices $(2,4,5,6)$ for the weak trace. The same construction works with the strict comparator; compare the two auxiliary arrays in [CP Algorithms contributors, restoring the subsequence after binary search](https://cp-algorithms.com/dynamic_programming/longest_increasing_subsequence.html#restoring-the-subsequence_1).

**Deleting or changing one term.** If $x^{\setminus k}$ deletes position $k$, then

$$
L(x)-1\leq L(x^{\setminus k})\leq L(x).
$$

Deleting cannot create a longer [increasing subsequence](increasing-subsequence.md); removing position $k$ from a previously optimal selection loses at most one term. If $x'$ instead changes just the value at position $k$, both inputs have the same deleted [sequence](sequence.md), so their lengths each lie between its length and its length plus one. Consequently $|L(x')-L(x)|\leq1$. These bounds also hold for [strictly increasing subsequences](strictly-increasing-subsequence.md). In the weak example, deleting either $2$ lowers the length to three, while deleting the final zero leaves it four. This is a [Lipschitz bound](lipschitz-bound.md) for single-term edits, regardless of the numerical size of a replacement. Insertion has the same bound by reversing deletion, so $m$ insertions, deletions or replacements can change $L$ by at most $m$.

For historical context, [Fredman, On computing the length of longest increasing subsequences (1975)](https://doi.org/10.1016/0012-365X(75)90103-X) studies the comparison count for distinct elements of a [totally ordered set](totally-ordered-set.md). Its distinctness assumption makes the weak and strict conventions coincide. No distinctness assumption is needed for the comparator-specific [algorithms](algorithm-split.md) above.

**Table of contents**

- [Minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md)

## ↑ Ancestors (5)

1. [Increasing subsequence](increasing-subsequence.md)
2. [Combinatorics](combinatorics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Increasing subsequence](increasing-subsequence.md)
- [Increasing-subsequence certificate concentration](increasing-subsequence-certificate-concentration.md)
- [Longest increasing subsequence](longest-increasing-subsequence.md)
- [Minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-103/6/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-208/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-208/4/b/solution.md)
- [Robinson–Schensted correspondence](robinson-schensted-correspondence.md)
- [Strictly increasing subsequence](strictly-increasing-subsequence.md)
