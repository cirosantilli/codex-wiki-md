<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

No slip and impermeability give dimensional $u=-U$, $w=0$ on the upward-moving wall, so $\boxed{\widehat u=-1,\ \widehat w=0}$ there. For the interface normal, $h_x=\delta\widehat h_{\widehat x}$, and hence

$$
\mathbf n=(\delta\widehat h_{\widehat x},-1)+O(\delta^2)
$$

in its $x,z$ components. The relevant stresses scale as

$$
\sigma_{xx}=-\Pi\widehat p+O(\mu U/L),\qquad
\sigma_{xz}=\frac{\mu U}{\delta L}\widehat u_{\widehat z}+O(\delta\mu U/L),
\qquad\sigma_{zz}=-\Pi\widehat p+O(\mu U/L).
$$

Multiplying by the inward normal gives the leading [traction](../../../../../traction.md)

$$
\boxed{\mathbf t\sim-\frac{\mu U}{\delta L}
(\widehat p\widehat h_{\widehat x}+\widehat u_{\widehat z})\mathbf i
+\frac{\mu U}{\delta^2L}\widehat p\mathbf k.}
$$

Its leading normal component vanishes only if $\widehat p=0$ at the interface; the tangential component then requires $\widehat u_{\widehat z}=0$.

The [free surface](../../../../../free-surface.md) is material. Applying the [material derivative](../../../../../material-derivative.md) to $z-h(x,t)=0$ gives $w=h_t+uh_x$, which in the scaled variables becomes

$$
\boxed{\widehat w=\widehat h_{\widehat t}+\widehat u\widehat h_{\widehat x},\qquad
\widehat p=0,\qquad\widehat u_{\widehat z}=0
\quad\text{at }\widehat z=\widehat h.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
