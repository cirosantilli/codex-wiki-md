# Integer rounding in a divide-and-conquer recurrence

↑ **Parent:** [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)

An integer-valued problem size requires integer subproblem sizes and a base case. For the displayed unequal split with $n\geq2$, both children have positive size less than $n$, and $1/4\leq m/n\leq1/2$. The [entropy potential for a divide-and-conquer recurrence](entropy-potential-for-a-divide-and-conquer-recurrence.md) therefore supplies a uniform positive potential decrease. The squared sizes satisfy $m^2+(n-m)^2\leq5n^2/8$, which similarly closes a quadratic [inductive hypothesis](induction-hypothesis.md) when the work at the root is $n^2$.

## ↑ Ancestors (4)

1. [Divide-and-conquer algorithm](divide-and-conquer-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/discrete-mathematics-continuous-mathematics-and-probability/3/e/i/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2014/discrete-mathematics-continuous-mathematics-and-probability/3/e/ii/solution.md)
