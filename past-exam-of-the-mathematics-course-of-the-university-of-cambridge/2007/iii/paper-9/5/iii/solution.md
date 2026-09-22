<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since [Lipschitz functions](../../../../../../lipschitz-continuity.md) are continuous, the feasible class here is smaller, giving $m_L\leq m_d$. To prove the reverse inequality, take any continuous feasible pair $f,g$ and perform [Lipschitz regularization of transport potentials](../../../../../../lipschitz-regularization-of-transport-potentials.md):

$$
h(x)=\min_{y\in X}\{d(x,y)-g(y)\}.
$$

The minimum exists by [compactness](../../../../../../compact-space.md). For every $x,x'$ the [triangle inequality](../../../../../../triangle-inequality.md) gives $h(x)\leq d(x,x')+h(x')$; interchanging $x,x'$ proves $|h(x)-h(x')|\leq d(x,x')$. Thus $h$ has [Lipschitz constant](../../../../../../lipschitz-constant.md) at most $1$.

The original constraint yields $f(x)\leq h(x)$, and evaluating the minimum at $y=x$ gives $h(x)\leq-g(x)$. Moreover, $h(x)-h(y)\leq d(x,y)$, so $(h,-h)$ is a feasible [Lipschitz](../../../../../../lipschitz-continuity.md) pair with

$$
\int f\,dP+\int g\,dQ\leq\int h\,dP-\int h\,dQ\leq m_L.
$$

Taking the supremum over the original continuous pairs proves **$m_L(P,Q)=m_d(P,Q)=W(P,Q)$**. Notice that this is an exact regularization, with no density or approximation assumption about the initial pair.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
