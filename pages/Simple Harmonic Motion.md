Tags: #Topic

# Simple Harmonic Motion

Simple harmonic motion, also abbreviated as **SHM**, is motion in which a restoring force is directly proportional to the displacement of the object.

Nature's response to a disturbance is often simple harmonic motion.

**Simple Harmonic Oscillator** - An object that is experiencing simple harmonic motion.

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

Additionally since the particle is moving a circular motion, we know there is a centripetal force acting on it.

$$\Large a_\text{c} = \frac{v_\text{tang}^2}{r}$$

Using the arc length formula, we know that

$$\Large r \omega = v_\text{tang}$$

Therefore,

$$
\Large
\begin{aligned}
a_\text{c} &= \frac{r^2 \omega^2}{r} \\
&= r \omega^2 \\
\end{aligned}
$$

In the context of SHM, $r$ is normally the position of an object undergoing SHM. Additionally, a negative is often added to indicate that the acceleration is a restoring force — a force that acts against the direction of movement.

Therefore the formula, also know as the **general form of SHM** is written as

$$\Huge a = -\omega^2 x$$
> **LEGEND:**
> $a$ - Acceleration of the particle pointing in the direction of displacement
> $x$ - Displacement of the particle
> $\omega$ - The angular frequency of the SHM.

This equation is also often rewritten as

$$\Huge a + \omega^2 x = 0$$
$$\Huge \frac{d^2x}{dt^2} + \omega^2 x = 0$$

## Equations of Simple Harmonic Motion

$$
\Huge
\begin{aligned}
x = A\cos(\omega t + \phi) \\
x = A\sin(\omega t + \phi) \\
\end{aligned}
$$

> **LEGEND:**
> $x$ - Position of the object.
> $t$ - Time that has passed.
> $A$ - Amplitude of the SHM.
> $\phi$ - The phase angle, which accommodates for any phase shift in the trigonometric function. In the context of an oscillator, a phase shift means starting an oscillator off at a position that is away from the equilibrium position.
> $\omega$ - The angular frequency of the SHM.

### Maximums

The max velocity and acceleration of an object undergoing SHM can be found by taking the derivative of the SHM position equation.

$$\Large x_\text{max} = A$$

$$\Large v_\text{max} = \omega A$$

$$\Large a_\text{max} = \omega^2 A$$

> **NOTE:**
> Since we apply chain rule when taking a derivative, the constant $\omega$ gets moved out to the outside of the trig function whenever we take a derivative. This is what we get extra $\omega$'s for every derivative we take.
> 
> And since we are dealing with sin/cos trig functions, we know the max value for these functions is 1, therefore the max of each positional equation is just the trig function's coefficient (ie. $A$ for $x(t)$, $\omega A$ for $v(t)$, etc.)

## Period and Frequency
**Angular Frequency** ($\omega$ : Scalar) - The frequency of a SHM object equating it to a particle travelling in circular motion. This is a purely mathematical concept and does not have a "real-world" meaning for the object undergoing SHM.

$$\Huge \omega = \frac{2\pi}{T} = 2\pi f$$

**Period** ($T$ : Scalar) - The time it takes for on oscillation to reach it's original state. For SHM, the period is the time it takes for an object starting at some position to return to that same position.

**Frequency** ($f$ : Scalar) - The number of oscillations per second.

Frequency and period are inversely proportional to each other.

$$\Huge f = \frac{1}{T}$$

## Common Types of SHM

#### [[Spring Mass Oscillators]]
#### [[Pendulums]]

## Energy of SHM

Simple harmonic motion creates a constant cycle of transfering potential energy into kinetic energy and then back into potential energy.

### Potential Energy

Since the [potential energy of a spring](Spring%20Potential%20Energy.md), which is also the potential energy of a SHM, is given by

$$\Large U_\text{s} = \frac{1}{2}kx^2$$

we can plug in the position function of a spring oscillator to get the potential energy with respect to time

$$
\Large
\begin{aligned}
U_\text{s} &= \frac{1}{2}k \left( A\cos ( \omega t + \phi ) \right)^2 \\
&= \frac{1}{2}k A^2 \cos^2 ( \omega t + \phi ) \\
\end{aligned}
$$


### Kinetic Energy

Since the [kinetic energy](Kinetic%20Energy.md) of an object is given by 

$$\Large K = \frac{1}{2}mv^2$$

and since the velocity function of SHM is just

$$\Large v(t) = -A\omega \sin(\omega t + \phi)$$

then,

$$\Large K = \frac{1}{2}mA^2\omega^2 \sin^2(\omega t + \phi)$$

> **NOTE:**
> We ignore the negative sign in the velocity equation since we only care about the magnitude of the velocity when finding kinetic energy.

And since it is given that

$$\Large \omega^2 = \frac{k}{m}$$

we know that

$$
\Large
\begin{aligned}
K &= \frac{1}{2}mA^2 \left( \frac{k}{m} \right) \cos^2(\omega t + \phi) \\
&= \frac{1}{2} k A^2 \cos^2(\omega t + \phi) \\
\end{aligned}
$$

### Total Energy

Since 

$$
\Large
\begin{aligned}
U &= \frac{1}{2}k A^2 \cos^2 ( \omega t + \phi ) \\
K &= \frac{1}{2}k A^2 \sin^2(\omega t + \phi) \\

E &= U + K
\end{aligned}
$$

then the total energy stored by a simple harmonic oscillator is

$$
\begin{aligned}
E &= \frac{1}{2}k A^2 \cos^2 ( \omega t + \phi ) + \frac{1}{2}k A^2 \sin^2(\omega t + \phi) \\
&= \frac{1}{2}k A^2 \left( \cos^2 ( \omega t + \phi ) +  \sin^2(\omega t + \phi) \right) \\
\end{aligned}
$$

Using the trig identity

$$\Large \cos^2 x + sin^2 x = 1$$

we finally find that

$$\Huge E = \frac{1}{2}k A^2$$

> **LEGEND:**
> $E$ - Total energy in the oscillator system.
> $k$ - A constant of proportionality.
> $A$ - The amplitude of the oscillations in meters.