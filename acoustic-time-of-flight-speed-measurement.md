# Acoustic time-of-flight speed measurement

↑ **Parent:** [Wave speed](wave-speed.md)

The experiment in [A time of flight method to measure the speed of sound using a stereo sound card by Carlos C. Carvalho and others](a-time-of-flight-method-to-measure-the-speed-of-sound-using-a-stereo-sound-card-by-carlos-c-carvalho-and-others.md) makes [wave speed](wave-speed.md) visible as a delay. Two powered [microphones](microphone.md) feed separate channels of one stereo line input. A clap beyond one end of their common axis reaches the nearer [microphone](microphone.md) first. The displayed [signals](signal.md) show two separated onsets when enlarged; count their sample separation $N$ to obtain $\Delta t=N/f_s$ and infer [speed of sound](speed-of-sound.md) $c=d/\Delta t$ from the measured [microphone](microphone.md) spacing $d$. The reported [sampling rate](sampling-rate.md) is $44100\,\mathrm{s^{-1}}$. Repeating at different spacings gives a distance-versus-delay plot whose slope estimates [speed of sound](speed-of-sound.md); dependence on distance helps identify acoustic travel rather than a fixed electronic delay. These are the paper's apparatus and observed readout, not measurements made for this article.[A time of flight method to measure the speed of sound using a stereo sound card by Carlos C. Carvalho and others](a-time-of-flight-method-to-measure-the-speed-of-sound-using-a-stereo-sound-card-by-carlos-c-carvalho-and-others.md)

A controlled implementation also needs [timing calibration for acoustic speed measurements](timing-calibration-for-acoustic-speed-measurements.md). Put the [microphones](microphone.md) side by side to estimate the channel-delay offset $\tau_0$, swap channels to check its sign, and check the acquisition clock against an independent timing reference. Measure spacings between consistent points on the [microphones](microphone.md), keep the source outside their span and on their axis, and fit $\Delta t=d/c+\tau_0$ by [linear regression](linear-regression-split.md) rather than forcing a zero intercept. Repeat pulses and compare the same onset criterion before reflections arrive. These are proposed calibration and control checks, not additional procedures claimed for the paper.

One sample corresponds to $1/f_s\simeq22.7\,\mathrm{\mu s}$ for the reported [sampling rate](sampling-rate.md), so a delay of only a few samples has large relative [measurement error](measurement-error.md). Background [measurement noise](measurement-noise.md), different [microphone](microphone.md) responses and threshold choice can move the apparent onset; reflections can supply a later competing pulse. Record [temperature](temperature.md), keep air motion small, and compare several spacings. The result estimates [speed of sound](speed-of-sound.md) under those conditions; it cannot prove an exactly zero precursor below the instrument's sensitivity or establish [finite propagation speed](finite-propagation-speed.md) for every real medium. Both new diagrams in these sections show explicitly synthetic ideal [wave equation](wave-equation-split.md) solutions.[A time of flight method to measure the speed of sound using a stereo sound card by Carlos C. Carvalho and others](a-time-of-flight-method-to-measure-the-speed-of-sound-using-a-stereo-sound-card-by-carlos-c-carvalho-and-others.md)

**Table of contents**

- [Timing calibration for acoustic speed measurements](timing-calibration-for-acoustic-speed-measurements.md)
- [Microphone](microphone.md)
- [Sampling rate](sampling-rate.md)

## ↑ Ancestors (7)

1. [Wave speed](wave-speed.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Microphone](microphone.md)
