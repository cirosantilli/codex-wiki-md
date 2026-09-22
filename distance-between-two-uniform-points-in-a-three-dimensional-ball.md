# Distance between two uniform points in a three-dimensional ball

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution-split.md)

For two [independent random variables](independent-random-variables.md) taking values in a three-dimensional [ball](ball-mathematics.md) with constant volume [probability density](probability-density.md), the density of their distance is the displayed expression for $0\leq r\leq2R$, and zero otherwise. Both [independence](independent-random-variables.md) and the common radius $R>0$ are essential. To derive it, put $u=|\mathbf r_1|$, $v=|\mathbf r_2|$ and integrate the product volume [differential form](differential-form-split.md) over orientations. The [law of cosines](law-of-cosines.md) gives the angular [Jacobian determinant](jacobian-determinant.md) $v/(ur)$, leaving $f_R(r)=9r\int uv\,du\,dv/(2R^6)$ over $0\leq u,v\leq R$, $|u-v|\leq r\leq u+v$. With $x=u+v$, $y=u-v$, the integrand becomes $(x^2-y^2)\,dx\,dy/8$. Direct integration gives $\int uv\,du\,dv=2R^3r/3-R^2r^2/2+r^4/24$. An independent geometric derivation uses the overlap volume of two radius-$R$ balls displaced by $r$, namely $\pi(4R+r)(2R-r)^2/12$, multiplied by $4\pi r^2$ and divided by the square of $4\pi R^3/3$. The density integrates to one and has mean $36R/35$.

## ↑ Ancestors (7)

1. [Continuous probability distribution](continuous-probability-distribution-split.md)
2. [Probability distribution](probability-distribution.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-71/1/solution.md)
