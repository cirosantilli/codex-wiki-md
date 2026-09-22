# Big O notation

↑ **Parent:** [Real analysis](real-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Big_O_notation)

The statement $f(n)=O(g(n))$ as $n\to\infty$ means there are constants $C>0$ and $N$ such that

$$
\boxed{|f(n)|\le C|g(n)|\qquad\text{for every }n\ge N.}
$$

The same constant must work for all sufficiently large inputs. Near a finite [limit](limit-of-a-function.md) point $a$, replace $n\ge N$ by $0<|x-a|<\delta$ within the domain. [Absolute values](absolute-value.md) allow signed or complex-valued [functions](function-split.md); when discussing nonnegative operation counts they can be omitted.

The notation records an [upper bound](upper-bound-in-a-partially-ordered-set.md), not an exact leading coefficient or necessarily a tight growth order. For example, $3n^2+7n+4=O(n^2)$ because for $n\ge1$ it is at most $14n^2$. It is also $O(n^3)$, a weaker statement. A tight comparison uses [big theta notation](big-theta-notation.md); a ratio tending to one uses [asymptotic equivalence](asymptotic-equivalence.md). Formally $O(g)$ denotes a class of [functions](function-split.md), and writing $f=O(g)$ is conventional shorthand for membership in that class. [MIT 6.006, Demaine, Ku and Solomon, Recitation 1, page 3: asymptotic upper and tight bounds](https://live.ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/c6d8f06c6f11e3342633dec85498f551_MIT6_006S20_r01.pdf)

<a id="image-constants-affect-finite-comparisons-while-normalized-ratios-expose-eventual-growth"></a>
![](asymptotic-growth-constants-and-ratios.png)

**[Figure 14](#image-constants-affect-finite-comparisons-while-normalized-ratios-expose-eventual-growth). Constants affect finite comparisons while normalized ratios expose eventual growth**.

The first panel compares stipulated operation counts $A(n)=1000n$ and $B(n)=n^2$. Although $A$ is linear and $B$ quadratic, $B(n)<A(n)$ for $1\le n<1000$; the ordering reverses beyond their crossing. These are mathematical cost models, not measured runtimes. The [time complexity](time-complexity.md) notation describes the growth of whichever cost function has been specified, whether that function represents a worst-case bound, an average, or another explicit quantity.

The middle panel gives a concrete eventual bound: $n^2+10^5n\le2n^2$ for every $n\ge10^5$. Its normalized ratio approaches one, but the threshold matters. The final panel shows the [asymptotic comparison of exponential functions](asymptotic-comparison-of-exponential-functions.md), with its geometrically shrinking relative difference.

Constants may depend on fixed parameters. For each fixed $\alpha>0$, $f_\alpha(n)=\alpha n$ is $O(n)$ with $C=\alpha$; one constant cannot cover every positive $\alpha$. A [uniform big O bound](uniform-big-o-bound.md) makes this extra quantifier explicit.

The notation was already used in nineteenth-century [number theory](number-theory-split.md). In his 1976 paper, Donald E. Knuth reports Landau identifying Bachmann's 1894 book as the first appearance of $O$ known to him. Knuth's account gives the earlier mathematical setting of a notation now also common in [time complexity](time-complexity.md) analysis. [Knuth, Big Omicron and big Omega and big Theta, 1976, page 19](https://danluu.com/knuth-big-o.pdf)

**Table of contents**

- [Little o notation](little-o-notation.md)
- [Big theta notation](big-theta-notation.md)
- [Uniform big O bound](uniform-big-o-bound.md)

## ↑ Ancestors (5)

1. [Real analysis](real-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (90)

- [Adaptive Euler step doubling for exponential decay](adaptive-euler-step-doubling-for-exponential-decay.md)
- [Adjacency list storage and query costs](adjacency-list-storage-and-query-costs.md)
- [Amortized analysis](amortized-analysis.md)
- [Arithmetic work of the Dirichlet hyperbola method](arithmetic-work-of-the-dirichlet-hyperbola-method.md)
- [Array (data structure)](array-data-structure.md)
- [Asymptotic analysis](asymptotic-analysis.md)
- [Asymptotic equivalence](asymptotic-equivalence.md)
- [Barycentric interpolation formula](barycentric-interpolation-formula.md)
- [Bellman-Ford algorithm](bellman-ford-algorithm.md)
- [Big theta notation](big-theta-notation.md)
- [Binary heap](binary-heap.md)
- [Binary powering multiplication count](binary-powering-multiplication-count.md)
- [Binary search tree](binary-search-tree.md)
- [Bipartite graph](bipartite-graph-split.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
- [Breadth-first search](breadth-first-search.md)
- [Cached cell value](cached-cell-value.md)
- [Circular buffer operation costs](circular-buffer-operation-costs.md)
- [Composite midpoint quadrature rule](composite-midpoint-quadrature-rule.md)
- [Composite Simpson's rule](composite-simpson-s-rule.md)
- [Composite trapezoidal rule](composite-trapezoidal-rule.md)
- [Computational tradeoffs of the kernel trick](computational-tradeoffs-of-the-kernel-trick.md)
- [Conditional expectations algorithm cost](conditional-expectations-algorithm-cost.md)
- [Consistency of a numerical method](consistency-of-a-numerical-method.md)
- [Counting sort](counting-sort.md)
- [Depth-first search](depth-first-search.md)
- [DFS lowpoint](dfs-lowpoint.md)
- [Dijkstra algorithm](dijkstra-algorithm.md)
- [Divide-and-conquer combination cost](divide-and-conquer-combination-cost.md)
- [Divisor summatory function](divisor-summatory-function.md)
- [Dynamic array doubling](dynamic-array-doubling.md)
- [Dynamic programming](dynamic-programming.md)
- [Embedded Runge-Kutta pair](embedded-runge-kutta-pair.md)
- [Factorial recursion and returning frames](factorial-recursion-and-returning-frames.md)
- [Fast Fourier transform](fast-fourier-transform.md)
- [FIFO queue](fifo-queue.md)
- [Fundamental strip of a Mellin transform](fundamental-strip-of-a-mellin-transform.md)
- [Gale-Shapley algorithm](gale-shapley-algorithm.md)
- [Gaussian elimination](gaussian-elimination.md)
- [Gaussian peak behind Stirling's formula](gaussian-peak-behind-stirling-s-formula.md)
- [Hash table resizing](hash-table-resizing.md)
- [Insertion sort](insertion-sort.md)
- [Interval scheduling](interval-scheduling.md)
- [Jackknife bias correction](jackknife-bias-correction.md)
- [Kahn's algorithm](kahn-s-algorithm.md)
- [Karatsuba digit-operation cost](karatsuba-digit-operation-cost.md)
- [Kruskal component merging](kruskal-component-merging.md)
- [Leading Taylor term](leading-taylor-term.md)
- [Linear probing cluster](linear-probing-cluster.md)
- [Linear search comparison count](linear-search-comparison-count.md)
- [Linked list](linked-list.md)
- [Little o notation](little-o-notation.md)
- [Logarithmic energy gain from a Peierls distortion](logarithmic-energy-gain-from-a-peierls-distortion.md)
- [Longest increasing subsequence](longest-increasing-subsequence.md)
- [LU factorization and solve costs](lu-factorization-and-solve-costs.md)
- [Matrix-chain dynamic programming](matrix-chain-dynamic-programming.md)
- [Memoization arithmetic and stack costs](memoization-arithmetic-and-stack-costs.md)
- [Merge algorithm](merge-algorithm.md)
- [Merge sort](merge-sort.md)
- [Multigrid method](multigrid-method-split.md)
- [Neighbour enumeration](neighbour-enumeration.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-309/2/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ia/paper-4/9a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/30j/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1/19/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/15/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/15/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/12/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/12/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/12/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/19/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/10/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/6/d/ii/solution.md)
- [Power iteration direction error](power-iteration-direction-error.md)
- [Radix sort](radix-sort.md)
- [Representation independence](representation-independence.md)
- [Richardson extrapolation](richardson-extrapolation.md)
- [Separate chaining](separate-chaining.md)
- [Singular perturbation](singular-perturbation-split.md)
- [Small rotation commutator](small-rotation-commutator.md)
- [Stable digit sort](stable-digit-sort.md)
- [Stable record placement in counting sort](stable-record-placement-in-counting-sort.md)
- [Tangent plane](tangent-plane.md)
- [Tidal force](tidal-force.md)
- [Time complexity](time-complexity.md)
- [Trace and local volume change](trace-and-local-volume-change.md)
- [Tridiagonal matrix algorithm](tridiagonal-matrix-algorithm.md)
- [Union-find operation bounds](union-find-operation-bounds.md)
