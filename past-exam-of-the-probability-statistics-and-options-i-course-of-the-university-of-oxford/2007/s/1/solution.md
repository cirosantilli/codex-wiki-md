<h1 id="s/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The first four jobs all have deadlines at most ten, but their total processing time is $2+4+3+2=11$. They cannot all be completed by time ten on one machine, so at least one is late in every schedule.

[Moore's algorithm](../../../../moore-hodgson-algorithm.md) processes jobs in nondecreasing deadline order. Whenever the [electric current](../../../../electric-current.md) on-time list first misses the new job's deadline, remove from that list a job with the largest processing time and put it on the late list. Continue, then append the rejected jobs after the on-time list. The theorem for this algorithm states that it minimizes the number of late jobs when all jobs are initially available.

The source order is already deadline order. The steps are

$$
\begin{array}{c|c|c|c}
\text{job added}&\text{tentative completion}&\text{action}&
\text{on-time list afterward}\\\hline
1&2\leq3&\text{keep}&1\\
2&6\leq7&\text{keep}&1,2\\
3&9\leq9&\text{keep}&1,2,3\\
4&11>10&\text{remove }2\ (p_2=4)&1,3,4\\
5&12\leq13&\text{keep}&1,3,4,5\\
6&16>15&\text{remove }5\ (p_5=5)&1,3,4,6
\end{array}
$$

After the first removal the cumulative time is seven; after the second it is eleven. Append jobs two and five. One optimal schedule is

$$
\boxed{1,3,4,6,2,5,\qquad\text{two late jobs}.}
$$

Its completion times are $2,5,7,11,15,20$. Comparing with the corresponding deadlines verifies that precisely jobs two and five are late. Moore's theorem certifies that no schedule can improve on that number.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [S](../../s.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
