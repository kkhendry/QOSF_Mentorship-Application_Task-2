# QOSF_Mentorship-Application_Task-2
The jupyter notebook enclosed in this repository presents solutions and extensions to Task 2 of the October 2021 QOSF (Quantum Open Source Foundation) Mentorship Application.

Task 2 Description: Train a variational quantum circuit to transform 4 random 4-qubit input states to the following target states:
|0011>
|0101>
|1010>
|1100>

The solutions presented below make use of the Qiskit open-source SDK and draws inspiration from [1] ["A generative modeling approach for benchmarking and training shallow quantum circuits"](https://www.nature.com/articles/s41534-019-0157-8.pdf). 

Section 1 builds up the overall problem structure and present a solution which uses a simplified version of the data driven approach taken in [1]. In section the problem structure, cost functions, gradient functions and optimizers are built without the use of any ML (Machine Learning) libraries such as Tensorflow or Pytorch. The optimizer and gradient fucntions have in built flexibility to allow for investigation of the best solution through hyperparameter tuning and gradient evaluation. The executed cells below present a finite different gradient descent approach using a TwoLocal ansatz made up of RX, RY and CX gates. The results of section 1 demonstrate a solution that performs the task fairly well but can certainly be improved through further investigation into the ansatz, gradient function and optimizer.

Section 2 uses the basic problem structure from section 1 and attempts to implement some of Qiskit's more sophistaicated in-built gradient functions and optimizers. The results were not as successful as those in Section 1 and the running times experienced were longer.
