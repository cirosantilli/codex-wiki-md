# Perfect matching

↑ **Parent:** [Matching (graph theory)](matching-graph-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_matching)

A [perfect matching](perfect-matching.md) is a [matching in a graph](matching-graph-theory.md) that covers every [vertex](vertex-graph-theory.md) exactly once. Its [edges](edge-of-a-graph.md) have no shared endpoints, and every [vertex](vertex-graph-theory.md) is an endpoint of one selected [edge](edge-of-a-graph.md). It is useful when a collection must be divided into disjoint pairs with no element left over.

In a [bipartite graph](bipartite-graph.md) with equally many [vertices](vertex-graph-theory.md) on its two sides, a [perfect matching](perfect-matching.md) can assign every person one allowed job and every job one person. The example under [permanent of a matrix](permanent-mathematics.md) has three people and three jobs, with exactly three valid assignments. The blue [edges](edge-of-a-graph.md) below show those three [perfect matchings](perfect-matching.md); a crossing in the drawing is not an extra [vertex](vertex-graph-theory.md).

<a id="image-three-perfect-matchings-pair-every-person-vertex-with-one-job-vertex-along-allowed-edges"></a>
![](permanent-perfect-matching-assignments.png)

**[Figure 34](#image-three-perfect-matchings-pair-every-person-vertex-with-one-job-vertex-along-allowed-edges). Three perfect matchings pair every person vertex with one job vertex along allowed edges**.

Every selected [edge](edge-of-a-graph.md) covers two [vertices](vertex-graph-theory.md), so a [graph](graph-split.md) with an [odd integer](odd-integer.md) number of [vertices](vertex-graph-theory.md) has no [perfect matching](perfect-matching.md). An [even integer](even-number.md) number is necessary but does not guarantee existence: an [isolated vertex](isolated-vertex.md) cannot be covered. A [perfect matching](perfect-matching.md) also need not be unique. For example, the [complete bipartite graph](complete-bipartite-graph.md) $K_{2,2}$ has two [perfect matchings](perfect-matching.md), corresponding to the two ways of assigning two people to two jobs.

Counting all [perfect matchings](perfect-matching.md) is a different question from finding one. For a zero-one [biadjacency matrix](biadjacency-matrix.md) of a balanced [bipartite graph](bipartite-graph.md), the count is its [permanent of a matrix](permanent-mathematics.md). The [nonzero determinant criterion for a perfect matching](perfect-matching-from-a-nonzero-determinant.md) supplies an existence test, but cancellation means that a zero [determinant](determinant.md) does not rule one out.

**Table of contents**

- [Flexible vertex in a balanced bipartite graph](flexible-vertex-in-a-balanced-bipartite-graph.md)
- [Minimum-weight perfect matching](minimum-weight-perfect-matching.md)
- [One-factorization](one-factorization.md)

## ↑ Ancestors (6)

1. [Matching (graph theory)](matching-graph-theory.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (37)

- [Assignment problem](assignment-problem.md)
- [Augmenting path in a matching](augmenting-path-in-a-matching.md)
- [Birkhoff decomposition by support matchings](birkhoff-decomposition-by-support-matchings.md)
- [Configuration model](configuration-model.md)
- [Flexible vertex in a balanced bipartite graph](flexible-vertex-in-a-balanced-bipartite-graph.md)
- [Hall matching of maximal separated sets](hall-matching-of-maximal-separated-sets.md)
- [Hungarian algorithm](hungarian-algorithm.md)
- [Matching generating function](matching-generating-function.md)
- [Minimum-weight perfect matching](minimum-weight-perfect-matching.md)
- [Nested matching criterion for a regular subgraph](nested-matching-criterion-for-a-regular-subgraph.md)
- [Octahedral graph](octahedral-graph.md)
- [One-factorization](one-factorization.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-3/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-11/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/17h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3/17h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-7/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/17f/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2/17f/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/17f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-42/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-3/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-3/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-38/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-212/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/15h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/17g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/17h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-215/3/c/solution.md)
- [Perfect matching](perfect-matching.md)
- [Permanent (mathematics)](permanent-mathematics.md)
- [Short augmenting paths in a dense bipartite graph](short-augmenting-paths-in-a-dense-bipartite-graph.md)
