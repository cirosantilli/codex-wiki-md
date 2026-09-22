<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The root calculation for the [Huber location estimator](../../../../../../huber-location-estimator.md) gives

$$
\operatorname{IF}(z;T,\Phi)=\frac{\psi_b(z)}{2\Phi(b)-1}.
$$

Since $|\psi_b(z)|\leq b$ and equality is attained for $|z|\geq b$, its [gross-error sensitivity](../../../../../../gross-error-sensitivity.md) is

$$
\boxed{\sup_z|\operatorname{IF}(z;T,\Phi)|=\frac{b}{2\Phi(b)-1}<\infty.}
$$

Thus it is a [B-robust estimator](../../../../../../b-robust-estimator.md) at the normal reference distribution. At a general centred distribution the same conclusion requires $m=\mathbb E_F\psi_b'(X)>0$, in which case the bound is $b/m$. Boundedness of the score alone does not rescue a zero sensitivity denominator.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
