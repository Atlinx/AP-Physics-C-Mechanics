Tags: #Topic

# Simple Harmonic Motion

Simple harmonic motion, also abbreviated as **SHM**, is motion in which a restoring force is directly proportional to the displacement of the object.

Nature's response to a disturbance is often simple harmonic motion.

## Derivation

Simple harmonic motion is derived from the motion of moving around a circle. Imagine having a particle starting at one end of the circle and then moving around the entire circle. The velocity of the movement is $\omega$

The $x$ position of the particle would be

$$\Large x = A\cos(\theta)$$

where $A$ is the radius of the circle and $\theta$ is the total angle the particle has travelled.

Since by definition of velocity, we know that 

$$\Large \omega = \dfrac{\theta}{t}$$

We can rearrange it to form

$$\Large \theta = \omega t$$

which we can then plug into the $cos()$ equation to form the basic formula of simple harmonic motion.

$$\Large x = A\cos(\omega t)$$

> **NOTE:**
> The $y = Asin(\theta t)$ comes from using  the $y$ position of the imaginary particle moving around a circle.

Additionally particle follow simple harmonic motion if

$$\Large a = -\omega^2 x$$
> **LEGEND:**
> $a$ - Acceleration of the particle pointing in the direction of displacement
> $x$ - Displacement of the particle
> $\omega$ - A constant of proportionality

## Forms of Simple Harmonic Motion

$$
\Huge
\begin{aligned}
x = A\cos(\omega t + \phi) \\
x = A\sin(\omega t + \phi) \\
\end{aligned}
$$

> **NOTE:**
> $\phi$ just accommodates for any phase shift in the trigonometric function. In the context of an oscillator, a phase shift means starting an oscillator off at a position that is away from the equilibrium position.

## Period and Frequency

**Period** ($T$ : Scalar) - The time it takes for on oscillation to reach it's original state. For SHM, the period is the time it takes for an object starting at some position to return to that same position.

$$\Huge T = \frac{2 \pi}{\omega}$$

> **NOTE:**
> This comes from the equation of distance ($d$), rate ($r$), and time ($t$).
> 
> $$
\Large
\begin{aligned}
tr &= d \\
t &= \frac{d}{r} \\\\
d &= 2\pi \\
r &= \omega \\
t &= T \\\\
T &= \frac{2 \pi}{\omega}\\
\end{aligned}
> $$

**Frequency** ($f$ : Scalar) - The number of oscillations per second.

Frequency and period are inversely proportional to each other.

$$\Huge f = \frac{1}{T}$$

## [[Spring Mass Oscillators]]
## [[Pendulums]]