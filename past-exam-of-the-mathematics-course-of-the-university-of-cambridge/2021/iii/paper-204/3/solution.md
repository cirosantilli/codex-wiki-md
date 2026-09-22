<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For $\omega\in\{0,1\}^{E}$, write $o(\omega)=|\eta(\omega)|$ and $c(\omega)=|E|-o(\omega)$. The [random-cluster model](../../../../../random-cluster-model.md) is

$$
\phi_{p,q}(\omega)=\frac1{Z_{p,q}}p^{o(\omega)}(1-p)^{c(\omega)}q^{k(\omega)}.
$$

For $0\leq p\leq1$ and $q\geq1$, its [positive association of the random-cluster model](../../../../../positive-association-of-the-random-cluster-model.md) states that increasing functions $f,g$ satisfy $\phi_{p,q}(fg)\geq\phi_{p,q}(f)\phi_{p,q}(g)$.

For the two parallel edges $e_1,e_2$, the four unnormalized weights for $00,10,01,11$ are respectively

$$
(1-p)^2q^2,quad p(1-p)q,quad p(1-p)q,quad p^2q.
$$

For the increasing events $A=\{e_1\text{ open}\}$ and $B=\{e_2\text{ open}\}$, positive association is equivalent to $w_{00}w_{11}\geq w_{10}w_{01}$, which reduces to $q\geq1$. It therefore fails whenever $p,q\in(0,1)$.

At $p=1/2$, all factors involving the number of open edges are equal, so the weight is proportional to $q^{k(\omega)}$. The smallest possible component count is one. Dividing numerator and denominator by $q$ and sending $q\downarrow0$ leaves equal weight precisely on connected spanning subgraphs, proving the stated [uniform connected-subgraph limit of the random-cluster model](../../../../../uniform-connected-subgraph-limit-of-the-random-cluster-model.md).

Finally let $p,q\downarrow0$ with $q/p\to0$, and let $N=|V|$. Fix a spanning tree $\tau$. The ratio of the weight of $\omega$ to that of $\tau$ is

$$
\left(\frac{p}{1-p}\right)^{o(\omega)-N+1}q^{k(\omega)-1}
=(1-p)^{N-1-o(\omega)}p^{d(\omega)}\left(\frac qp\right)^{k(\omega)-1},
$$

where $d(\omega)=o(\omega)+k(\omega)-N\geq0$. Equality $d=0$ means that the open graph is a forest. The ratio tends to zero unless $d=0$ and $k=1$, which means precisely that $\omega$ is a spanning tree. All spanning trees have equal weight, so the limiting law is the [uniform spanning-tree limit of the random-cluster model](../../../../../uniform-spanning-tree-limit-of-the-random-cluster-model.md):

$$
\phi_{p,q}(\omega)\longrightarrow
\begin{cases}
1/|\mathcal T|,&\omega\in\mathcal T,\\
0,&\omega\notin\mathcal T,
\end{cases}
$$

where $\mathcal T$ is the set of spanning trees of $G$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 204](../../paper-204-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
