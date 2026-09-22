<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $R(z)=\tfrac14(\wp''/\wp')^2-2\wp(z)$. This is an [elliptic function](../../../../../elliptic-function.md). Its only possible poles modulo $\Lambda$ are $0$ and the three simple zeros $h$ of $\wp'$. At such a nonzero half-period, periodicity and evenness give $\wp(h+t)=\wp(h-t)$, so

$$
\wp'(h+t)=At+O(t^3),\quad A\ne0,
\qquad \frac{\wp''(h+t)}{\wp'(h+t)}=\frac1t+O(t).
$$

It follows that $R(h+t)=1/(4t^2)+O(1)$ with no simple-pole term. This is exactly the principal part of $\wp(2h+2t)=\wp(2t)$.

At zero the source expansion yields

$$
\wp=z^{-2}+O(z^2),\quad\wp'=-2z^{-3}+O(z),\quad
\wp''=6z^{-4}+O(1),\quad\wp''/\wp'=-3z^{-1}+O(z^3).
$$

Consequently $R(z)=1/(4z^2)+O(z^2)$, again matching $\wp(2z)$. Thus $R(z)-\wp(2z)$ is a [holomorphic function](../../../../../holomorphic-function-split.md) on a compact connected [Riemann surface](../../../../../riemann-surfaces-split.md), hence constant. Its limit at zero is zero, proving

$$
\boxed{\wp(2z)=\frac14\left(\frac{\wp''(z)}{\wp'(z)}\right)^2-2\wp(z).}
$$

The equality extends over the apparent singularities as an identity of [meromorphic functions](../../../../../meromorphic-function.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the geometry course of the University of Oxford](../../../../split.md)
6. [Geometry course of the University of Oxford](../../../../../geometry-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
