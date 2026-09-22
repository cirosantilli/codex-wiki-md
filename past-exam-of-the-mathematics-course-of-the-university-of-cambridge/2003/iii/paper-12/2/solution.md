<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Couple the [uniform random graph process](../../../../../uniform-random-graph-process.md) by giving every possible [edge](../../../../../edge-of-a-graph.md) an independent uniform label in $[0,1]$ and revealing them in increasing order. The [graph](../../../../../graph-split.md) at label threshold $p$ is a [binomial random graph](../../../../../binomial-random-graph.md). Define $\tau_0$ as the first step with no [isolated vertices](../../../../../isolated-vertex.md) and $\tau_c$ as the first [connected graph](../../../../../connected-graph.md). Deterministically $\tau_c\geq\tau_0$. We prove the reverse inequality [with high probability](../../../../../with-high-probability.md) by tracking the same process through a short interval.

Put $w=\tfrac14\log\log n$, $p_\pm=(\log n\pm w)/n$, and $L=np_-$. At $p_-$ the [isolated vertex](../../../../../isolated-vertex.md) count $Z$ has

$$
\mathbb EZ=n(1-p_-)^{n-1}\sim e^w\longrightarrow\infty,\qquad \frac{\operatorname{Var}Z}{(\mathbb EZ)^2}\leq\frac1{\mathbb EZ}+\frac{p_-}{1-p_-}\longrightarrow0.
$$

The variance estimate follows by comparing two isolated-vertex indicators, whose joint-to-product probability ratio is $(1-p_-)^{-1}$. Thus $Z>0$ [with high probability](../../../../../with-high-probability.md). Also the [Markov inequality](../../../../../markov-inequality.md) gives $Z\leq\log n$ with probability tending to one.

At this same threshold, exclude every [graph component](../../../../../component-graph-theory.md) with order $2\leq s\leq n/2$. For $2\leq s\leq n/\log n$, any such component contains a [spanning tree](../../../../../spanning-tree.md). The [Cayley formula](../../../../../cayley-s-formula.md) and a [union bound](../../../../../boole-s-inequality.md) therefore give

$$
\Pr(\text{an }s\text{-vertex component exists})\leq\binom ns s^{s-2}p_-^{s-1}(1-p_-)^{s(n-s)}\leq\frac{n}{Ls^2}\left(eL e^{-L(1-s/n)}\right)^s.
$$

In this range the bracket is at most $A=e^2Le^w/n=o(1)$. Summing over $s\geq2$ gives $O(nA^2/L)=O(Le^{2w}/n)=o(1)$. For $n/\log n<s\leq n/2$, even the cut-absence bound is enough:

$$
\binom ns(1-p_-)^{s(n-s)}\leq\left(\frac{en}{s}e^{-L/2}\right)^s\leq\left(e\log n\,n^{-1/2}e^{w/2}\right)^s.
$$

The bracket tends to zero, so this range also has total [probability](../../../../../probability.md) $o(1)$. Consequently the graph at $p_-$ consists of one component of order greater than $n/2$ and its isolated-vertex set $S$, where $1\leq|S|\leq\log n$ [with high probability](../../../../../with-high-probability.md).

Conditional on the entire graph at $p_-$, every unrevealed edge label remains independently uniform on $(p_-,1)$. In particular,

$$
\Pr(\text{an edge within }S\text{ appears by }p_+\mid G(p_-))\leq\binom{|S|}{2}\frac{p_+-p_-}{1-p_-}=O\left(\frac{(\log n)^2\log\log n}{n}\right)=o(1).
$$

There are no [isolated vertices](../../../../../isolated-vertex.md) at $p_+$ [with high probability](../../../../../with-high-probability.md), because their [expected value](../../../../../expected-value.md) is asymptotic to $e^{-w}\to0$. On the intersection of these events, each vertex of $S$ loses isolation by joining the original large component, never by forming a separate small component with another vertex of $S$. At every step between these two thresholds there is therefore one nontrivial component and some isolated vertices. The final isolated vertex disappears precisely when the graph becomes connected. This proves the [connectivity hitting time equals disappearance of isolated vertices](../../../../../connectivity-hitting-time-equals-disappearance-of-isolated-vertices.md) result:

$$
\boxed{\Pr(\tau_c=\tau_0)\longrightarrow1.}
$$

For the critical-window probability, let $p=(\log n+\alpha(n))/n$ with $|\alpha(n)|\leq B$. For each fixed $j$, the [falling factorial](../../../../../falling-factorial.md) moment of the isolated-vertex count is

$$
\mathbb E(Z)_j=(n)_j(1-p)^{j(n-j)+\binom j2}=e^{-j\alpha(n)}+o(1),
$$

uniformly for such shifts. Apply the [Bonferroni inequalities](../../../../../bonferroni-inequalities.md) to the zero-count event. Its odd and even truncations bracket $\Pr(Z=0)$ by partial sums of $\sum_{j\geq0}(-1)^je^{-j\alpha(n)}/j!$. Since $e^{-\alpha(n)}\leq e^B$, their remainders tend uniformly to zero. Hence $\Pr(Z=0)=e^{-e^{-\alpha(n)}}+o(1)$. The process equality just proved changes this probability by at most its $o(1)$ failure probability. Therefore

$$
\boxed{\Pr(G_{n,p}\text{ connected})=e^{-e^{-\alpha(n)}}+o(1),\qquad \frac{\Pr(G_{n,p}\text{ connected})}{e^{-e^{-\alpha(n)}}}\longrightarrow1.}
$$

The ratio follows because the denominator is bounded below by $e^{-e^B}>0$; no convergence of $\alpha(n)$ is needed.

**The printed second conclusion has the complementary denominator and is false as written.** For $\alpha(n)=0$, the printed ratio tends to $e^{-1}/(1-e^{-1})=1/(e-1)\ne1$. Its denominator $1-e^{-e^{-\alpha(n)}}$ is correct for the probability of being disconnected. Thus either remove the leading $1-$ in the denominator or replace “connected” by “disconnected”; the proof supplies both corrected versions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
