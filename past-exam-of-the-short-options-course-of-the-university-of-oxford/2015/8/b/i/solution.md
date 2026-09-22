<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Now use $(ct,x)^T$ and $\eta_2=\operatorname{diag}(1,-1)$. Write

$$
L=\begin{pmatrix}a&b\\d&e\end{pmatrix}.
$$

Preservation of the [Minkowski metric](../../../../../minkowski-metric.md) says that the first column has squared norm $1$, the second has squared norm $-1$, and the columns are orthogonal for the [Minkowski inner product](../../../../../minkowski-inner-product.md):

$$
a^2-d^2=1,\qquad b^2-e^2=-1,\qquad ab-de=0.
$$

Orthochronousness gives $a\ge1$. From the orthogonality equation, $b=de/a$; substituting in the second norm identity gives $e^2=a^2$. Hence $(b,e)=\varepsilon(d,a)$ with $\varepsilon=\pm1$. The [determinant](../../../../../determinant.md) is then $\varepsilon(a^2-d^2)=\varepsilon$, so properness forces $\varepsilon=1$. Thus $b=d$ and $e=a$.

Set $\beta=d/a$. The first norm identity implies $|\beta|<1$ and $a=(1-\beta^2)^{-1/2}$. With $u=c\beta$, this gives

$$
\boxed{L=\begin{pmatrix}\gamma&\gamma u/c\\\gamma u/c&\gamma\end{pmatrix},
\qquad\gamma=(1-u^2/c^2)^{-1/2},\quad |u|<c.}
$$

Conversely, the displayed [matrix](../../../../../matrix.md) has $\gamma^2-(\gamma u/c)^2=1$, equal off-diagonal entries, [determinant](../../../../../determinant.md) one, and positive time-time entry. Direct multiplication therefore gives $L^T\eta_2L=\eta_2$, proving both directions. The plus signs are the [Lorentz boost](../../../../../lorentz-boost.md) convention used in the paper; reversing the boost direction replaces $u$ by $-u$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
