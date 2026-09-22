<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

A [topological space](../../../../../topological-space.md) is [connected](../../../../../connected-space.md) when it is not the union of two disjoint nonempty open subsets. It is [path-connected](../../../../../path-connected-space.md) when every two points $x,y$ can be joined by a [path](../../../../../continuous-path.md), meaning a continuous map $\gamma:[0,1]\to X$ with $\gamma(0)=x$ and $\gamma(1)=y$.

To prove that $[0,1]$ is connected, suppose it had a separation $[0,1]=U\cup V$ with $0\in U$. Let

$$
c=\sup\{x\in[0,1]:[0,x]\subseteq U\}.
$$

Whichever of $U$ or $V$ contains $c$, its relative openness supplies an interval about $c$ that contradicts either the definition of the [supremum](../../../../../supremum.md) or the fact that all points immediately below $c$ lie in $U$. Thus no separation exists.

If $X$ is path-connected and $X=U\cup V$ were a separation, choose $u\in U$ and $v\in V$. A path from $u$ to $v$ would make $[0,1]$ the union of the disjoint nonempty open sets $\gamma^{-1}(U)$ and $\gamma^{-1}(V)$, contradicting the connectedness just proved. Hence

$$
\boxed{\text{path-connected}\Longrightarrow\text{connected}}.
$$

Now let $X\subseteq\mathbb R^n$ be open. Every point $x\in X$ lies in an open ball contained in $X$, and an [open ball](../../../../../open-ball.md) is path-connected by straight line segments. It follows that every [path component](../../../../../path-component.md) of $X$ is open. If there were more than one path component, one component and the union of all the others would separate $X$. Consequently a connected open subset of Euclidean space is path-connected. The converse follows from the preceding implication.

The same argument answers the locally Euclidean question affirmatively. Every point has a neighbourhood homeomorphic to an open subset of $\mathbb R^n$, hence a path-connected open neighbourhood after restricting to a sufficiently small ball. Thus $X$ is [locally path-connected](../../../../../locally-path-connected-space.md), its path components are open, and connectedness forces there to be only one.

For the final example, put

$$
Y=A\cup\bigcup_{n\geq1}C_n.
$$

The set $Y$ is path-connected: each vertical segment $C_n$ meets the horizontal segment $A$. The segment $B$ is also path-connected and lies in the [closure](../../../../../closure-topology.md) of $Y$, because $(1/n,y)\to(0,y)$ for every $y\in[1/2,1]$. A connected set together with a connected subset of its closure is connected, so

$$
\boxed{X=Y\cup B\text{ is connected}}.
$$

It is not path-connected. The image of the first coordinate of any path in $X$ lies in

$$
\{0\}\cup\{1/n:n\geq1\}\cup(0,1]
$$

but, while the path has positive height, its first coordinate lies in the totally disconnected set $\{0\}\cup\{1/n:n\geq1\}$. A path beginning on $B$ cannot leave $x=0$ before reaching height zero, and $X$ contains no point $(0,y)$ with $0\leq y<1/2$. Hence no path joins $B$ to $Y$, and

$$
\boxed{X\text{ is not path-connected}}.
$$

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
