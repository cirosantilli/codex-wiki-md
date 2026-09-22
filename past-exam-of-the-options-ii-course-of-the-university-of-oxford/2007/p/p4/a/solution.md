<h1 id="p/p4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Gershgorin's theorem states that every complex [eigenvalue](../../../../../eigenvalue.md) of a square matrix lies in at least one row disc

$$
D_i=\{z\in\mathbb C:|z-a_{ii}|\le R_i\},\qquad R_i=\sum_{j\ne i}|a_{ij}|.
$$

Let $Av=\lambda v$ with $v\ne0$, and choose an index $i$ where $|v_i|$ is maximal. Its row equation gives

$$
|\lambda-a_{ii}|\,|v_i|=\left|\sum_{j\ne i}a_{ij}v_j\right|\le\sum_{j\ne i}|a_{ij}|\,|v_i|.
$$

Dividing by the positive $|v_i|$ proves $\lambda\in D_i$. This proof applies to complex eigenvectors even when the matrix is real.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
