<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix any structure and any assignment of the three quantified variables, writing their values as $a_0,a_1,a_2$. If either of the nested antecedents is false, the corresponding implication is true. If both are true, then $f^A(a_0)=a_1$ and $f^A(a_0)=a_2$. Actual identity is transitive, so $a_1=a_2$, making the consequent true as well.

Thus the unquantified matrix is true under every assignment in every structure. The universal-quantifier semantic clause then makes its universal closure true in every structure:

$$
\boxed{\models\forall x_0\forall x_1\forall x_2\,[f(x_0)=x_1\to(f(x_0)=x_2\to x_1=x_2)].}
$$

No assumption that $f$ is [injective](../../../../../injective-function.md) is used. The argument says that one value cannot equal two distinct elements, not that distinct inputs have distinct outputs.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the logic and set theory course of the University of Oxford](../../../../split.md)
6. [Logic and set theory course of the University of Oxford](../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
