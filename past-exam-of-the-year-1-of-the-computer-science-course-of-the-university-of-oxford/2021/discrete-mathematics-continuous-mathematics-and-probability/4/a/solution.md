<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the standard spacing convention for [machine epsilon](../../../../../machine-epsilon.md): the next representable [floating-point number](../../../../../floating-point-number.md) above $1$ is $1+2^{-40}$. In a normalized binary representation this corresponds to $41$ significant binary digits, including the leading digit. The spacing throughout $[1,2)$ is therefore $2^{-40}$.

With [rounding](../../../../../rounding.md) to nearest, the associated [unit roundoff](../../../../../unit-roundoff.md) is half that spacing, $u=2^{-41}$; for a normal result the relative [round-off error](../../../../../round-off-error.md) is bounded by $u$. Some texts instead call $u$ machine epsilon. **Here $2^{-40}$ denotes the spacing scale**, and the iteration counts below use that convention. It describes representation precision, not a guarantee that an arbitrarily evaluated [function](../../../../../function-split.md) has a relative error this small.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
