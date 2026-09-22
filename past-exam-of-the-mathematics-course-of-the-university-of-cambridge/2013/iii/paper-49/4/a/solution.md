<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat the printed $e^\mu$ as an [orthonormal coframe](../../../../../../orthonormal-coframe-in-spacetime.md), with frame metric $\eta=\operatorname{diag}(-1,1,1,1)$. Work on a patch $z\ne0$ and $F=1-\alpha z^3>0$, so the given real coframe exists. Define $f=\sqrt F$ and $A=zf'-f$. The [exterior derivatives](../../../../../../exterior-derivative.md) are

$$
de^0=A e^3\wedge e^0,\qquad
de^1=-f e^3\wedge e^1,\qquad
de^2=-f e^3\wedge e^2,\qquad de^3=0.
$$

The [connection 1-forms](../../../../../../connection-1-form-split.md) satisfying [Cartan's first structure equation](../../../../../../cartan-s-first-structure-equation.md) and [metric compatibility](../../../../../../metric-compatibility.md) are

$$
\boxed{\omega^0{}_3=\omega^3{}_0=Ae^0,\qquad
\omega^1{}_3=-fe^1,\quad\omega^3{}_1=fe^1,\qquad
\omega^2{}_3=-fe^2,\quad\omega^3{}_2=fe^2.}
$$

All other forms vanish. With a Lorentzian frame, it is the lowered forms $\omega_{ab}=\eta_{ac}\omega^c{}_b$ that are antisymmetric; the two mixed time–space forms are equal. These displayed forms solve the torsion-free structure equation, and uniqueness of the [Levi-Civita connection](../../../../../../levi-civita-connection.md) identifies them as the required connection.

Apply [Cartan's second structure equation](../../../../../../cartan-s-second-structure-equation.md). For example,

$$
\Theta^0{}_3=d(Ae^0)=-(zfA'+A^2)e^0\wedge e^3,
\qquad
\Theta^0{}_1=\omega^0{}_3\wedge\omega^3{}_1=Af e^0\wedge e^1.
$$

The remaining derivatives give $\Theta^1{}_3=Af e^1\wedge e^3$ and $\Theta^1{}_2=-f^2e^1\wedge e^2$, with analogous forms for index 2. Put $q=\alpha z^3$ and $B=1+q/2$. From $f^2=1-q$,

$$
Af=zf f'-f^2=-B,\qquad zfA'+A^2=F.
$$

Therefore all six independent [curvature 2-forms](../../../../../../curvature-2-form.md) are

$$
\boxed{\begin{aligned}
\Theta^0{}_1&=-B e^0\wedge e^1,&\Theta^0{}_2&=-B e^0\wedge e^2,\\
\Theta^0{}_3&=-F e^0\wedge e^3,&\Theta^1{}_2&=-F e^1\wedge e^2,\\
\Theta^1{}_3&=-B e^1\wedge e^3,&\Theta^2{}_3&=-B e^2\wedge e^3.
\end{aligned}}
$$

The other six are fixed by $\Theta^b{}_a=-\eta_{aa}\eta_{bb}\Theta^a{}_b$ for $a\ne b$, with no sum: equal for time–space pairs and opposite for spatial pairs. All diagonal forms are zero. The [Lorentzian connection-form antisymmetry](../../../../../../lorentzian-connection-form-antisymmetry.md) is essential to these signs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
