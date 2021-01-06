For the file entitled GCNN_attempt.ipynb 
The code in this jupyter notebook recreates work undertaken in November that was overwritten due to OneDrive syncing issues and follows deepchem github tutorials.
Once Oran and I had solved why deepchem was not functioning I set out to try and get predictive scores out of a deepchem model. 
It is worth noting that some parameters such as epoch could be optimised whilst others such as dense layer number / size could not. 
As we realised this system did not allow attenuation of datasets due to errors in the deepchem CSV loader function and batch normalization, further investigation of hyperparameter optimization was sidelined. Unfortunately due to the fact deepchem doesn't have functions for cross validation - head on statistical comparison between GCNN_attempts results and results from workingNOTEBOOK.ipynb (where Oran created a cross validation fn) are not possible in the time frame.
___________________________________
For the file entitled workingNOTEBOOK.ipynb
The code in this jupyter notebook responds to deepchem's faulty CSV loader and batch normalization. The grand majority of the code in this file was created by Oran and uses a custom package created in the last few weeks of the report which replaces parts of the DeepChem package that were restricting our ability to feed models attenuated datasets. As can be seen, it is not possible to change the number of dense layers, change the epoch, change the learning rate etc which means the loss function could not be minimised.
