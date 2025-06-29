5/27/2025

LAST SECTION 4.1: pg. 




### Time-Dependent Coordinates Definitions
For the sake of the document, I will be using the following compressions for coordinate dynamics.
$$\begin{align}
g_{ij}&=e_i\cdot e_j && \text{(Metric Tensor)}\\
\omega_{ij}&=e_i\cdot\dfrac{de_j}{dt} && \text{(Frame Velocity Tensor)}\\
\alpha_{ij}&=e_i\cdot\dfrac{d^2e_j}{dt^2} && \text{(Frame Acceleration Tensor)}\\
\epsilon_{ij}&=\dfrac{de_i}{dt}\cdot\dfrac{de_j}{dt} && \text{(Inertial Strain Tensor)}\\
\sigma_{ij}&=\dfrac{de_i}{dt}\cdot\dfrac{d^2e_j}{dt^2} && \text{(Frame Sheer Tensor)}\\
\epsilon_{ij}^{(2)}&=\dfrac{d^2e_i}{dt^2}\cdot\dfrac{de_j^2}{dt^2} && \text{(Inertial Stretch Tensor)}\\
\end{align}$$






## Tensor Quantities (Time-Dependent Coordinates)
I will be using condensed notations, including the following:
$$\begin{align}
\delta^i_j&=e^ie_j && \text{(Duality Condition)}\\
\bra{a}&=a_ie^i && \text{(Row/Bra 1-Form)}\\
\ket{a}&=a^ie_i && \text{(Col/Ket 1-Vector)}\\
\braket{a|a}=\vec{a}^2&=g_{ij}a^ia^j && \text{(Inner Product)}\\
\end{align}$$
---
### Position
$$\begin{align}
\vec{r}&=r^ie_i\\
\vec{r}^2&=g_{ij}r^ir^j
\end{align}$$
---
### Velocity
#### Standard Notation
$$\begin{align}
\vec{v}&=\left(\dfrac{dr^i}{dt}+r^j\omega_j^i\right)e_i=v^ie_i\\
\vec{v}^2&=g_{ij}\left(\dot{r}^i\dot{r}^j+(r^k\omega_k^i)\dot{r}^j+\dot{r}^i(r^l\omega_l^j)+(r^k\omega_k^i)(r^l\omega_l^j)\right)
\end{align}$$
#### Stanley's Notation
$$\begin{align}
\vec{v}&=\dot{r}^ie_i+r^i\dot{e}_i\\
\vec{v}^2&=g_{ij}\dot{r}^i\dot{r}^j+\omega_{ij}\dot{r}^ir^j+\omega_{ji}r^i\dot{r}^j+\epsilon_{ij}r^ir^j\\
\end{align}$$
---
#### Acceleration
**Standard Notation**
$$\begin{align}
\vec{a}&=\left(\dfrac{d^2r^i}{dt^2}+r^j\omega_j^i\right)e_i+\left(\dfrac{dr^i}{dt}+r^j\omega_j^i\right)\omega_i^ke_k
\end{align}$$
**Stanley's Notation**
$$\begin{align}
\vec{a}&=\ddot{r}^ie_i+2\dot{r}^i\dot{e}_i+r^i\ddot{e}_i\\
\vec{a}&=g_{ij}\ddot{r}^i\ddot{r}^j+2\left(\omega_{ij}\ddot{r}^i\dot{r}^j+\omega_{ji}\dot{r}^i\ddot{r}^j\right)+\left(\alpha_{ij}\ddot{r}^ir^j+\alpha_{ji}r^i\ddot{r}^j\right)\\
&\ \ \ \ +4\epsilon_{ij}\dot{r}^i\dot{r}^j+2\left(\sigma_{ij}\dot{r}^ir^j+r^i\dot{r}^j\sigma_{ji}\right)+\epsilon_{ij}^{(2)}r^ir^j\\


\end{align}$$
---










### Physical Quantities
#### Quantities
$$\begin{align}
\vec{r}&=r^ie_i && \text{(Position)}\\
\vec{v}&=\dfrac{dr^i}{dt}e_i+r^i\dfrac{de_i}{dt} && \text{(Velocity)}\\
&=v^ie_i+r^i\dfrac{de_i}{dt}\\
\vec{a}&=a^ie_i+2v^i\omega_i+r^i\alpha_i && \text{(Accleration)}\\
\vec{p}&=m\vec{v} && \text{(Classical Momentum)}\\
\vec{F}&=m\vec{a} && \text{(Classical Force)}\\
\end{align}$$
#### Squared Quantities (Metric Notation)
$$\begin{align}

\vec{v}^2&=g_{ij}v^iv^j+\Omega_{ji}r^iv^j+\Omega_{ij}v^ir^j+\omega_{ij}r^ir^j\\
\vec{v}^2&=g_{ij}v^iv^j=g_{ij}\left(\right)\\
\end{align}$$







### Rest of Document
For the rest of the document, lets define:
$$\begin{align}
\dfrac{de_i}{dt}&=\omega_i & \dfrac{d^2e_i}{dt^2}&=\alpha_i\\
\end{align}$$



$$\begin{align}
\vec{v}^2&=v_ie^i+r_i\dfrac{de^i}{dt}+v^je_j+r^j\dfrac{de_j}{dt}

\end{align}$$


$$\begin{align}
\vec{r}\cdot\vec{r}&=g_{ij}r^ir^j\\
\end{align}$$

For the basis components, we will use the following:
$$\begin{align}
g_{ij}&=e_i\cdot e_j\\
\Omega_{ij}&=e_i\cdot\dfrac{de_j}{dt}\\
\omega_{ij}&=\dfrac{de_i}{dt}\cdot\dfrac{de_j}{dt}\\
\end{align}$$



$$\begin{align}
g_{ij}&=e_i\cdot e_j\\
\Gamma_{ij}&=e_i\cdot\dfrac{de_j}{dt}\\
\omega_{ij}&=\dfrac{de_i}{dt}\cdot\dfrac{de_j}{dt}\\
\end{align}$$
