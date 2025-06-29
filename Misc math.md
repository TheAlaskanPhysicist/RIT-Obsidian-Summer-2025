Let the directions $\{\vec{v}_1,\vec{v}_2,\dots,\vec{v}_d\}\subset\mathbb{R}^d$.
Each direction has a probability associated $\{p_1,p_2,\dots,p_d\}$, where $\sum p_k=1$.

$$\begin{align}
\mathbb{E}[\vec{X}_N]=\sum_i\mathbb{E}[\vec{S}_i]=N\sum_kp_k\vec{v}_k
\end{align}$$




### Complicated Random Walk
Basis & Probabilities depends position and time.
However, this field should be smooth.

#### 2D Idea
The directions $\vec{s}$ are now parametrized by $\theta$:
$$\begin{align}
\vec{s}(\vec{x},t,\theta)&=r(\vec{x},t,\theta)\hat{s}(\theta)=r(\vec{x},t,\theta)\begin{bmatrix}\cos\theta\\\sin\theta\end{bmatrix}
\end{align}$$
With associated probabilities:
$$\begin{align}
p(\vec{x},t,\theta)
\end{align}$$
To make sure probability is always 100%, we see that:
$$\begin{align}
\int_0^{2\pi} p(\vec{x},t,\theta)\ d\theta&=1
\end{align}$$

The expected value of a single displacement:
$$\begin{align}
\vec\mu(\vec{x},t)&=\mathbb{E}[\vec{s}]\\
&=\int_0^{2\pi}\vec{s}(\vec{x},t,\theta)\cdot p(\vec{x},t,\theta)\ d\theta
\end{align}$$
And the variance of a single displacement:
$$\begin{align}
\vec\Sigma(\vec{x},t)&=\mathbb{E}[(\vec{s}-\vec\mu)(\vec{s}-\vec\mu)^T]\\
&=\int_0^{2\pi}(\vec{s}-\vec\mu)(\vec{s}-\vec\mu)^T\cdot p(\vec{x},t,\theta)\ d\theta
\end{align}$$



### Spacetime Walks
At point $x^\mu\in\mathcal{M}$, we define the following:

A local basis $e_\mu^{(a)}(x)$ where:
$$\begin{align}
g_{\mu\nu}(x)&=\eta_{ab}e_\mu^{(a)}(x)e_\nu^{(b)}(x)
\end{align}$$
And tangent vector $\delta x^\mu$ parametrize possible displacements.


There exists a local probability distribution satisfying:
$$\begin{align}
\int P(\delta x; x)\ d^4(\delta x)&=1
\end{align}$$
We want to have a density centered around the classical path direction $u^\mu(x)$, with small fluctuations, so lets assert a Gaussian (covariant) since Gaussians show up everywhere:
$$\begin{align}
P(\delta x; x)&=\dfrac{1}{\sqrt{(2\pi)^4\det|\Sigma(x)|}}\exp\left(-\dfrac{1}{2}\Sigma^{-1}_{\mu\nu}(x)\delta x^\mu\delta x^\nu\right)
\end{align}$$
We let $\delta x^\mu=u^\mu(x)\cdot\delta\tau$, and there have the probability density:
$$\begin{align}
P(\delta x; x)&=\dfrac{1}{\sqrt{(2\pi)^4\det|\Sigma(x)|}}\exp\left(-\dfrac{1}{2}\Sigma^{-1}_{\mu\nu}(x)u^\mu u^\nu\delta\tau^2\right)
\end{align}$$
We can write a generalized diffusion equation as the following:
$$\begin{align}
\dfrac{\partial\rho}{\partial\tau}&=-\nabla_\mu\left(\rho u^\mu\right)+\nabla_\mu\nabla_\nu\left(\Sigma^{\mu\nu}\rho\right)
\end{align}$$




