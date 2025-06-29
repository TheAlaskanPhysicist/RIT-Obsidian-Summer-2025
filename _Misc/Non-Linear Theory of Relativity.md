

### Conventions
$$\begin{align}
x^\mu(\tau)&=\dfrac{du^\mu}{d\tau} && \text{(4-Position)}\\
u^\mu(\tau)&=\dfrac{dx^\mu}{d\tau} && \text{(4-Velocity)}\\
a^\mu(\tau)&=\dfrac{du^\mu}{d\tau} && \text{(4-Acceleration)}\\
g_{\mu\nu}&=\eta_{\mu\nu} && \text{(Minkowski Metric)}
\end{align}$$
### The Lorentz Boost Transform ($a=0$)
For inertial frames, velocity transforms by a linear Lorentz boost.
$$\begin{align}
u'^\mu&=\mathcal{V}^\mu_\nu u^\nu
\end{align}$$
where $\mathcal{V}^\mu_\nu=\Lambda^\mu_\nu$ that also respects the metric $g_{\mu\nu}$:
$$\begin{align}
g_{\alpha\beta}&=\mathcal{V}^\mu_\alpha g_{\mu\nu}\mathcal{V}^\nu_\beta
\end{align}$$
### Non-Linear Correction Transform
We want to generalize the transform into the following form:
$$\begin{align}
x'^\mu&=x^\mu+\mathcal{V}^\mu_\nu v^\nu+\mathcal{A}^\mu_{\nu\rho} a^\nu a^\rho
\end{align}$$
This gives us our typical linear Lorentz boost, but also a quadratic acceleration.

### Coordinate Transform under uniform acceleration
Similar to Rindler coordinates, we can generalize to 3+1 spacetime as:
$$\begin{align}
x'^\mu&=x^\mu+\gamma(v)v^\mu+\dfrac{1}{2}a^\mu\tau^2
\end{align}$$



$$\begin{align}
\mathcal{A}^\mu_{\nu\rho}&=\alpha(\tau)g^{\mu\lambda}\left(\delta_\nu^\lambda\delta_\rho^\sigma+\delta_\rho^\lambda\delta_\nu^\sigma\right)u_\sigma\\
\Aboxed{\mathcal{A}^\mu_{\nu\rho}&=\alpha(\tau)g_{\nu\rho}u^\mu }
\end{align}$$
$$\begin{align}
x'^\mu&=x^\mu+\mathcal{V}^\mu_\nu v^\nu+\alpha(\tau)u^\mu a_\nu a^\nu
\end{align}$$


























### Founding Idea
We want to explore a mathematical structure that allows for frame transforms between all frames, not just inertial, but still recover inertial structure when higher order motion is suppressed.

We can write a general transform as the following:

Where $\mathcal{V}$ is our typical Lorentz boost. Each tensor corrects for higher order motion, and respects the metric and light-cones.



### Case: Linear Velocity
Required mechanics ($x$ is the lab frame, $x'$ is the particle frame):
$$\begin{align}
a^\mu&=\dfrac{du^\mu}{d\tau}=0
\end{align}$$
We recover the Lorentz boost for Inertial Frames of Reference.
$$\begin{align}
x'^\mu&=\mathcal{V}^\mu_\nu x^\nu+\mathcal{A}^\mu_{\nu\rho} x^\nu x^\rho+\mathcal{J}^\mu_{\nu\rho\sigma} x^\nu x^\rho x^\sigma
\end{align}$$


### Case: Linear Acceleration
Required mechanics ($x$ is the lab frame, $x'$ is the particle frame):
$$\begin{align}
a^\mu&=\dfrac{du^\mu}{d\tau} & j^\mu&=\dfrac{da^\mu}{d\tau}=0
\end{align}$$
We can then write the general equation as:
$$\begin{align}
x'^\mu&=\mathcal{V}^\mu_\nu x^\nu+\mathcal{A}^\mu_{\nu\rho} x^\nu x^\rho
\end{align}$$
#### Rindler coordinates
A good theory worth its salt should replicate mechanics we've already observed.
Defining $a=a_x$, we should recover the following coordinates:
$$\begin{align}
x'^\mu(\tau)&=
\end{align}$$















### Founding Idea
What if the Lorentz factor is just a linear approximation of a true Lorentz Factor?
$$\begin{align}
\gamma&=\dfrac{1}{\sqrt{1-\tfrac{v^2}{c^2}}} && \text{(Relativistic Gamma)}\\
\gamma&=\dfrac{1}{\sqrt{1-\tfrac{2GM}{c^2r}}} && \text{(Gravitational Gamma)}
\end{align}$$
Setting those equal, we see:
$$\begin{align}
v^2&=\dfrac{2GM}{r} &\implies&& \dfrac{1}{2}mv^2&=\dfrac{GMm}{r}
\end{align}$$
This is just classical Kinetic and Potential Energies. However, we know that both these kinds of energies are just first-order approximations in their relativistic types.
$$\begin{align}
K(v)&=(\gamma(v)-1)mc^2\\
&=\dfrac{1}{2}m\dfrac{v^2}{c^2}c^2+\dfrac{3}{8}m\dfrac{v^4}{c^4}c^2+\dfrac{5}{16}m\dfrac{v^6}{c^6}c^2+\dfrac{35}{128}m\dfrac{v^8}{c^8}c^2+\dots\\
&=\dfrac{1}{2}mv^2\left(1+\dfrac{3}{4}\beta^2+\dfrac{5}{8}\beta^4+\dfrac{35}{64}\beta^6+\dots\right)\\
\end{align}$$
So what if the Lorentz Factor is just a linear approximation, then it would be written with Classical Kinetic Energy as:
$$\begin{align}
\gamma&=\dfrac{1}{\sqrt{1-2\dfrac{K}{E_0}}}
\end{align}$$
We will ignore a potential for the time being.

We know the total energy is $E=K+E_0$, and so:
$$\begin{align}
\gamma&=\sqrt{\dfrac{E_0}{3E_0-2E}}
\end{align}$$
Rearranging for total energy we get:
$$\begin{align}
E&=\left(\dfrac{3}{2}-\dfrac{1}{2\gamma^2}\right)E_0
\end{align}$$









Something else of note, let $\gamma$ be the following:
$$\begin{align}
\gamma&=-\dfrac{1}{\sqrt{1+\beta^2}}
\end{align}$$
We can then see the following Taylor expansion around $\beta=0$:
$$\begin{align}
\gamma&=1-\dfrac{1}{2}\beta^2+\dfrac{3}{8}\beta^4-\dfrac{5}{16}\beta^6+\dfrac{35}{128}\beta^8+\dots\\
\end{align}$$
