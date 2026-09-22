<h1 id="7/h/solution">Solution</h1>

↑ **Parent:** [H](../h.md)

A spatially uniform source changes only the [zero Fourier mode](../../../../../zero-fourier-mode.md). Its exact integrated increment over a time step beginning at $t$ is

$$
\Delta q=\int_t^{t+\Delta t}0.1e^{-s/10}\,ds
=e^{-t/10}-e^{-(t+\Delta t)/10}.
$$

The unnormalised two-dimensional [discrete Fourier transform](../../../../../discrete-fourier-transform-split.md) stores a constant field $q$ as $n_xn_yq$ in element `(1,1)`.[The forward defining sum has no normalization; the linked inverse definition includes the factor $1/(n_xn_y)$.](../../../../../fft2-documentation-by-mathworks.md) Keep the existing homogeneous exponential multiplication and add this source increment to that element:
```
for i = 1:nt
    t = (i-1)*dt;
    u_hat = u_hat .* exp(-alpha*K2*dt);
    dq = exp(-t/10) - exp(-(t+dt)/10);
    u_hat(1,1) = u_hat(1,1) + nx*ny*dq;
end
```
This replacement uses the original variable names and [MATLAB](../../../../../matlab.md) indexing. The [uniform forcing of a periodic heat equation](../../../../../uniform-forcing-of-a-periodic-heat-equation.md) is integrated exactly in time here. No source multiplier is applied to the other modes, and the zero-mode homogeneous multiplier equals one. Adding only `dq` to the unnormalised coefficient would underestimate the physical temperature increment by the factor $n_xn_y$.

## ↑ Ancestors (12)

1. [H](../h.md)
2. [7](../../7.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2025](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
