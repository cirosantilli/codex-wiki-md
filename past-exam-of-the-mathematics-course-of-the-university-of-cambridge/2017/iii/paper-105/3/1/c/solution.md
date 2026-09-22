<h1 id="3/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

When the velocity depends on $u$, different initial values travel at different speeds. The resulting [characteristic crossing](../../../../../../../characteristic-crossing.md) can destroy a classical solution in finite time, even though the initial function is smooth and bounded. For the [Inviscid Burgers equation](../../../../../../../inviscid-burgers-equation.md), take $u_0(a)=-\tanh a$. Before crossing,

$$
X(t,a)=a-t\tanh a,\qquad u(t,X(t,a))=-\tanh a,
$$

and

$$
u_x(t,X(t,a))=\frac{-\operatorname{sech}^2a}{1-t\operatorname{sech}^2a}.
$$

At $a=0$ this tends to $-\infty$ as $t\uparrow1$, while $|u|\le1$. Thus $\boxed{\text{bounded states can undergo finite-time gradient blow-up and shock formation}.}$ The [bounded-derivative Burgers flux](../../../../../../../bounded-derivative-burgers-flux.md) agrees with this equation on the whole state range, if a global bounded-speed flux is desired. After crossing, arbitrary [weak solutions](../../../../../../../weak-solution.md) need not be unique; an [entropy solution](../../../../../../../entropy-solution.md) condition is needed to select the admissible continuation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [3](../../../3.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
