<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Work on the [Riemann sphere](../../../../../riemann-sphere.md), including zero and infinity. For $j(z)=1/z$, two iterations give the identity and one does not, so $\operatorname{ord}(j)=2$. For $k(z)=1/(1-z)$, direct composition gives

$$
k^2(z)=\frac{z-1}{z},\qquad k^3(z)=z.
$$

Neither $k$ nor $k^2$ is the identity; in particular $0\mapsto1\mapsto\infty\mapsto0$. Thus

$$
\boxed{\operatorname{ord}(z\mapsto1/z)=2,\qquad\operatorname{ord}(z\mapsto1/(1-z))=3.}
$$

To prove the [Möbius conjugacy normal forms](../../../../../mobius-conjugacy-normal-forms.md), write a [Möbius transformation](../../../../../mobius-transformation.md) as $f(z)=(az+b)/(cz+d)$ with $ad-bc\ne0$. A finite fixed point satisfies $cz^2+(d-a)z-b=0$. If $c\ne0$, this quadratic has two roots counting multiplicity, and infinity is not fixed. If $c=0$, the transformation is affine, infinity is fixed, and there is one further finite fixed point unless its slope is one. A nonidentity slope-one affine map is a nonzero translation with only infinity fixed. Thus any nonidentity [Möbius transformation](../../../../../mobius-transformation.md) has one or two distinct fixed points.

If there are two, say $p,q$, choose a [Möbius transformation](../../../../../mobius-transformation.md) $h$ taking them to zero and infinity. For finite $p,q$ one can use $h(z)=(z-p)/(z-q)$; the cases involving infinity use an affine map or reciprocal. The conjugate $hfh^{-1}$ fixes zero and infinity. Fixing infinity sets its denominator's linear coefficient to zero, and fixing zero sets its numerator's constant term to zero; hence it is $z\mapsto\mu z$ with $\mu\ne0$.

If there is only one fixed point, send it to infinity. The conjugate has the affine form $az+b$. If $a\ne1$, $b/(1-a)$ would be another fixed point, which is impossible; therefore $a=1,b\ne0$. Conjugating this translation by $z\mapsto z/b$ yields $z\mapsto z+1$. The identity is already the scaling $\mu=1$. This proves the classification, and invertibility excludes $\mu=0$.

Conjugation carries fixed-point sets bijectively. The translation $z+1$ has exactly one fixed point, infinity. A nonidentity scaling has the two fixed points zero and infinity, while the identity fixes every point. Therefore **$z+1$ is not conjugate to any scaling**.

Finally let $f$ have finite positive order $n$. A nonzero translation has infinite order, since its $k$th iterate is $z+k$ after normalization. Thus $f$ is conjugate to $z\mapsto\mu z$, where $\mu$ has multiplicative order exactly $n$. For $n>1$, zero and infinity each form a singleton orbit. At a finite nonzero $z$, an iterate returns precisely when $\mu^kz=z$, equivalently $\mu^k=1$; the least positive return time is $n$. Conjugacy preserves orbit sizes. Hence the [finite-order Möbius orbit sizes](../../../../../finite-order-mobius-orbit-sizes.md) are

$$
\boxed{1\text{ and }n\quad(n>1),\qquad\text{only }1\quad(n=1).}
$$

For $n>1$ exactly two points have size-one orbits; every other point has orbit size $n$.

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
