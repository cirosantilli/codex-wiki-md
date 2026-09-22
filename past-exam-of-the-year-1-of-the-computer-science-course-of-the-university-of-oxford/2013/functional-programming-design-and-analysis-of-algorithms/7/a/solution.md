<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Dynamic programming](../../../../../dynamic-programming.md) specifies a collection of overlapping subproblems, expresses each answer using smaller subproblem answers, and stores answers so each subproblem is solved once. One may fill a table in dependency order or use [memoization](../../../../../memoization.md) to compute only requested entries. The key design choice is a state that retains every feature needed by later decisions.

The [principle of optimality](../../../../../principle-of-optimality.md) says that, after a decision in an optimal solution, the remaining decisions must solve the corresponding residual subproblem optimally. Otherwise, replacing that residual solution by a better one would improve the entire solution. This replacement argument requires the state to describe the residual constraints completely. Its useful form here is

$$
\boxed{\text{optimal value of a state}=\max_{\text{feasible first decisions}}\{\text{immediate value}+\text{optimal residual value}\}.}
$$

The maximization applies to these value-maximization problems; minimization uses the analogous minimum recurrence.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
