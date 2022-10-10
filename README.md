# mod14challenge Algorithmic Trading

# Machine learning trading bot

Describe how machine learning is disrupting algorithmic trading in finance.

Write your own simple trading algorithm based on technical indicators.

Evaluate the performance of your trading algorithm by using backtesting and risk/reward characteristics.


---

## Technologies

Pandas

NumPy

hvPlot

Matplotlib

scikit-learn

---

### Files

machine_learning_trading_bot.ipynb 

---

Import libraries

<img width="564" alt="Screen Shot 2022-10-09 at 9 58 36 PM" src="https://user-images.githubusercontent.com/107937930/194793634-a82085c8-d3eb-4773-8caf-be3b1b0c5a54.png">


# Establish a Baseline Performance


cumulative return plot that shows the actual returns vs. the strategy returns.
This is a baseline performance for the Strategy vs Actual Returns using the SVM Training Algorithm 
based on 3 months of training data.


Using the trading signals SMA_Fast with parameter short_window = 4 Days, & SMA_Slow parameter long_window = 100. Based on the SVM model predictions that the precision for the -1 class is .43 and .56 for class 1. We can conclude that the higher model based on the SVM data is better at predicting the class 1 data .96 to class -1 at .04. 


<img width="480" alt="Screen Shot 2022-10-09 at 7 30 07 PM" src="https://user-images.githubusercontent.com/107937930/194786473-5985c4a5-9012-47ce-9878-3b4321b7a660.png">


<img width="592" alt="Screen Shot 2022-10-09 at 7 31 53 PM" src="https://user-images.githubusercontent.com/107937930/194786542-b09ccd89-5694-4a49-b6b8-f21ffeb3f8a0.png">



# Questions

 Q: What impact resulted from increasing or decreasing the training window?
 
 A: Increasing the training data to 10 months resulted to the training data being increasingly more 
 
 accurate. 
 
---

# Tune the Baseline Trading Algorithm

<img width="591" alt="Screen Shot 2022-10-09 at 9 24 46 PM" src="https://user-images.githubusercontent.com/107937930/194791534-a4d5f125-68da-410a-a0dd-ad4d4ef4d2a4.png">


<img width="465" alt="svm_tuned" src="https://user-images.githubusercontent.com/107937930/194792850-bee1620f-530f-4e1b-9c62-cd288d9a9188.png">



# Questions 

Q: What impact resulted from increasing or decreasing either or both of the SMA windows?

A: Increasing the SMA short_window to 60 shows that the Actual returns were accurate until mid 2017

and gets more inaccurate through time.


---

# Evaluate a New Machine Learning Classifier



<img width="594" alt="logistic_plot" src="https://user-images.githubusercontent.com/107937930/194790368-2cab146c-960e-4eb2-a94a-f5d9001367ca.png">


<img width="440" alt="logistic_model" src="https://user-images.githubusercontent.com/107937930/194790319-955eccda-451d-4007-9675-597553a8d487.png">


# Questions

Q: Did this new model perform better or worse than the provided baseline model? 
Q: Did this new model perform better or worse than your tuned trading algorithm?

A: The original baseline model performed better than the logistic model and the tuned model. The original model had a better a better accuracy (.96) to the logistic model (.66) and the tuned algorithm (.82).




