# Assignment 6 Part 2 - Writeup

---

## Question 1: Feature Importance

Based on your house price model, rank the four features from most important to least important. Explain how you determined this ranking.

**YOUR ANSWER:**
1. Most Important: Squarefeet
2. Bedrooms
3. Bathrooms
4. Least Important: Age 

**Explanation:**
What I did was look at the cooefficients of each feature to determine their importance. Since bedrooms and bathrooms were in the thousands, they were ranked higher than the absolute value of age ( which was around 900). Although squarefeet is the smallest cooeficient, since there is thousands of square feet in a house, that number scales up higher than the other factors. This info also matched up with the graph, where squarefeet seems the eaisest for a line of best fit and age was much more difficult to find a line of best fit.



---

## Question 2: Interpreting Coefficients

Choose TWO features from your model and explain what their coefficients mean in plain English. For example: "Each additional bedroom increases the price by $___"

**Feature 1:**
Each additional squarefoot the house had, price increases by $121.11

**Feature 2:**
Each additional bathroom the house had, price increases by $3,858.90

---

## Question 3: Model Performance

What was your model's R² score? What does this tell you about how well your model predicts house prices? Is there room for improvement?

**YOUR ANSWER:**

The model's R^2 score was 0.9936 meaning that the model was able to explain 99.36% of the variation of data, which for imperfect situations that occur in real life, is a pretty good score. Although this already seems good enough, we could always add more variables so that it can take those into account for a more accurate price.


---

## Question 4: Adding Features

If you could add TWO more features to improve your house price predictions, what would they be and why?

**Feature 1:**
Location 

**Why it would help:**
Although this may be hard to implement because houses are almost anywhere on earth, I feel like where the house is located is a big deciding factor for how much people would be willing to pay for it. For example, downtown areas are much more expensive than rural areas.

**Feature 2:**
Drive way / Garages

**Why it would help:**
It's another common house feature that can be implemented as one of the variables. This one would probably have a small range since I believe the average amount of garages is around 1. Eiter way, this would most likely have a decent impact on pricing

---

## Question 5: Model Trust

Would you trust this model to predict the price of a house with 6 bedrooms, 4 bathrooms, 3000 sq ft, and 5 years old? Why or why not? (Hint: Think about the range of your training data)

**YOUR ANSWER:**
Although the R^2 score was really high for predicting house prices, every variable except age is outside of the training data. This means that there's a chance that a house with features like these are priced differently than the ones in our dataset, so we would have to update our dataset in order to create a trustworthy model.

