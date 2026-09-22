<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Along an exact autonomous-ODE solution, $f(y)=y'$ and

$$
g(y)=f'(y)f(y)=y''.
$$

Move every term to the left and substitute the [Taylor expansions](../../../../../../taylor-expansion.md) about $t_n$. The coefficients of $h^jy^{(j)}(t_n)$ vanish for $0\leq j\leq4$, while the first nonzero coefficient is

$$
\frac{2}{165}h^5y^{(5)}(t_n).
$$

Thus the local defect is $O(h^5)$. At $h=0$ the first characteristic polynomial is

$$
\rho(\xi)=\xi^2-\frac{16}{11}\xi+\frac5{11}
=(\xi-1)\left(\xi-\frac5{11}\right),
$$

which satisfies the [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md). The method is therefore zero-stable and has

$$
\boxed{\text{order }4}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
