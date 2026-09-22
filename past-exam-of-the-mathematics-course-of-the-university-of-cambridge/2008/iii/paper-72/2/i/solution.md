<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The stated kinematics do not, by themselves, fix a [galaxy](../../../../../../galaxy-split.md)'s intrinsic axis ratio. The requested curve is the usual simplified [oblate-rotator flattening proxy](../../../../../../oblate-rotator-flattening-proxy.md); its additional geometric and streaming conventions should be explicit. Put $q=b/a=1-e$ and adopt the approximate moment prescription

$$
q\simeq\frac{\sigma_z^2}{\sigma_x^2+v_p^2}.
$$

Here $v_p^2$ is the ordered support assigned to one in-plane component. Using $\sigma_z^2=(1-\beta)\sigma_x^2$ and solving gives

$$
\boxed{\frac{v_p}{\sigma_x}\simeq\sqrt{\frac{e-\beta}{1-e}}.}
$$

In this prescription, isotropic random motions give the [oblate isotropic rotator](../../../../../../oblate-isotropic-rotator.md) curve; positive $\beta$ allows flattening with less rotation. A real solution requires $0\le e<1$, $\beta<1$, and $e\ge\beta$. Equality $e=\beta$ gives no rotation. This is a useful diagnostic approximation, not an exact identity for arbitrary density distributions.

To see what the [tensor virial theorem](../../../../../../tensor-virial-theorem.md) actually requires, take a finite stationary axisymmetric system with mass-weighted constant [velocity dispersions](../../../../../../velocity-dispersion.md) and azimuthal streaming speed $v_{\rm az}$. Since $u_x=-v_{\rm az}\sin\phi$, the azimuthal average has $\langle u_x^2\rangle=v_{\rm az}^2/2$. The $xx$ and $zz$ components give

$$
-W_{xx}=M(\sigma_x^2+v_{\rm az}^2/2),\qquad -W_{zz}=M\sigma_z^2,
$$

and therefore, with the [oblate tensor-virial shape factor](../../../../../../oblate-tensor-virial-shape-factor.md) $Q=W_{xx}/W_{zz}$,

$$
\boxed{\frac{v_{\rm az}^2}{\sigma_x^2}=2\big[(1-\beta)Q-1\big].}
$$

For similar oblate self-gravitating density surfaces, write $s=\sqrt{1-q^2}$. The ellipsoidal force coefficients, obtained by integrating the Newtonian force over those surfaces, are

$$
A_1=\frac{q\arccos q}{s^3}-\frac{q^2}{s^2},\quad A_3=\frac2{s^2}-\frac{2q\arccos q}{s^3},\quad Q=\frac{A_1}{q^2A_3}.
$$

The common radial integral in the [stellar potential-energy tensor](../../../../../../stellar-potential-energy-tensor.md) cancels, but these shape coefficients remain. At $q=1/2$, $Q\simeq1.79$, rather than $1/q=2$. With $\beta=0$, the intrinsic azimuthal ratio is about $1.26$, whereas the printed simplified ratio is $1$. Recovering the latter uses both $v_p=v_{\rm az}/\sqrt2$ and $Q\simeq1/q$. Thus, if the printed $v$ literally means intrinsic azimuthal speed, its claimed exact relation omits necessary model assumptions and a streaming normalization. The next sketch displays the requested approximate curve with that qualification.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
