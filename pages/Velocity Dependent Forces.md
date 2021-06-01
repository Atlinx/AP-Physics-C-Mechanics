Tags: #Topic #TODO

# Velocity Dependent Forces

## Drag

When an object moves through a fluid, it will experience drag. This fluid could be a gas, like air, or a liquid, like water. The drag force points in the opposite direction of movement and is proportional to the speed, the cross-sectional area, and fluid density.

The derivation for the drag equation is

$$\Large F_\text{drag} = -bv$$

> **LEGEND:**
> $F_\text{drag}$ - Drag force.
> $b$ - Constant that represents the cross-sectional area, the fluid density, the surface of the object, and all the other factors that influence drag which are not already present in the equation.
> $v$ - Velocity of the object.
> $-$ - Negative sign indicates that the force points in the opposite direction to the velocity.

> **NOTE:**
> This is an extreme simplification of drag, since it consolidates a lot of terms into $b$. But this is all you are expected to know for the AP exam.

### Air Resistance

For air resistance, drag is often written as

$$
\Large
\begin{aligned}
F_\text{net} &= ma \\
&= m\frac{dv}{dt} \\
&= F_\text{g} - F_\text{drag} \\
&= mg - bv \\
\end{aligned}
$$

Therefore,

$$\Large m\frac{dv}{dt} = mg - bv$$

> **NOTE:**
> $m \dfrac{dv}{dt}$ must always be the opposite sign of the drag force. This seems to be just a common convention used. (Technically it does not matter where the signs are since a negative would just show up when evaluating for $\dfrac{dv}{dt}$, but College Board seems to prefer this convention).  

Additionally, this equation is often solved to be a transient equation for velocity. This solution is,

$$
\Large 
\begin{aligned}
m\frac{dv}{dt} &= mg - bv \\
\frac{dv}{dt} &= g - \frac{b}{m}v \\
\end{aligned}
$$

$$\Large 
\frac{dv}{g - \frac{b}{m}v} = dt $$

$$\Large \frac{dv}{- \frac{b}{m}v + g} = dt $$

$$\Large  \left( \frac{1}{-\frac{m}{b}} \right) \frac{dv}{- \frac{b}{m}v + g} = dt \left( \frac{1}{-\frac{m}{b}} \right)$$

$$\Large \frac{dv}{v - \frac{mg}{b}} = - \frac{b}{m} dt$$

$$\Large \int_0^v \frac{dv}{v - \frac{mg}{b}} = \int_0^t - \frac{b}{m} dt$$

$$\Large \left. ln \left| v - \frac{mg}{b} \right| \right|_0^v = \left. \left( - \frac{b}{m}t \right) \right|_0^t$$

Since we are evaluating from $0$ to $v$ and from $0$ to $t$, we can remove the absolute value.

$$\Large \left. ln \left( v - \frac{mg}{b} \right) \right|_0^v = \left. \left(- \frac{b}{m}t \right) \right|_0^t$$

$$ln \left( v - \frac{mg}{b} \right) - ln \left( - \frac{mg}{b} \right) = - \frac{b}{m}t - 0$$

$$\Large ln \left(\frac{v - \frac{mg}{b}}{- \frac{mg}{b}} \right) = - \frac{b}{m}t $$

$$\Large \frac{v - \frac{mg}{b}}{- \frac{mg}{b}} = e^{- \frac{b}{m}t} $$

$$\Large v - \frac{mg}{b} = - \frac{mg}{b} e^{- \frac{b}{m}t} $$

$$\Large v = - \frac{mg}{b} e^{- \frac{b}{m}t} + \frac{mg}{b}$$

$$\Large v = \frac{mg}{b} \left( - e^{- \frac{b}{m}t} + 1 \right)$$

Therefore our equation is

$$\huge v = \frac{mg}{b} \left(1 - e^{- \frac{b}{m}t} \right)$$

We can see that as $t \to \infty$, the velocity appraoches $\dfrac{mg}{b}$.

This means the terminal velocity, the maximum speed of an object, is

$$\Huge v_\text{max} = \dfrac{mg}{b}$$