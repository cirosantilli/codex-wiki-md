<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

Since $4^{-1}\equiv16\pmod{21}$ and $2^{-1}\equiv23\pmod{45}$, the two [linear congruences](../../../../../linear-congruence.md) reduce to

$$
x\equiv16\pmod{21},
\qquad
x\equiv25\pmod{45}.
$$

Write $x=16+21k$. The second congruence becomes

$$
21k\equiv9\pmod{45},
$$

or $7k\equiv3\pmod{15}$ after division by three. Since $7^{-1}\equiv13\pmod{15}$, $k\equiv9\pmod{15}$. The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) therefore gives the complete family

$$
\boxed{x\equiv205\pmod{315}}.
$$

The modulus is $\operatorname{lcm}(21,45)=315$ because the compatibility condition modulo their greatest common divisor is satisfied.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
