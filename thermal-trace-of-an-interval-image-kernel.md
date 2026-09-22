# Thermal trace of an interval image kernel

↑ **Parent:** [Dirichlet heat kernel on an interval](dirichlet-heat-kernel-on-an-interval.md)

For a particle with mass $m$ on $(0,L)$, put $K_0(x;\beta)=\sqrt{m/(2\pi\hbar^2\beta)}e^{-mx^2/(2\hbar^2\beta)}$. The [method of images](method-of-images.md) gives $K_D(q_f,q_i;\beta)=\sum_r[K_0(q_f-q_i+2rL;\beta)-K_0(q_f+q_i+2rL;\beta)]$. The diagonal integral is

$$
Z=L\sqrt{\frac m{2\pi\hbar^2\beta}}\sum_{r\in\mathbb Z}e^{-2mL^2r^2/(\hbar^2\beta)}-\frac12.
$$

The reflected intervals tile the real line, giving the subtraction $1/2$. The [Poisson summation formula](poisson-summation-formula.md) converts this to $\sum_{n\ge1}e^{-\beta\hbar^2\pi^2n^2/(2mL^2)}$, proving equality between the image and [energy eigenstate](energy-eigenstate.md) calculations.

## ↑ Ancestors (9)

1. [Dirichlet heat kernel on an interval](dirichlet-heat-kernel-on-an-interval.md)
2. [Heat kernel](heat-kernel.md)
3. [Heat equation](heat-equation.md)
4. [Diffusion equation](diffusion-equation-split.md)
5. [Partial differential equation](partial-differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-81/3/c/solution.md)
