# Persistence of unsampled graph components

↑ **Parent:** [Achlioptas process](achlioptas-process.md)

Fix positive $\alpha$, $D\geq2$ and $B>0$. Suppose a size band $[k,Dk)$ of an [Achlioptas process](achlioptas-process.md) contains at least $\alpha n$ [vertices](vertex-graph-theory.md) at time $m$. For every fixed $k$, at least $\beta n$ of those [vertices](vertex-graph-theory.md) remain in unchanged [graph components](component-graph-theory.md) throughout the next $T=\lceil Bn/k\rceil$ steps, [with high probability](with-high-probability.md), where one may take $\beta=\alpha e^{-16BD}/4$. This is a deliberately nonoptimal positive constant.

For independent uniform candidate [edges](edge-of-a-graph.md), an initial [graph component](component-graph-theory.md) with $w<Dk$ [vertices](vertex-graph-theory.md) is untouched if none of the $2T$ candidate [edges](edge-of-a-graph.md) meets it. A uniform [edge](edge-of-a-graph.md) hits it with [probability](probability.md) at most $3w/n$. For sufficiently large $n$, $(1-3w/n)^{2T}\geq e^{-16BD}$, so the [expected value](expected-value.md) of the untouched vertex mass $Y$ is at least $\alpha e^{-16BD}n$. Replacing one row of two candidate [edges](edge-of-a-graph.md) can change $Y$ by at most $8Dk$, because only the initial [graph components](component-graph-theory.md) hit by an old or new endpoint can change status. The [McDiarmid inequality](mcdiarmid-s-inequality.md) therefore makes $Y\geq\alpha e^{-16BD}n/2$ except on an event of [probability](probability.md) $e^{-c n/k}$, for a positive constant $c$ depending only on $\alpha,B,D$. An untouched [graph component](component-graph-theory.md) stays unchanged whichever offered [edge](edge-of-a-graph.md) is selected.

For candidates restricted to absent [edges](edge-of-a-graph.md), generate each by an independent uniform proposal stream and reject already present [edges](edge-of-a-graph.md). During any interval of $O(n)$ steps with $O(n)$ present [edges](edge-of-a-graph.md), each proposal has rejection [probability](probability.md) $O(1/n)$ conditional on the past. The number of rejections is at most $O(\log n)$ except on an event of [probability](probability.md) smaller than any inverse power of $n$: if there were $r$ rejections among $2T+r$ proposals, a [union bound](boole-s-inequality.md) over their positions bounds this by $\binom{2T+r}r(C/n)^r$. The first $2T$ proposals are independent and give the previous untouched-mass estimate. Extra proposals can touch at most $2r$ additional initial [graph components](component-graph-theory.md), losing only $O(Dk\log n)=o(n)$ [vertices](vertex-graph-theory.md) for fixed $k$. This leaves the stated $\beta n$ bound. A [union bound](boole-s-inequality.md) makes these estimates simultaneous over starting times $m\leq3n$. They hold through the entire interval, so deterministic or random stopping times within it are allowed.

## ↑ Ancestors (7)

1. [Achlioptas process](achlioptas-process.md)
2. [Random graph](random-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Achlioptas process](achlioptas-process.md)
- [Continuity of fixed-choice percolation](continuity-of-fixed-choice-percolation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/5/ii/solution.md)
