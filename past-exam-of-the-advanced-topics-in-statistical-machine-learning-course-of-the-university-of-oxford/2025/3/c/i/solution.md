<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use only the first $n-1$ observations to define

$$
\begin{aligned}
A&=(k(x_i,x_j))_{i,j<n}+\sigma^2I_{n-1},&
 b&=(k(x_i,x_n))_{i<n},\\
a&=(k(x_i,x_*))_{i<n},&
 c&=k(x_n,x_n)+\sigma^2,\\
d&=k(x_n,x_*),&k_{**}&=k(x_*,x_*).
\end{aligned}
$$

Thus the full noisy [covariance matrix](../../../../../covariance-matrix.md) is $C_n=\begin{pmatrix}A&b\\b^T&c\end{pmatrix}$ and the full cross-covariance [vector](../../../../../vector.md) is $(a^T,d)^T$. Set

$$
s=c-b^TA^{-1}b,\qquad M=s^{-1}.
$$

The scalar $s$ is the [Schur complement](../../../../../schur-complement.md) of $A$. Substituting the block inverse into the [Gaussian process regression posterior](../../../../../gaussian-process-regression-posterior.md) [variance](../../../../../variance-split.md) gives

$$
\begin{aligned}
v_n(x_*)&=k_{**}-\begin{pmatrix}a^T&d\end{pmatrix}C_n^{-1}\begin{pmatrix}a\\d\end{pmatrix}\\
&=k_{**}-a^TA^{-1}a-M\left[(a^TA^{-1}b)^2-2d\,a^TA^{-1}b+d^2\right]\\
&=v_{n-1}(x_*)-M(d-b^TA^{-1}a)^2.
\end{aligned}
$$

Consequently,

$$
\boxed{c_1=\frac1{k(x_n,x_n)+\sigma^2-b^TA^{-1}b},\qquad c_2=b^TA^{-1}a},
$$

and

$$
\boxed{\operatorname{Var}_{n-1}(f_*)-\operatorname{Var}_n(f_*)=c_1\bigl(k(x_n,x_*)-c_2\bigr)^2}.
$$

For interpretation, after the first $n-1$ observations the remaining [covariance](../../../../../covariance.md) between $f_*$ and $f(x_n)$ is $r=d-b^TA^{-1}a$, while the [conditional variance](../../../../../conditional-variance.md) of the new noisy observation is $s$. Thus the reduction is the squared remaining [covariance](../../../../../covariance.md) divided by the remaining observation [variance](../../../../../variance-split.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
