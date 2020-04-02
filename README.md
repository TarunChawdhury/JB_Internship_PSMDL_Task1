# JetBrains_Internship_PSMDL_Task1

Решение **Задачи 1** в заявке для проекта *Предсказание синтезируемости молекул лекарств с помощью глубокого обучения*.

Для запуска решения необходимо выполнить все requirements из [README](https://github.com/korney3/JetBrains_Internship_PSMDL_Task1/blob/master/chemical_vae/README.md) оригинального репозитория.

Код для закодирования, декодирования и предсказывания свойств молекул:

* Cc1ccc(S2(=O)=NC(=O)Nc3ccccc32)cc1
* CN(Cc1ccc2c(c1)C(=O)CC2)C(=O)OC(C)(C)C
* COC(=O)C1CCC(Oc2ccc(NC(=O)C(=O)NN)cn2)CC1

находится в Jupyter notebook [Solution.ipynb](https://github.com/korney3/JetBrains_Internship_PSMDL_Task1/blob/master/Solution.ipynb)

## Ответ

|Original SMILES|Encoded representation Z|Decoded SMILES|Properties|
|---|---|---|---|
|Cc1ccc(S2(=O)=NC(=O)Nc3ccccc32)cc1|**shape** (1, 196) with **norm** 10.274|C(cccc(C[n+]2=NC(=O)Nc3ccccc32)cc1|**qed**: 0.723, **SAS**: 2.410, **logP**: 3.147|
|CN(Cc1ccc2c(c1)C(=O)CC2)C(=O)OC(C)(C)C|**shape** (1, 196) with **norm** 13.454|CN(C)cccc2c(c1)C(=O)CC2)C(=O)OC(C)(C)C|**qed**: 0.723, **SAS**: 2.410, **logP**: 2.438|
|COC(=O)C1CCC(Oc2ccc(NC(=O)C(=O)NN)cn2)CC1|**shape** (1, 196) with **norm** 13.123|COC(=O)C1CCC(Oc2ccc(NC(=O)C(=O)NN)cn2)CC1|**qed**: 0.753, **SAS**: 2.478, **logP**: 0.050|
