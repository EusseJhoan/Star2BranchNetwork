# Certification of nonlocality on a two-branch node quantum network using the quantum computer *ibm_kyiv*

## Summary
![esquema](https://github.com/user-attachments/assets/4da495e8-967d-40d6-8d03-09774c569bc7)

In this project, the two-branch star network depicted above was replicated in the quantum computer *ibm-kyiv*, based on the procedures proposed in the article [npj
Quantum Information 2021 7:1 7, 1 (2021)](https://www.nature.com/articles/s41534-021-00450-x). 
In addition, it was verified that the correlations between the results obtained in the two-branch star violate the Bell-type inequality $S_2 \equiv \sqrt{|I_1|} + \sqrt{|I_2|} \leq 1$, thus certifying the nonlocality of the studied network.

## Authors
* Jhoan Eusse

## Files
* [Circuits.ipynb: ](https://github.com/EusseJhoan/Star2BranchNetwork/blob/main/Circuits.ipynb) Notebook to build the required quantum circuits to model the two-node star network. It is important to highlight that in this notebook we did not run the circuits, we ran them directly on the [IBM Quantum Plataform](https://quantum.ibm.com/).
* [StarBSM_kyiv.ipynb: ](https://github.com/EusseJhoan/Star2BranchNetwork/blob/main/StarBSM_kyiv.ipynb) Notebook with the statistical analysis to calculate the Bell inequality from quantum computer data.
* [data: ](https://github.com/EusseJhoan/Star2BranchNetwork/tree/main/data) Folder that contains the data generated through IBM Quantum Plataform to model the network. Each file inside the folder contains the data generated for a particular setting of Alice and Charile's measurements. 

## Execution
Execute the notebook [StarBSM_kyiv.ipynb ](https://github.com/EusseJhoan/Star2BranchNetwork/blob/main/StarBSM_kyiv.ipynb) to calculate the value $S_n$ based on the data contained on the folder [data](https://github.com/EusseJhoan/Star2BranchNetwork/tree/main/data).

Execute the notebook [Circuits.ipynb](https://github.com/EusseJhoan/Star2BranchNetwork/blob/main/Circuits.ipynb) if you want to create the circuits to model the network using [Qiskit](https://www.ibm.com/quantum/qiskit) python library. You can also reproduce the circuits directly on the IBM Quantum Plataform.

## Results
With the data yielded by the *ibm-kyiv* quantum computer, a value of $S_2= 1.113$ was obtained, which violates Bell's inequality, $S_2 \leq 1$, indicating that the two-branch star quantum network exhibits nonlocal correlations.
