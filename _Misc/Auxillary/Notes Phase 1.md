5/27/2025

LAST SECTION 4.1: pg. 






### Physical Quantities
I will be using condensed notations, including the following:
$$\begin{align}
\delta^i_j&=e^ie_j && \text{(Duality Condition)}\\
\bra{a}&=a_ie^i && \text{(Row/Bra 1-Form)}\\
\ket{a}&=a^ie_i && \text{(Col/Ket 1-Vector)}\\
\braket{a|a}=\vec{a}^2&=g_{ij}a^ia^j && \text{(Inner Product)}\\
\end{align}$$
---
#### Position
Position is typically represented as a contravariant vector:
$$\begin{align}
\vec{r}&=r^ie_i\\
\vec{r}^2&=g_{ij}r^ir^j
\end{align}$$
---
#### Velocity
We define $\Omega_j^i$ to be the *frame velocity tensor*, defined as:
$$\begin{align}
\Omega_j^i=e^i\cdot\dfrac{de_j}{dt}&&\implies&&\dfrac{de_j}{dt}=\Omega_j^ie_i\\
\Omega_{ij}=e_i\cdot\dfrac{de_j}{dt}&&\implies&&\Omega_{ij}=g_{ik}\Omega_j^k&&\implies&&\Omega_j^i=g^{ik}\Omega_{kj}\\
\end{align}$$
Velocity is typically represented as a contravariant vector, and so can be written as:
$$\begin{align}
\Aboxed{\vec{v}&=\left(\dot{r}^i+r^j\Omega_j^i\right)e_i}
\end{align}$$
And it's square:
$$\begin{align}
\vec{v}^2&=g_{ij}\left(\dot{r}^i+r^k\Omega_k^i\right)\left(\dot{r}^j+r^l\Omega_l^j\right)\\
&=g_{ij}\dot{r}^i\dot{r}^j+(g_{ij}\Omega_k^i)r^k\dot{r}^j+(g_{ij}\Omega_l^j)r^l\dot{r}^i+g_{ij}r^k\Omega_k^ir^l\Omega_l^j\\
\Aboxed{\vec{v}^2&=g_{ij}\dot{r}^i\dot{r}^j+\Omega_{ij}\dot{r}^ir^j+\Omega_{ji}\dot{r}^jr^i+
(g^{ij}\Omega_{ik}\Omega_{jl})r^kr^l}
\end{align}$$
---
#### Acceleration
We define $\Omega_j^i$ to be the *frame acceleration tensor*, defined as:
$$\begin{align}
A_j^i&=e^i\cdot\dfrac{d^2e_j}{dt^2}=\dot\Omega_j^i+\Omega_j^k\Omega_k^i&&\implies&&\dot\Omega_j^i=A_j^i-\Omega_j^k\Omega_k^i\\
A_{ij}&=g_{ik}A^k_j&&\implies&&A_j^i=g^{ik}A_{kj}
\end{align}$$
Acceleration is typically represented as a contravariant vector, and so can be written as:
$$\begin{align}
\vec{a}&=\left(\ddot{r}^i+\dot{r}^j\Omega_j^i+r^j\dot{\Omega}_j^i\right)e_i
        +\left(\dot{r}^j+r^i\Omega_i^j\right)\Omega_j^ke_k\\
&=\left(\ddot{r}^i+\dot{r}^j\Omega_j^i+r^jA_j^i-r^j\Omega_j^k\Omega_k^i\right)e_i
 +\left(\dot{r}^k+r^j\Omega_j^k\right)\Omega_k^ie_i\\
&=\left(\ddot{r}^i+\dot{r}^j\Omega_j^i+\dot{r}^k\Omega_k^i
 +r^jA_j^i-r^j\Omega_j^k\Omega_k^i+r^j\Omega_j^k\Omega_k^i\right)e_i\\
