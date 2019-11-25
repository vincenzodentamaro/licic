# licic
Less Important Components for Imbalanced multi-class Classification - LICIC
##Abstract: 
Multiclass classification in cancer diagnostics, using DNA or Gene Expression Signatures, but also classification of bacteria species fingerprints in MALDI-TOF mass spectrometry data, is challenging because of imbalanced data and the high number of dimensions with respect to the number of instances. In this study, a new oversampling technique called LICIC will be presented as a valuable instrument in countering both class imbalance, and the famous “curse of dimensionality” problem. The method enables preservation of non-linearities within the dataset, while creating new instances without adding noise. The method will be compared with other oversampling methods, such as Random Oversampling, SMOTE, Borderline-SMOTE, and ADASYN. F1 scores show the validity of this new technique when used with imbalanced, multiclass, and high-dimensional datasets.

##Cite
Dentamaro, V., Impedovo, D., & Pirlo, G. (2018). LICIC: Less Important Components for Imbalanced Multiclass Classification. Information, 9(12), 317.

https://www.mdpi.com/2078-2489/9/12/317/htm

## Example usage
    from sklearn import datasets
    iris = datasets.load_iris()
    x = iris.data
    y = iris.target
    licic = LICIC()
    x,y = licic.fit_sample(x,y)
    print(x)
    print(y)
