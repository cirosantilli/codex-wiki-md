# Convergence of a zero-stable multiderivative method

↑ **Parent:** [Multiderivative multistep method](multiderivative-multistep-method.md)

For a fixed-step [multiderivative multistep method](multiderivative-multistep-method.md), the ordinary [zero-stability](zero-stability.md) root condition still controls propagation of the starting errors when all derivative evaluation maps are uniformly [Lipschitz continuous](lipschitz-continuity.md) on the relevant bounded region. A local defect $O(h^{p+1})$ then yields global error $O(h^p)$ over a fixed time interval, provided the starting errors are $O(h^p)$ and the implicit updates use the nearby solution branch.

For example, writing the numerical error equation as $\rho(E)e_n=hF_h(e_{n+s})+d_n$, with $F_h$ uniformly [Lipschitz continuous](lipschitz-continuity.md), a bounded impulse response for the [root condition for a multistep method](root-condition-for-a-multistep-method.md) gives

$$
\max_{j\leq n}\|e_j\|
\leq C\left(\max_{j<s}\|e_j\|+\sum_{j<n}\|d_j\|\right)
+Ch\sum_{j\leq n}\max_{i\leq j}\|e_i\|.
$$

Absorbing the last current-step term for small $h$ and applying the [discrete Gronwall inequality](discrete-gronwall-inequality.md) gives the stated order. The higher derivatives enter through $F_h$, whose bound stays uniform as $h\to0$.

## ↑ Ancestors (7)

1. [Multiderivative multistep method](multiderivative-multistep-method.md)
2. [Linear multistep method](linear-multistep-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/1/a/solution.md)
