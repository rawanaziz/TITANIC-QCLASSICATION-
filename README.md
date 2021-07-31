# TITANIC-QCLASSICATION
# UNDERSTANDING FEATURES  MAP IN QISKIT  :
We Know that features map to reduce the dimension of the features. In Qiskit libaray (platframe), there are 3 common feature maps :
1-ZFeautre map 
2-ZZ feautre map 
3- 
Besides, you can build your feature map as you want.
The main problem here, that the  number of features have to be equal to the number of the wires of the circuit  (lines, q0----qn):


Three steps to check if your features map is suitable your dataset or  not :

- You have to choose the most suitable features for your dataset, by statistic way, machine learning, data mining ...etc.
- You have to decide how many features you want to use, you have to remember the Backend as simulation, the highest number of the qubit is 32, for example (qasm_simulator).
- Depending on the dataset you will choose ZZFeautre map  , Zfeautre map ,... etc
ZZ feature map :
![image](https://user-images.githubusercontent.com/61630088/127745285-c00beae0-b353-47a3-912c-b7d9128d0633.png)
![image](https://user-images.githubusercontent.com/61630088/127745432-5f394a77-0068-4040-bf4c-45ac8f51a14d.png)

Z feature map :
![image](https://user-images.githubusercontent.com/61630088/127745277-66d281c2-25e9-405f-ae18-e09b1906aeb1.png)

![image](https://user-images.githubusercontent.com/61630088/127745425-b61a493c-f10c-4925-b687-ad36d8765242.png)
 
 
How to know is the suitable, you can by checking the score the classification report .
let see the classifaction of titanic using QSVC :


![image](https://user-images.githubusercontent.com/61630088/127745459-0e809c71-16f0-43d9-9e59-f4dcef48b7d0.png)


By the score , we figuer out that more suitable feautre map is  ZZ feautre.


References  :
https://www.kaggle.com/c/titanic/
https://sooluthomas.github.io/testTranslation/aqua/feature_maps.html
https://numpy.org/
https://pandas.pydata.org/
