# Special Functions

## Trigonometric functions

### csc

$$ \csc(x) = \frac{1}{\sin(x)} $$

## Hyperbolic Functions

### sinh

$$ \sinh z\equiv \frac{1}{2} (e^z-e^{-z}) $$

### cosh

$$ \cosh z \equiv \frac{1}{2}(e^z+e^{-z}) $$

### tanh


\begin{align}
\tanh (x) &= \frac{\sinh (x)}{\cosh (x)} \\
\frac{\partial \tanh (x)}{\partial x} &= \text{sech}^2(x) \\
\int \tanh (x) \, dx &= \log (\cosh (x))
\end{align}

<div align=center><img src="../special_func.assets/tanh.png" alt="tanh" style="zoom:60%;" /></div>


## Gamma Function

$$\Gamma (z)=\int _0^{\infty } t^{z-1} e^{-t}  \,dt$$

### Properties & Relations

$$\Gamma(z)\Gamma(1-z) \equiv \pi \csc(\pi z)$$

## Error Function

$$\text{erf} (z)=\frac{2}{\sqrt{\pi }}\int_0^z e^{-t^2} \,dt$$

### Complementary Error Function

$$ \text{erfc} (z) = 1-\text{erf} (z) $$

### Imaginary Error Function

$$ \text{erfi} (z) = \frac{\text{erf} (iz)}{i} $$

## Bessel Function

### Bessel function of the first kind

$J_n(z)$ satisfies the differential equation $z^2y''+zy'+(z^2-n^2)y=0$.

#### Properties

$$\frac{dJ_n(x)}{dx}=\frac{1}{2}(J_{n-1}(x)-J_{n+1}(x))$$

### Bessel function of the second kind

$Y_n(z)$ satisfies the differential equation $z^2y''+zy'+(z^2-n^2)y=0$. 
