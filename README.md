## AI-Risk Analytics Projects

This repository includes three machine learning projects I developed independently during my Master of Science in Information Systems (MSIS) program. Each project explores a different cybersecurity challenge using applied machine learning. All models were built using Python and common data science libraries such as `scikit-learn`, `pandas`, `numpy`, and `matplotlib`.

---

### P1: Encryption Method Classifier

**Goal**  
Classify whether an encrypted message was generated using a Caesar or Playfair cipher based on a given plaintext/ciphertext pair.

**My Process**  
- Generated 500 plaintext samples and encrypted them using the `pycipher` library  
- Combined plaintext and ciphertext into single 18-character strings  
- Converted characters into numeric features  
- Trained a Logistic Regression model that achieved 100% test accuracy

**Lessons Learned**  
This project showed how machine learning can identify hidden structure and patterns even in classical encryption techniques.

[Project1.pdf](./Project1.pdf) 
[Encryption_Classifier(P1).ipynb](./Encryption_Classifier(P1).ipynb)


### P2: Detecting Network Attacks

**Goal**  
Detect whether network traffic is benign or part of an attack (e.g., DoS, Port Scan, DDoS) using supervised learning.

**My Process**   
- Explored and cleaned a dataset with over 1,500 features  
- Trained and tuned Decision Tree and Random Forest classifiers  
- Used Logistic Regression as a baseline  
- Evaluated models using confusion matrices, ROC curves, and F1 scores

**Lessons Learned**   
This project helped me better understand model complexity and overfitting, especially in high-dimensional security datasets. I saw firsthand how tree ensembles like Random Forests can generalize better than single trees and baselines when dealing with noisy attack data.

[Project2.pdf](./Project2.pdf)  
[GoodorBadNetworkPacket(P2).ipynb](./GoodorBadNetworkPacket(P2).ipynb)



### A3: Intrusion Detection with Adversarial Inputs

**Goal**  
Develop a neural network-based intrusion detection system and evaluate its ability to withstand adversarial modifications to malicious traffic.

**My Process**  
- Trained a baseline MLP (Multi-Layer Perceptron) model  
- Created adversarial inputs using controlled noise (epsilon-based perturbation)  
- Built two defenses:
  - Adversarial training (retraining with perturbed data)
  - Ensemble method combining MLP and Random Forest via soft voting  
- Evaluated performance across clean and perturbed inputs using accuracy, precision, recall, and false positive rate

**Lessons Learned**  
This project taught me the tradeoffs between robustness and precision in adversarial defense. Adversarial training helped the model resist attack samples but raised false positives, while the ensemble approach struck a better balance without extra retraining. It deepened my understanding of real-world security model constraints.

[Project3.pdf](./Project3.pdf) 
[NeuralNetworkIDS(P3).ipynb](./NeuralNetworkIDS(P3).ipynb)


## License

This code is not licensed for reuse or redistribution. Please contact me before using any part of this work.


