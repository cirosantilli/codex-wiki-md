<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Prove both identities by [mathematical induction](../../../../../mathematical-induction.md). The base case $n=2$ is the two-set form of [De Morgan's laws](../../../../../de-morgan-s-laws.md). For the [union](../../../../../set-union.md) identity, suppose the result holds for $n$. Applying the two-set identity and then the [inductive hypothesis](../../../../../induction-hypothesis.md) gives

$$
\begin{aligned}
A\setminus\bigcup_{i=1}^{n+1}B_i
&=\left(A\setminus\bigcup_{i=1}^{n}B_i\right)\cap(A\setminus B_{n+1})\\
&=\left(\bigcap_{i=1}^{n}(A\setminus B_i)\right)\cap(A\setminus B_{n+1})
=\bigcap_{i=1}^{n+1}(A\setminus B_i).
\end{aligned}
$$

For the [intersection](../../../../../set-intersection.md) identity, the corresponding step is

$$
\begin{aligned}
A\setminus\bigcap_{i=1}^{n+1}B_i
&=\left(A\setminus\bigcap_{i=1}^{n}B_i\right)\cup(A\setminus B_{n+1})\\
&=\left(\bigcup_{i=1}^{n}(A\setminus B_i)\right)\cup(A\setminus B_{n+1})
=\bigcup_{i=1}^{n+1}(A\setminus B_i).
\end{aligned}
$$

These close the two inductions.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
