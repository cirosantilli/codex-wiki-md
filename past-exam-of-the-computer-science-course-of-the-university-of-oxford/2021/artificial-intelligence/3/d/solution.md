<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**A sufficient sequential bound is $T_{\max}=4m+2$ for any physically valid initial and [goal states](../../../../../goal-state.md), assuming every bucket is directly reachable.** A goal must be consistent with the stated one-hand and one-location invariants. No bound can guarantee a satisfying [plan](../../../../../plan.md) for an inconsistent goal, such as requiring the same ball in two buckets simultaneously.

Here is a constructive bound independent of the number of buckets. If the hand initially holds a ball, drop it in the current bucket, costing at most one action. For each ball that should end in a bucket, move to its current bucket, pick it up, move to its target bucket, and drop it: at most four actions per ball, omitting unnecessary actions. If the final state requires a held ball, reserve it for last, move to its current bucket and pick it up, costing at most two more actions. Finally move the arm to its prescribed final location, costing at most one action.

If the final hand is empty, this costs at most $1+4m+1=4m+2$. If it holds a ball, only $m-1$ balls need bucket placement, giving at most $1+4(m-1)+2+1=4m$ for $m\ge1$. Thus the common bound is valid. A partially specified, physically consistent goal can first be completed to a valid target state. For the special goal of putting all balls in one bucket with no specified final arm location, $4m$ is already a sufficient bound.

A separate finite-state check is available: physically valid configurations number

$$
|S|=n\left(n^m+m n^{m-1}\right)=n^m(n+m),
$$

counting an empty hand or the choice of a held ball, and the arm's location. A shortest [plan](../../../../../plan.md) never repeats a state, so $|S|-1$ also bounds a shortest solution whenever one exists. The constructive bound is much smaller.

For an encoding requiring a fixed horizon, permit idle layers, or run [SATPlan](../../../../../satplan.md) through all horizons up to the bound. A [plan](../../../../../plan.md) shorter than $T_{\max}$ need not be padded by arbitrary physical actions. The sequential bound also suffices for a parallel encoding, since a serial [plan](../../../../../plan.md) is a permitted special case.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
