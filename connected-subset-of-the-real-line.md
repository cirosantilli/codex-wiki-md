# Connected subset of the real line

↑ **Parent:** [Connected space](connected-space.md)

In the usual [subspace topology](subspace-topology.md) from the [real line](real-line.md), a [subset](subset.md) $A\subseteq\mathbb R$ is [connected](connected-space.md) exactly when it has the defining property of a [real interval](interval-mathematics.md):

$$
a,b\in A,\qquad a<c<b\quad\Longrightarrow\quad c\in A.
$$

Every [real number](real-number.md) between two members must be present. Thus [open intervals](open-interval.md), [closed intervals](closed-real-interval.md), intervals with only one endpoint included, and unbounded [real intervals](interval-mathematics.md) are [connected](connected-space.md). [Singleton sets](singleton-mathematics.md) are [connected](connected-space.md) too. With the no-[separation of a topological space](separation-of-a-topological-space.md) convention used here, the [empty set](empty-set.md) satisfies the same property; some texts reserve the word [connected](connected-space.md) for nonempty [topological spaces](topological-space.md).[p. 68, and Proposition C2.6, p. 73: the nonempty convention and the interval characterization](general-topology-by-tom-leinster.md)

Removing an interior point changes the answer:

$$
[-2,2]\setminus\{0\}=[-2,0)\cup(0,2].
$$

These two [real intervals](interval-mathematics.md) are exactly its [connected components](connected-component.md) and its [path components](path-component.md). Removing an endpoint instead leaves a [real interval](interval-mathematics.md), for example $[-2,2]\setminus\{2\}=[-2,2)$, which stays [connected](connected-space.md). This is why an interior point of a [closed interval](closed-real-interval.md) is a [cut point](cut-point.md), whereas an endpoint is not. A nonempty [finite set](finite-set.md) of points in the [real line](real-line.md) is [connected](connected-space.md) exactly when it is a [singleton set](singleton-mathematics.md).

Proof outline: if $a,b\in A$ but $c\in(a,b)$ is missing, the [subsets](subset.md)

$$
A\cap(-\infty,c),\qquad A\cap(c,\infty)
$$

give a [separation of a topological space](separation-of-a-topological-space.md), since the two [open intervals](open-interval.md) make both pieces [open](open-set.md) in $A$. Conversely, a nonempty [real interval](interval-mathematics.md) contains the [continuous path](continuous-path.md) $t\mapsto(1-t)a+tb$ between any two of its points, so it is [path-connected](path-connected-space.md) and hence [connected](connected-space.md). Together with [continuous image of a connected space](continuous-image-of-a-connected-space.md), this characterization gives the [intermediate value theorem](intermediate-value-theorem.md): a [continuous function](continuous-function.md) on a [real interval](interval-mathematics.md) cannot jump over a value lying between two attained values.

## ↑ Ancestors (5)

1. [Connected space](connected-space.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Connected component](connected-component.md)
- [Connected space](connected-space.md)
- [Continuous image of a connected space](continuous-image-of-a-connected-space.md)
- [Derivative criterion for monotonicity](derivative-criterion-for-monotonicity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2/4g/b/solution.md)
