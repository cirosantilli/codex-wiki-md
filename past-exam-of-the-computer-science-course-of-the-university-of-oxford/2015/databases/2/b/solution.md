<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A simple valid [database query plan](../../../../../database-query-plan.md) uses a [block nested-loop join](../../../../../block-nested-loop-join.md) with the salesperson records on the outside, checking both sale conditions during the same inner scan. It avoids materializing the potentially much larger set of matching sale pairs.

- Read a block of salesperson records. Retain each `empid`, its name, and two initially false flags, one for each target price.
- Scan all of `Sales`. Apply [relational selection](../../../../../relational-selection.md) to disregard other prices. For each retained sale, match `salespersonid` against the identifiers in the current outer block, and set the corresponding price flag. Several matching sales only set the same flag again.
- After the inner scan, output the names of outer records with both flags true. Repeat for the next outer block, then eliminate repeated names to implement [set semantics](../../../../../set-semantics.md).

Let $p\leq SPT$ be the actual number of salesperson data pages and $k$ the number of outer data pages that fit along with the flags and working buffers. With the usual convention of $B-2$ outer pages, one inner input page and one output page, take $k=B-2$ for $B\geq3$. If flag storage requires an extra reserved page, reduce $k$ accordingly. The number of outer records is at most $p\,SPR$, and there are $\lceil p/k\rceil$ outer blocks. Every such block requires a complete scan of the $ST$ sales data pages.

Count a [database page](../../../../../database-page.md) read or write as one I/O. Conservatively charge $H_{SP}$ to locate the first salesperson leaf and $H_S$ to locate the start of each inner scan; this permits a small double charge if a definition of height includes a data leaf. The estimated read cost is

$$
\boxed{C_{\mathrm{read}}=H_{SP}+p+\left\lceil\frac{p}{k}\right\rceil(H_S+ST),\qquad p\leq SPT.}
$$

In the common convention that scan startup and cached internal pages are ignored, the usual upper estimate is

$$
\boxed{SPT+\left\lceil\frac{SPT}{B-2}\right\rceil ST.}
$$

For an empty outer input there are no inner scans. This [database query plan](../../../../../database-query-plan.md) requires neither a sorted sale input nor a price index. In particular, the [clustered database index](../../../../../clustered-database-index.md) on `invoiceno` cannot locate records by price. The quantities $TN$ and $THO$ describe the amount of qualifying data; they do not justify replacing a complete scan cost $ST$ by $TN+THO$. They can bound the retained work within each scan by roughly $(TN+THO)SR$ sale records, if those page counts describe packed qualifying records. Comparison cost against the outer block is CPU work rather than additional I/O.

Finally let $D_\delta$ be the extra I/O for eliminating repeated output names, including any temporary writes and reads, and let $w$ be the final result size in [database pages](../../../../../database-page.md) if materialization is required. The total estimate is

$$
\boxed{C=C_{\mathrm{read}}+D_\delta+w.}
$$

If enough additional memory is available to retain all distinct qualifying names while producing the stream, then $D_\delta=0$. This extra memory is an additional assumption, separate from the $B$ join buffers. More generally, for $q$ pages of raw qualifying names, [external merge sort](../../../../../external-merge-sort.md) gives $D_\delta=O\!\left(q\left[1+\log_{B-1}\max\{1,\lceil q/B\rceil\}\right]\right)$ for $B\geq3$, including spooling. Names can be deduplicated during the merges. Counting this work matters because a [database primary key](../../../../../database-primary-key.md) on `empid` does not make names unique. No claim of optimality is needed for this [database query plan](../../../../../database-query-plan.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Databases](../../../databases-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
