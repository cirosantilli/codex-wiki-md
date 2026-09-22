# Rotational kinetic energy

↑ **Parent:** [Kinetic energy](kinetic-energy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rotational_kinetic_energy)

[Rotational kinetic energy](rotational-kinetic-energy.md) is the [kinetic energy](kinetic-energy.md) of a [rigid body](rigid-body-dynamics.md)'s rotation. For pure rotation about an axis fixed in an [inertial frame](inertial-frame.md),

$$
K_{\mathrm{rot}}=\frac12I\omega^2,
\qquad I=\int r_\perp^2\,dm,
\qquad \omega=|\boldsymbol\omega|.
$$

Here $r_\perp$ is the perpendicular distance of a [mass](mass.md) element $dm$ from that axis, $I$ is the [moment of inertia](moment-of-inertia.md) about that same axis, and $\omega$ is the common [angular speed](angular-speed.md), measured in [radians](radian.md) per second. The [rigid body](rigid-body-dynamics.md) assumption fixes the relative positions of the [mass](mass.md) elements; they share [angular velocity](angular-velocity.md) but have different [speeds](speed.md) $v=\omega r_\perp$. Summing their [kinetic energies](kinetic-energy.md) $dm\,v^2/2$ gives the formula. This is a nonrelativistic model; deformation or internal motion can contribute additional [kinetic energy](kinetic-energy.md).[§10.4](university-physics-volume-1-by-william-moebs-and-others/10-4-moment-of-inertia-and-rotational-kinetic-energy.md)

For a computed example, take a uniform disc and an ideal thin ring, each of [mass](mass.md) $M=2\,\mathrm{kg}$ and radius $R=0.30\,\mathrm m$, rotating about its central perpendicular axis at [angular speed](angular-speed.md) $10\,\mathrm{rad/s}$. The [moment of inertia of a uniform disc](moment-of-inertia-of-a-uniform-disc.md) is $MR^2/2=0.090\,\mathrm{kg\,m^2}$, while the ring has [moment of inertia](moment-of-inertia.md) $MR^2=0.180\,\mathrm{kg\,m^2}$. Their [rotational kinetic energies](rotational-kinetic-energy.md) are therefore $4.5\,\mathrm J$ and $9.0\,\mathrm J$. The ring stores twice the [energy](energy.md) at the same [angular speed](angular-speed.md), because more [mass](mass.md) lies farther from the axis. At the same nonzero [rotational kinetic energy](rotational-kinetic-energy.md), its [angular speed](angular-speed.md) would instead be $1/\sqrt{2}$ times the disc's. This makes radial placement useful for storing [energy](energy.md) in a rotating wheel, although a real design must also withstand the stresses of rotation.

For fixed-axis rotation with constant [moment of inertia](moment-of-inertia.md), write the signed rotation rate as $\Omega=\dot\theta$, with [angle](angle.md) $\theta$ in [radians](radian.md). The axial component of net external [torque](torque.md) obeys $\tau_{\mathrm{axis}}=I\dot\Omega$, so the [work-energy theorem](work-energy-theorem.md) becomes

$$
\frac{dK_{\mathrm{rot}}}{dt}=\tau_{\mathrm{axis}}\Omega,
\qquad \Delta K_{\mathrm{rot}}=\int\tau_{\mathrm{axis}}\,d\theta.
$$

An opposing [torque](torque.md) removes [rotational kinetic energy](rotational-kinetic-energy.md); bearing [friction](friction.md) must be included in the net [torque](torque.md). The signed $\Omega$ matters when the direction reverses. Rotation about a fixed axis need not be about a [principal axis](principal-axis.md): the scalar [energy](energy.md) formula still holds, but transverse bearing [torques](torque.md) can be needed to maintain that axis.

For general [rigid body](rigid-body-dynamics.md) motion, use the [inertia tensor](inertia-tensor.md) $\mathsf I_G$ about the [centre of mass](center-of-mass.md) $G$:

$$
K_{\mathrm{total}}=\frac12M|\mathbf V_G|^2+\frac12\boldsymbol\omega^{\mathsf T}\mathsf I_G\boldsymbol\omega,
\qquad \mathbf L_G=\mathsf I_G\boldsymbol\omega.
$$

This is the [kinetic-energy decomposition about the centre of mass](kinetic-energy-decomposition-about-the-centre-of-mass.md). In a [principal body frame](principal-body-frame.md), the rotational term is $\tfrac12(I_1\omega_1^2+I_2\omega_2^2+I_3\omega_3^2)$, using the [principal moments of inertia](principal-moment-of-inertia.md). Away from a [principal axis](principal-axis.md), [angular momentum](angular-momentum.md) and [angular velocity](angular-velocity.md) need not be parallel. A freely rotating asymmetric [rigid body](rigid-body-dynamics.md) can change the direction of [angular velocity](angular-velocity.md) relative to the body even while [rotational kinetic energy](rotational-kinetic-energy.md) remains constant; [Euler equations for a torque-free rigid body](euler-equations-for-a-torque-free-rigid-body.md) govern that motion. One constant axial [moment of inertia](moment-of-inertia.md) is then insufficient.[Chapter 20: Rotation in space](the-feynman-lectures-on-physics-volume-i-by-richard-feynman-and-others/chapter-20-rotation-in-space.md)

## ↑ Ancestors (6)

1. [Kinetic energy](kinetic-energy.md)
2. [Energy](energy.md)
3. [Classical mechanics](classical-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Classical mechanics](classical-mechanics-split.md)
- [Equipartition theorem](equipartition-theorem.md)
- [Ideal gas](ideal-gas.md)
- [Inertia tensor](inertia-tensor.md)
- [Inertia tensor of paired point masses](inertia-tensor-of-paired-point-masses.md)
- [Kinetic-energy decomposition about the centre of mass](kinetic-energy-decomposition-about-the-centre-of-mass.md)
- [Molecular rotation](molecular-rotation.md)
- [Moment of inertia](moment-of-inertia.md)
- [Parallel axis theorem](parallel-axis-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-42/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/9b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/12c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-4/3a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-306/1/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/8e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-4/11c/b/ii/solution.md)
- [Principal moment of inertia](principal-moment-of-inertia.md)
- [Rigid rotor](rigid-rotor.md)
- [Rotational energy ellipsoid](rotational-energy-ellipsoid.md)
- [Rotational kinetic energy](rotational-kinetic-energy.md)
