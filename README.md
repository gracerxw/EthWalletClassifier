# Ethereum Wallet Classifier

# About

**CZ1115 DSAI Mini Project Submission**

This project tries to identify Ethereum wallet addresses that belong to centralised exchanges, as opposed to user owned wallets. 

Since the Web3 space is growing exponentially, more and more users are joining the space, and many of them are not particularly educated about the space. This leads to many scams and we want to try and reduce that as much as possible. 

By deanonymizing the ownership of wallet addresses, we hope to be able to help people identify proper CEX wallets, and verify that they are depositing their crypto into the right wallet address, as opposed to a potentialy scammer's user wallet. 

This classifier might also prove to be useful to protocols that might want to airdrop stuff to random wallets, but want to excluse CEX wallets as well.

Our project is split into 5 main sections:

* [Data Extraction](https://github.com/matthew-chua/EthWalletClassifier/blob/main/DataExtraction.ipynb)
* [Data Cleaning](https://github.com/matthew-chua/EthWalletClassifier/blob/main/CleanData.ipynb)
* [EDA](https://github.com/matthew-chua/EthWalletClassifier/blob/main/EDA.ipynb)
* [Predictor Exploration](https://github.com/matthew-chua/EthWalletClassifier/blob/main/ExploringPredictors.ipynb)
* [Fine Tuning Models](https://github.com/matthew-chua/EthWalletClassifier/blob/main/TuningModels.ipynb)

---

# Contributors

- @marctan2705 - KNN / Grid Search
- @gracerxw - Decision Tree / Data Cleaning
- @matthew-chua Data Extraction / Random Forests

---

# Problem Definition

We want to find out if it is possible to classify wallet addresses into hot wallets belonging to **centralised exchanges** and **normal user wallets,** using data available on Etherscan.

---

# Models Used

- Decision Tree
- Random Forests
- K-Nearest Neighbour

---

# Conclusion
We managed to get a classification accuracy of more than 90% with the Random Forest model, with a decently low FPR and FPN.
However, it is worth noting that our dataset is rather small as well, which might lead to a slight amount of overfitting.
Possible future improvements could involve using BiqQuery to collect a larger dataset, from which a better model can be trained on.

---

# Learning Points

- Web Scrapers
- How CEXs utilise their hot wallets
- How KNN works

---

# References

https://medium.com/trm-insights/how-we-used-machine-learning-to-label-one-million-ethereum-addresses-e69c96a841b9

https://etherscan.io
