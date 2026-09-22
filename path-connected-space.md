# Path-connected space

↑ **Parent:** [Geometry and topology](geometry-and-topology-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Path-connected_space)

A [topological space](topological-space.md) $X$ is [path-connected](path-connected-space.md) if, for every $a,b\in X$, there is a [continuous map](continuous-map.md)

$$
\gamma:[0,1]\longrightarrow X,\qquad\gamma(0)=a,\qquad\gamma(1)=b.
$$

This [continuous path](continuous-path.md) must stay within $X$ for its entire duration. Its parameter need not represent physical time, and [continuity](continuous-function.md) does not require a [derivative](derivative.md) or finite [arc length](arc-length.md). [Munkres, Topology: A First Course, section 3-2, definition on p. 155](https://math.mit.edu/~hrm/palestine/munkres-topology.pdf)

In the [closed interval](closed-real-interval.md) $[0,1]$, any $a,b$ are joined by $\gamma(t)=(1-t)a+tb$. For $a=1/4$ and $b=3/4$, this becomes $\gamma(t)=1/4+t/2$, so $\gamma(0)=1/4$, $\gamma(1/2)=1/2$, and $\gamma(1)=3/4$. All its values stay in $[0,1]$. In the [union](set-union.md) $D=[-2,-1]\cup[1,2]$, however, a [continuous path](continuous-path.md) from $-1$ to $1$ would attain $0$ by the [intermediate value theorem](intermediate-value-theorem.md), although $0\notin D$. Thus $D$ is not [path-connected](path-connected-space.md).

Every [path-connected space](path-connected-space.md) is a [connected space](connected-space.md). Proof outline: if $X=U\cup V$ admitted a [separation of a topological space](separation-of-a-topological-space.md), choose $a\in U$ and $b\in V$. A [continuous path](continuous-path.md) between them would have nonempty [open](open-set.md) [inverse images](preimage.md) $\gamma^{-1}(U),\gamma^{-1}(V)$ with empty [intersection](set-intersection.md) and [union](set-union.md) $[0,1]$. This contradicts the [connectedness](connected-space.md) of that [closed interval](closed-real-interval.md).

The converse fails: the [topologist's sine curve](topologist-s-sine-curve.md) is [connected](connected-space.md) but has two [path components](path-component.md). [Path connectedness](path-connected-space.md) is useful when we need an actual [continuous path](continuous-path.md) of allowed positions, rather than only the absence of a [separation of a topological space](separation-of-a-topological-space.md). For instance, when modelling allowed positions as a [topological space](topological-space.md), membership in the same [path component](path-component.md) answers whether one can move continuously between two positions while remaining in that [topological space](topological-space.md).

**Table of contents**

- [Multiply connected region](multiply-connected-region.md)
- [Reciprocal spiral with its endpoint](reciprocal-spiral-with-its-endpoint.md)
- [Rational comb with a connecting spine](rational-comb-with-a-connecting-spine.md)
- [Polygonal connectivity of a finite-line complement](polygonal-connectivity-of-a-finite-line-complement.md)
- [Plane minus a countable set is path connected](plane-minus-a-countable-set-is-path-connected.md)
- [Continuous path](continuous-path.md)
  - [Path space](path-space.md)
  - [Locally rectifiable path](locally-rectifiable-path.md)
  - [Simple closed curve](simple-closed-curve.md)
    - [Nonseparating curve](nonseparating-curve.md)
  - [Path family](path-family.md)
- [Path component](path-component.md)
- [Locally path-connected space](locally-path-connected-space.md)
  - [Connected locally path-connected spaces are path-connected](connected-locally-path-connected-spaces-are-path-connected.md)
- [Cut point](cut-point.md)

## ↑ Ancestors (4)

1. [Geometry and topology](geometry-and-topology-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Connected space](connected-space.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/4b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/4f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/12e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/11h/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/21g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/2f/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-133/2/a/solution.md)
- [Path component](path-component.md)
- [Path-connected space](path-connected-space.md)