\Aboxed{\vec{a}&=\left(\ddot{r}^i+2\dot{r}^j\Omega_j^i+r^jA_j^i\right)e_i}
\end{align}$$
And it's square:
$$\begin{align}
\vec{a}^2&=
g_{ij}\left(\ddot{r}^i+2\dot{r}^k\Omega_k^i+r^kA_k^i\right)\left(\ddot{r}^j+2\dot{r}^l\Omega_l^j+r^lA_l^j\right)\\\\
&=g_{ij}\ddot{r}^i\ddot{r}^j+\left((g_{ij}A_k^i)r^k\ddot{r}^j+(g_{ij}A_l^j)\ddot{r}^ir^l\right)+2\left((g_{ij}\Omega_k^i)\dot{r}^k\ddot{r}^j+(g_{ij}\Omega_l^j)\ddot{r}^i\dot{r}^l\right)\\&+2\left(g_{ij}\Omega_l^jA_k^ir^k\dot{r}^l+g_{ij}\Omega_k^iA_l^jr^l\dot{r}^k\right)+4(g_{ij}\Omega_k^i\Omega_l^j)\dot{r}^k\dot{r}^l+(g_{ij}A_k^iA_l^j)r^kr^l\\\\
\Aboxed{\vec{a}^2&=g_{ij}\ddot{r}^i\ddot{r}^j+2A_{ij}\ddot{r}^ir^j+4\Omega_{ij}\ddot{r}^i\dot{r}^j+4(g^{ij}\Omega_{ik}\Omega_{jl})\dot{r}^k\dot{r}^l+4(g^{ij}\Omega_{ik}A_{jl})\dot{r}^kr^l+(g^{ij}A_{ik}A_{jl})r^kr^l}
\end{align}$$
---
#### Momentum
Momentum is typically represented as a covariant vector. Since $\vec{p}=m\vec{v}$, we can see that:
$$\begin{align}
\Aboxed{\vec{p}&=mg_{ij}\left(\dot{r}^j+r^k\Omega_k^j\right)e^i}
\end{align}$$
And it's square:
$$\begin{align}
\Aboxed{\vec{p}^2&=m^2g_{ij}\left(\dot{r}^i+r^k\Omega_k^i\right)\left(\dot{r}^j+r^l\Omega_l^j\right)}
\end{align}$$
---
#### Force
Force is typically represented as a covariant vector. Since $\vec{F}=m\vec{a}$, we can see that:

$$\begin{align}
\Aboxed{\vec{F}&=mg_{ij}\left(\ddot{r}^j+2\dot{r}^k\Omega_k^j+r^kA_k^j\right)e^i}
\end{align}$$
And it's square:
$$\begin{align}
\Aboxed{\vec{F}^2&=m^2g_{ij}\left(\ddot{r}^i+2\dot{r}^k\Omega_k^i+r^kA_k^i\right)\left(\ddot{r}^j+2\dot{r}^l\Omega_l^j+r^lA_l^j\right)}
\end{align}$$
---
#### Kinetic Energy
Kinetic Energy is represented as a scalar quantity with definition:
$$\begin{align}
T&=\dfrac{1}{2}m\vec{v}^2\\
\Aboxed{\vec{v}^2&=g_{ij}\dot{r}^i\dot{r}^j+\Omega_{ij}\dot{r}^ir^j+\Omega_{ji}\dot{r}^jr^i+(g^{ij}\Omega_{ik}\Omega_{jl})r^kr^l}
\end{align}$$









Angular momentum:
$$\begin{align}
\vec{L}&=\vec{r}\times\vec{p}
\end{align}$$

Center of Mass:
$$\begin{align}
M\vec{R}&=\int \vec{r}\ dm
\end{align}$$
Kinetic Energy:
$$\begin{align}
T&=\dfrac{1}{2}m\left(\vec{v}\cdot\vec{v}\right)\\
\dfrac{dT}{dt}&=
\end{align}$$


Linear Momentum is conserved
Angular Momentum is conserved

Is there a true total momentum conserved?











### Newton's First Law
In the absence of forces, a point particle moves with constant velocity $\vec{v}$.
> This only applies in Inertial Reference Frames


### Newton's Second Law
For any point particle of mass $m$, the net force $\vec{F}$ on the particle is always equal to the mass time acceleration of the particle's acceleration.
> This only applies in Inertial Reference Frames


### Newton's Third Law
The generation of forces must always come in pairs of equal and opposite value.
> This leads directly to the conservation of momentum.


No external forces $\implies$ Conserved momentum (over time).






Forces are "real," Potentials are not.
This is similar to $\vec{E}$ and $\vec{B}$ being "real," but $\phi$ and $\vec{A}$ are not.