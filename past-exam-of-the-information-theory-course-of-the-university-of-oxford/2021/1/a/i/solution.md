<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [chain rule for conditional entropy](../../../../../chain-rule-for-conditional-entropy.md) gives

$$
H(X,Y\mid Z)-H(X\mid Z)=H(Y\mid X,Z)\geq0.
$$

Indeed, for every conditioning value $(x,z)$ of positive [probability](../../../../../probability.md), each summand $-p(y\mid x,z)\log_2p(y\mid x,z)$ is nonnegative. Its sum is zero exactly when the [conditional probability mass function](../../../../../conditional-probability-mass-function.md) is concentrated at one value. Averaging over $(X,Z)$ therefore proves both the inequality and its equality criterion: **equality holds exactly when $Y=f(X,Z)$ [almost surely](../../../../../almost-sure-convergence.md) for some function $f$.** Conditioning values of [probability](../../../../../probability.md) zero impose no restriction. This is a statement about [discrete random variables](../../../../../discrete-random-variable.md); a [differential entropy](../../../../../differential-entropy.md) need not be nonnegative.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the information theory course of the University of Oxford](../../../../split.md)
6. [Information theory course of the University of Oxford](../../../../../information-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
