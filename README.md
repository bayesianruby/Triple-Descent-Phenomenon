# Triple-Descent-Phenomenon

The "double-descent" phenomenon appears while increasing the number of training examples N.  The generalization error of neural networks appears to peak when N is of the same order as the number of parameters P. A similar phenomenon is shown to exist in simpler models such as linear regression, where the peak instead occurs when N is equal to the input dimension D.

The paper [1] shows that these two scenarios are inherently different. In this work we focus on certain experiments of the paper and display that the relative size of the peaks is governed by the degree of nonlinearity of the activation function.

The **nonlinear peak** at N = P is a true divergence caused by **the extreme sensitivity of the output function** to both the noise corrupting the labels and the initialization of the random features. This peak survives in the absence of noise, but can be suppressed by regularization

In contrast, the **linear peak** at N = D is solely due to overfitting the noise in the labels. This peak is implicitly regularized by the nonlinearity.


The results display the effects of the non-linearity of the activation function as it follows: 
<img width="400" alt="Capture d’écran 2022-06-18 à 23 18 40" src="https://user-images.githubusercontent.com/80846462/174457337-e8b9181f-f093-493c-92da-ea27c8dcd79b.png">



[1] Stéphane d'Ascoli, Levent Sagun, Giulio Biroli. Triple descent and the two kinds of overfitting: Where & why do they appear?. France. 2020. ⟨hal-02983803⟩




