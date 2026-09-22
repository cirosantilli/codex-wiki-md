# Max-flow min-cut theorem

↑ **Parent:** [Flow network](flow-network-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Max-flow_min-cut_theorem)

For a finite [flow network](flow-network-split.md) with finite nonnegative real [flow network edge capacities](flow-network-edge-capacity.md), the greatest [strength of a flow](strength-of-a-flow.md) of a [feasible flow](feasible-flow.md) equals the least [cut capacity](cut-capacity.md) of a source-to-sink [cut of a flow network](cut-of-a-flow-network.md):

$$
\max_{f\text{ feasible}}|f|
=\min_{S\subseteq V:\,s\in S,\,t\notin S}
\sum_{(u,v)\in E:\,u\in S,\,v\notin S}c_{uv}.
$$

For a [maximum flow](maximum-flow-problem.md), the [vertices](vertex-graph-theory.md) reachable from the source in the [residual network](residual-network.md) define a [minimum cut](minimum-cut.md) whose outgoing original [edges](edge-of-a-graph.md) are saturated and whose incoming original [edges](edge-of-a-graph.md) carry zero [flow](flow.md).[Karger, MIT 6.854 Notes 6, maximum-flow optimality conditions](https://courses.csail.mit.edu/6.854/21/Notes/n06-flow.html)

Why is a [cut of a flow network](cut-of-a-flow-network.md) an upper bound? Sum [flow conservation](flow-conservation.md) on its source side $S$. Internal [edge](edge-of-a-graph.md) contributions cancel, leaving

$$
|f|=\sum_{(u,v)\in E:\,u\in S,\,v\notin S}f_{uv}
-\sum_{(u,v)\in E:\,u\notin S,\,v\in S}f_{uv}
\leq\sum_{(u,v)\in E:\,u\in S,\,v\notin S}c_{uv}
=c(S,V\setminus S).
$$

Only directed [edges](edge-of-a-graph.md) leaving $S$ contribute to [cut capacity](cut-capacity.md). Directed [edges](edge-of-a-graph.md) entering $S$ are subtracted in net [flow](flow.md), so adding their capacities to the upper bound would lose the intended bottleneck. This inequality is [weak duality](weak-duality.md); the theorem says the bound is attained, an instance of [strong duality](strong-duality.md). Its beauty is that a routing plan and a separating boundary independently witness each other's optimality.

In the running [flow network](flow-network-split.md), the two internal [vertices](vertex-graph-theory.md) give four possible source sides. For $S=\{s\}$, the [cut capacity](cut-capacity.md) is $c_{sa}+c_{sb}=3+2=5$. For $S=\{s,a\}$ it is $c_{sb}+c_{ab}+c_{at}=2+1+2=5$. For $S=\{s,b\}$ it is $c_{sa}+c_{bt}=3+3=6$; the incoming [edge](edge-of-a-graph.md) $a\to b$ contributes nothing to that [cut capacity](cut-capacity.md). Finally, $S=\{s,a,b\}$ gives $c_{at}+c_{bt}=2+3=5$. Thus the [minimum cut](minimum-cut.md) has [cut capacity](cut-capacity.md) $5$, matching the explicitly computed [maximum flow](maximum-flow-problem.md).

<a id="image-maximum-flow-of-value-five-and-two-minimum-cut-certificates"></a>
![](max-flow-cut-certificate.png)

**[Figure 3](#image-maximum-flow-of-value-five-and-two-minimum-cut-certificates). Maximum flow of value five and two minimum-cut certificates**. Labels show flow/capacity on each directed edge. The shaded source sides give cuts of capacities three plus two and two plus one plus two, both equal to the flow value.

Ford and Fulkerson's 1956 paper opens with a railway-capacity question attributed there to T. Harris and proves a minimal-cut theorem as Theorem 1. Its original formulation uses [graph paths](path-in-a-graph.md) carrying nonnegative amounts; the [residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md) below gives the finite directed [flow network](flow-network-split.md) proof used here.[Ford and Fulkerson, Maximal Flow Through a Network, Canadian Journal of Mathematics 8 (1956), pp. 399–404](https://doi.org/10.4153/CJM-1956-045-5)

**Table of contents**

- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Uniform capacity perturbation of a flow network](uniform-capacity-perturbation-of-a-flow-network.md)
- [Integral max-flow theorem](integral-max-flow-theorem.md)
- [Kőnig's theorem (graph theory)](konig-s-theorem-graph-theory.md)
- [Residual network](residual-network.md)
  - [Residual maximum flow is the remaining optimality gap](residual-maximum-flow-is-the-remaining-optimality-gap.md)
  - [Augmenting path](augmenting-path.md)
    - [Widest augmenting path](widest-augmenting-path.md)
      - [Geometric convergence of widest-path augmentation](geometric-convergence-of-widest-path-augmentation.md)
    - [Ford-Fulkerson algorithm](ford-fulkerson-algorithm.md)
      - [Integrality of the Ford-Fulkerson algorithm](integrality-of-the-ford-fulkerson-algorithm.md)
- [Parametric maximum flow with one source capacity](parametric-maximum-flow-with-one-source-capacity.md)

## ↑ Ancestors (6)

1. [Flow network](flow-network-split.md)
2. [Graph theory](graph-theory-split.md)
3. [Foundations of mathematics](foundations-of-mathematics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (36)

- [Cut capacity](cut-capacity.md)
- [Edmonds–Karp algorithm](edmonds-karp-algorithm.md)
- [Ford-Fulkerson algorithm](ford-fulkerson-algorithm.md)
- [Maximum flow problem](maximum-flow-problem.md)
- [Maximum flow with vertex capacities](maximum-flow-with-vertex-capacities.md)
- [Measurable Hall theorem](measurable-hall-theorem.md)
- [Minimum cut](minimum-cut.md)
- [Outdegree orientation criterion](outdegree-orientation-criterion.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/5h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-4/20d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-40/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/8c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-38/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-37/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/20h/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-109/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/20h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/20h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/17g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-3/19h/a/solution.md)
- [Residual maximum flow is the remaining optimality gap](residual-maximum-flow-is-the-remaining-optimality-gap.md)
- [Residual reachability certificate for maximum flow](residual-reachability-certificate-for-maximum-flow.md)
- [Server connectivity under component failures](server-connectivity-under-component-failures.md)
- [Uniform capacity perturbation of a flow network](uniform-capacity-perturbation-of-a-flow-network.md)
- [Widest augmenting path](widest-augmenting-path.md)
