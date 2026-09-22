<h1 id="10/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Sampling at $0.2$ Hz means $\Delta t=5$ s. The target times are therefore **$5$, $10$ and $15$ s**, all within the supplied observation range. For bracketing observations, [linear interpolation](../../../../../../linear-interpolation.md) gives $d(t)=d_i+(d_{i+1}-d_i)(t-t_i)/(t_{i+1}-t_i)$. Thus

$$
\begin{aligned}
d(5)&=5.2+(7.8-5.2)\frac{5-1.2}{6.7-1.2}=6.99636,\\
d(10)&=7.8+(15.5-7.8)\frac{10-6.7}{11.6-6.7}=12.98571,\\
d(15)&=15.5+(8.4-15.5)\frac{15-11.6}{15.3-11.6}=8.97568.
\end{aligned}
$$

The estimated displacements are **$7.00$, $12.99$ and $8.98\,\mu\mathrm m$**. Interpolation assumes approximately linear behavior within each interval; it does not recover any unobserved high-frequency motion.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [10](../../../10.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../split.md)
7. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Earth sciences (geology) course of the University of Oxford](../../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
