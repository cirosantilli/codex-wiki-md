<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [i](../i.md)

Write $h(A,B)=\sup_{a\in A}\operatorname{dist}(a,B)$, so that $\rho(A,B)=\max\{h(A,B),h(B,A)\}$ is the [Hausdorff distance](../../../../../hausdorff-distance.md). Since $X$ is a [bounded set](../../../../../bounded-set.md), there is a finite $M$ with $d(x,y)\leq M$. Nonemptiness of $A,B$ therefore gives $0\leq h(A,B)\leq M$, so $\rho$ is finite. Its symmetry and nonnegativity are immediate, as is $\rho(A,A)=0$.

If $\rho(A,B)=0$, then every $a\in A$ has zero [distance to a set](../../../../../distance-to-a-set.md) $B$. Since $B$ is a [closed set](../../../../../closed-set.md), part (a)(iii) gives $A\subseteq B$. Interchanging the sets gives $B\subseteq A$. Thus $\rho(A,B)=0$ implies $A=B$. Closedness is essential here: without it a set and its [closure](../../../../../closure-topology.md) have [Hausdorff distance](../../../../../hausdorff-distance.md) zero.

For the [triangle inequality](../../../../../triangle-inequality.md), fix $a\in A$ and $\epsilon>0$. The [approximation property of an infimum](../../../../../approximation-property-of-an-infimum.md) supplies $b\in B$ with $d(a,b)<\operatorname{dist}(a,B)+\epsilon$, and then $c\in C$ with $d(b,c)<\operatorname{dist}(b,C)+\epsilon$. Consequently,

$$
\operatorname{dist}(a,C)\leq d(a,c)<\operatorname{dist}(a,B)+h(B,C)+2\epsilon.
$$

Let $\epsilon\downarrow0$ and take the [supremum](../../../../../supremum.md) over $a$ to obtain $h(A,C)\leq h(A,B)+h(B,C)$. Applying this inequality in the reverse direction as well yields

$$
\boxed{\rho(A,C)\leq\rho(A,B)+\rho(B,C)}.
$$

All [metric](../../../../../metric.md) axioms follow. Boundedness was used to ensure finiteness, and closedness to distinguish different sets; neither was needed for the [triangle inequality](../../../../../triangle-inequality.md).

## ↑ Ancestors (13)

1. [i](../i.md)
2. [b](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
