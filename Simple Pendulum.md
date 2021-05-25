Tags: #Topic 

# Simple Pendulum

![](../attachments/simple_pendulum.png)

$$\Large \omega = \sqrt{\frac{g}{L}}$$

$$\Large T = 2 \pi \sqrt{\frac{L}{g}}$$

### Derivation via Force

According to [[Simple Harmonic Motion]], we must prove that

$$\Large a = \omega^2x$$

Since the acceleration, $a$, of the SHM particle must be in the direction of displacement, $a$ for the pendulum is equal to the tangential acceleration $a_\text{}$ of the mass, since this points in the direction of the displacement of the mass. And for the sake of clarity, we will use $s$ instead of $x$ for displacement. Therefore,

$$\Large a_\text{tang} = \omega^2s$$

Using some geometry, we know that 

$$
\Large 
\begin{aligned}
F_\text{tang} = F_g \sin\theta &= ma_\text{tang} \\
 mg \sin\theta &= ma_\text{tang} \\
 g \sin\theta &= a_\text{tang} \\
\end{aligned}
$$

Plugging back into the SHM equation,

$$\Large g \sin\theta = \omega^2x$$

Since $\theta \approx \sin\theta$ for small angles of $\theta$, then

$$\Large g \theta = \omega^2x$$

Since the displacement is an arc length,

$$
\Large
\begin{aligned}
\theta L &= s \\
\theta &= \frac{s}{L} \\
\end{aligned}
$$

Therefore,

$$
\Large
\begin{aligned}
g \left( \frac{s}{L} \right) &= \omega^2s \\
\frac{g}{L} &= \omega^2 \\
\omega &= \sqrt{\frac{g}{L}}\\
\end{aligned}
$$

This means,

$$
\Large
\begin{aligned}
T = 2\pi \sqrt{\frac{L}{g}}
\end{aligned}
$$

## Derivation via Torque

$$\Large \tau_p = (-\vec F_g \times \vec L) = I_p \alpha$$

> **NOTE:**
> This equation is negative since the force of gravity is a restoring forc

$$\Large -mgL\cos(90^\circ - \theta) = I_p \alpha$$

Rewriting angular acceleration as,

$$\Large \alpha = \frac{d^2 \theta}{dt^2}$$

$$
\Large
\begin{aligned}
-mgL\cos(90^\circ - \theta) &= I_p \cdot \frac{d^2 \theta}{dt^2} \\
-mgL\sin(\theta) &= I_p \cdot \frac{d^2x}{dt^2} \\
\end{aligned}
$$

For small angles of $\theta$, $\theta \approx \sin\theta$. Therefore,

$$
\Large 
\begin{aligned}
-mgL\theta &= I_p \cdot \frac{d^2 \theta}{dt^2} \\
-\left(\frac{mgL}{I_p}\right)\theta &= \frac{d^2 \theta}{dt^2} \\
\end{aligned}
$$

$$\Large \frac{d^2 \theta}{dt^2} + \left( \frac{mgL}{I_p} \right)\theta = 0$$

Since this equation followings the derived [[Simple Harmonic Motion]] equation of

$$\Large \frac{d^2x}{dt^2} + \omega^2 x = 0$$

we know that

$$\Large \omega = \sqrt{\frac{mgL}{I_p}}$$

And since for a point mass,

$$I_\text{point} = L^2m$$

we know that

$$
\Large
\begin{aligned}
\omega &= \sqrt{\frac{mgL}{L^2m}} \\
&= \sqrt{\frac{g}{L}} \\
\end{aligned}
$$

Therefore the period is

$$\Large T = 2 \pi \sqrt{\frac{L}{g}}$$