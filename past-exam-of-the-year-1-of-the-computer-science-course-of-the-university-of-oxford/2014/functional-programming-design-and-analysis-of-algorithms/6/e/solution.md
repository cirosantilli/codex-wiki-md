<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Store `pred[j] = i` whenever a strict improvement sets `D[j] = D[i] + 1`. Initialize predecessors to `NONE`. After the [dynamic programming](../../../../../dynamic-programming.md) pass, return `NONE` if the final position is unreachable; otherwise follow predecessors backwards:

```
route = []
j = n - 1
while j != 0:
    route.append(j)
    j = pred[j]
route.append(0)
reverse(route)
return route
```

Every stored predecessor is smaller than the current index, so reconstruction terminates. Its stored distance is exactly one smaller, so the output has precisely $D[n-1]$ jumps and each jump satisfies its input bound. Therefore $\boxed{\text{store a minimizing predecessor; reverse the predecessor chain from }n-1\text{ to }0}$. Reconstruction takes $O(n)$ additional [time complexity](../../../../../time-complexity.md) and $O(n)$ output space; the total [dynamic programming](../../../../../dynamic-programming.md) bounds remain $\Theta(n^2)$ time and $\Theta(n)$ [space complexity](../../../../../space-complexity.md). Keeping the first predecessor on ties selects one optimal route deterministically.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
