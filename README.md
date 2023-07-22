In this paper, the authors proposed method, known as conservative physics-informed neural network (cPINN), addresses nonlinear conservation laws on discrete domains. The discrete domains are obtained by dividing the computational domain, and the cPINN enforces flux continuity in the strong form at the interfaces between sub-domains. cPINN enforces an average solution at the common interface between two sub-domains, utilizing two different neural networks. It allows flexibility in using deep neural networks for complex solutions in the domain and shallow neural networks in sub-domains with relatively simple and smooth solutions. The method discusses different types of errors, including optimization, generalization, and approximation errors, and their sources in cPINN. Locally adaptive activation functions are employed, resulting in faster model training compared to fixed counterparts.

Both forward and inverse problems are solved using cPINN. The method is successfully applied to various test cases, such as scalar nonlinear conservation laws (e.g., Burgers, Korteweg–de Vries equations). It also tackles the lid-driven cavity test case governed by incompressible Navier–Stokes equations, and the results are compared against a benchmark solution.

One of the advantages of cPINN is its domain decomposition property, using separate neural networks in each sub-domain. This enables efficient parallelized computation, with each sub-domain assigned to a different computational node. cPINN lets the neural networks share information through the interfaces for different sub-domains
