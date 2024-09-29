# Sistema-de-Compressao

Desafio de sistema de compressão. Resolver o sistema com uma rede neural para prever eventos futuros, usando o método da PIRNN.

Equações:

$ \frac{d\dot{m}}{dt} = \frac{A_1}{L_C}(\phi (N(t), \dot{m})P_1 - P_P(t)) $

$ \frac{d P_P}{dt} = \frac{C_1^2}{\nu _P}(\dot{m}(t) - \alpha (t) K_\nu \sqrt{P_P - P_{out}}) $

$ \begin{matrix} A_1 & = & 2.6\centerdot 10^-3 m² \\
\nu _P & = & 2.0 m³ \\
L_C & = & 2.0 m \\
K_\nu & = & \frac{0.38 kg}{(kPa)^{0.5}s} \\
P_1 & = & 4.5 Bar \\
P{out} & = & 5.0 Bar \end{matrix}
$

$ \frac{d\dot{m}}{dt} = \frac{2.6\centerdot 10^{-3}}{2.0}(1.5\centerdot 4.5 - P_P) $

$ \frac{d P_P}{dt} = \frac{479.029^2}{2.0}(\dot{m} - \alpha {0.38} \sqrt{P_P - 5.0}) $

Bibliotecas:
- Numpy
- TensorFlow 2.17.0
- Keras 3.5.0
- Casadi 3.6.6
- Scipy
- Plotly 5.24.1
