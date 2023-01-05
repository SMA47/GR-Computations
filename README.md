# GR-Computations
A set of codes to compute Christoffel symbols, Riemann tensor (1,3), Riemann tensor (0,4) and the Ricci Tensor using python and the sympy library

Christoffell_symbols:- Contains the metric tensor and any varibales that may be needed for the metric tensor.
A list (array) of coordinates is also present in this file.

Riemann_tensor13:- This file computes the riemann tensor (1,3) variant. It uses the christoffel symbols file to compute the christoffel symbols required.
Computations can be made faster by removing the for loop in the Riemann_Tensor()function as this for loop only for the Einsteins summation law.

Riemann_tensor04:- This file computes the reimann tensor(0,4) variant.
This file achieves this by simply computing the Riemann_Tensor using the Riemann_Tensor13 file and multiplying it by the metric tensor found in the Christoffel_symbols file.

Ricci tensor:- This file Computes the Ricci tensor using the Christoffel_symbols file.
This file does not need the Riemann Tensor files as it uses a definition of the ricci tensor that only requires the Christoffel symbols.
Although the Ricci tensor has only 2 indices the code takes a while to give it's first output due to the use of the Einstein summation law used to compute it.

Note: To compute any single just uncomment the nested for loops at the end of each file.
