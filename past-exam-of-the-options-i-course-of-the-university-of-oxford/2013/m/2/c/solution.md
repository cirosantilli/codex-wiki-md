<h1 id="m/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [uniform distribution](../../../../../continuous-uniform-distribution.md) on $[0,1]$, the mean is $1/2$ and the [variance](../../../../../variance-split.md) is $1/12$. The [central limit theorem](../../../../../central-limit-theorem.md) for independent identically distributed variables with finite nonzero [variance](../../../../../variance-split.md) gives

$$
Z_n=\frac{S_n-n/2}{\sqrt{n/12}}\ \xrightarrow{d}\ N(0,1).
$$

Choose $\boxed{\alpha=1/2,\quad\beta=1/2}$. Then

$$
\mathbb P(S_n<\alpha n+n^\beta)=\mathbb P(Z_n<\sqrt{12})\longrightarrow\boxed{\Phi(\sqrt{12})}.
$$

The standard normal distribution function is continuous and strictly increasing, so its value at the finite positive number $\sqrt{12}$ is strictly between $1/2$ and one, as required.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [M](../../../m.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
