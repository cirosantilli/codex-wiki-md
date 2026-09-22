<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Start with every [state](../../../../../state-computer-science.md), and repeatedly discard a [state](../../../../../state-computer-science.md) that is outside $A=\operatorname{Sat}(\Phi)$ or has any successor outside the current candidate [set](../../../../../set-split.md). Use a fresh [set](../../../../../set-split.md) on each iteration so that the displayed procedure computes exactly $H(X)$:
```
function Sat_AG(S, Post, A):
    X = copy(S)
    repeat:
        Y = empty_set()
        for s in S:
            if s in A and every t in Post(s) belongs to X:
                insert s into Y
        if Y == X:
            return X
        X = Y
```
This is [fixed-point iteration](../../../../../fixed-point-iteration.md) $X_0=S$, $X_{i+1}=H(X_i)$. The first step gives $X_1=A$, because every successor is a [state](../../../../../state-computer-science.md) of $S$. Thus $X_1\subseteq X_0$. If $X_i\subseteq X_{i-1}$, the [order-preserving function](../../../../../order-preserving-function.md) property gives

$$
X_{i+1}=H(X_i)\subseteq H(X_{i-1})=X_i.
$$

The candidate [sets](../../../../../set-split.md) therefore form a descending chain under [set inclusion](../../../../../set-inclusion.md).

Every [fixed point](../../../../../fixed-point.md) $Z$ is contained in every $X_i$: initially $Z\subseteq S$, and $Z\subseteq X_i$ implies $Z=H(Z)\subseteq H(X_i)=X_{i+1}$. At return, $X=H(X)$, and $X$ contains every [fixed point](../../../../../fixed-point.md). The returned [set](../../../../../set-split.md) is consequently the [greatest fixed point](../../../../../greatest-fixed-point.md), so $\boxed{X=\operatorname{Sat}(\forall\square\Phi)}$ by part (d).

The iteration also has a direct interpretation. $X_1$ contains precisely the [states](../../../../../state-computer-science.md) satisfying $\Phi$ now; $X_2$ retains those satisfying it now and at all immediate successors; later rounds extend the checked horizon one step at a time. The stable [set](../../../../../set-split.md) enforces the condition at every future position.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
