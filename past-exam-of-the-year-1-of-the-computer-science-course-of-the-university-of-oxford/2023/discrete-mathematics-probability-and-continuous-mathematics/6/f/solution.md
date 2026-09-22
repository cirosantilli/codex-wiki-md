<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**Choose (iii), $|x_{n+1}-x_n|<2000\epsilon$.** Here the root has magnitude between $1000$ and $2000$. [Machine epsilon](../../../../../machine-epsilon.md) measures relative precision near unity; the spacing of representable [floating-point numbers](../../../../../floating-point-number.md) near the root is therefore of order $10^3\epsilon$. A step tolerance scaled to that magnitude is consistent with the attainable absolute positional accuracy. For IEEE binary64, using $\epsilon=2^{-52}$, $2000\epsilon\approx4.44\times10^{-13}$, comparable to the local spacing. A fixed numerical constant cannot promise an exact correctly rounded root, but this is the most sensible of the three proposals.

Condition **(ii)** asks for a step below $2\epsilon$, a scale appropriate near one rather than near this root. A nonzero representable change near the root is normally much larger. The test may trigger only after exact stagnation, and rounding-induced oscillation can prevent that; it asks for unnecessarily fine absolute resolution.

Condition **(i)** measures a residual, not a position error. It changes if the same root problem is multiplied by a constant. Moreover, evaluating $f$ can involve cancellation among quantities of order $1000$, so an absolute residual of order $\epsilon$ need not be meaningful or attainable. Here $1/2<f'(x^*)\le1$, making residual and position errors comparable in exact arithmetic, but their requested absolute scale is still too small. A practical [scale-aware stopping criterion for Newton iteration](../../../../../scale-aware-stopping-criterion-for-newton-iteration.md) should also detect stagnation or a cycle rather than assuming exact arithmetic persists indefinitely.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [6](../../6.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
