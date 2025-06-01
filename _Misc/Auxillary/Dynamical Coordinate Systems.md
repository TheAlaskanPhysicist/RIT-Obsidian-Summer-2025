



### Definitions
$$\begin{align}
\dfrac{\partial e_i}{\partial t}&=\Omega_{(t)i}^ke_k\\
\dfrac{\partial e_i}{\partial x^j}&=\Omega_{(j)i}^ke_k\\
\end{align}$$



### Tensor Quantities
$$\begin{align}
\vec{r}&=r^ie_i\\
\vec{v}&=\left[\dfrac{\partial r^i}{\partial t}+\dfrac{\partial r^i}{\partial x^j}\dfrac{dx^j}{dt}\delta_i^k+r^i\left(\Omega_{(t)i}^k+\Omega_{(j)i}^k\dfrac{dx^j}{dt}\right)\right]e_k\\
\end{align}$$



$$\begin{align}
\vec{r}&=r^ie_i\\
\vec{v}&=v^ke_k & v_k&=\left[\dfrac{\partial r^i}{\partial t}+\dfrac{\partial r^i}{\partial x^j}\dfrac{dx^j}{dt}\delta_i^k+r^i\left(\Omega_{(t)i}^k+\Omega_{(j)i}^k\dfrac{dx^j}{dt}\right)\right]\\
\end{align}$$





$$\begin{align}
g_{ij}=g_{ij}^{[0,0]}&=e_i\cdot e_j && \text{(Metric Tensor)}\\
\omega_{ij}=g_{ij}^{[0,1]}&=e_i\cdot\dfrac{de_j}{dt} && \text{(Frame Velocity Tensor)}\\
\omega_{ij}=g_{ij}^{[0,2]}&=e_i\cdot\dfrac{d^2e_j}{dt^2} && \text{(Frame Acceleration Tensor)}\\
\epsilon_{ij}=g_{ij}^{[1,1]}&=\dfrac{de_i}{dt}\cdot\dfrac{de_j}{dt} && \text{(Inertial Strain Tensor)}\\
\sigma_{ij}=g_{ij}^{[1,2]}&=\dfrac{de_i}{dt}\cdot\dfrac{d^2e_j}{dt^2} && \text{(Frame Sheer Tensor)}\\
\epsilon_{ij}^{(2)}=g_{ij}^{[2,2]}&=\dfrac{d^2e_i}{dt^2}\cdot\dfrac{de_j^2}{dt^2} && \text{(Inertial Stretch Tensor)}\\
\end{align}$$