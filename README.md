## King-County-House-Sales

Group Members: Ali Mahzoon, and Stephen Enke

-----
### Business Problem
King county is considered as 11th largest county in Washington state (slightly larger than 21 million tennis courts). Finding houses in such a large county has always been a problem for people to find a house that is not over price. On the other hand people don't want to spend their money until they are sure they couldn't have found a better place geographically.

we are real-state investors, we can use this model to project prices and to see properties are over or under value.

---------
### Questions:
1. Is the house price change based on the location?
2. What is the average house price base on the city in this county?
3. What is the price of a house with specific features?
4. Can people get any recommendation based on their available money? (i.e. I have x money what I can buy)
5. Is it possible to predict a house price based on the house features (bedrooms, bathrooms,...)?


------
### Dataset and Approach
* Dataset and Tools:
   * Given data by King County House Sales
   * statsmodel and scikit learn library


* Approach:
   * Feature Engineering
   * Multicolinearity of features
   * Multiple linear regression
   * Model fit in linear regression by using Stepwise selection with p-values, finding interactions by cross validation
   * Regression model validation by calculating Root Mean Squared Error (RMSE)
   * Data visualized by Seaborn and Matplotlib


-----
### Findings
We divide the King County map into 4 prats (NW, NE, SW, SE) as we can see most of the high-price houses (houses more than 613,275$) are mostly located at North and a little tendency to East.

![Image](https://github.com/alimahzoon/King-County-House-Sales/blob/Ali-wip/Images/1.png "Expensive houses")


On the other hand as we go toward South West houses become less expensive (houses less than 317,000$) as we can see in the following image.

![Image](https://github.com/alimahzoon/King-County-House-Sales/blob/Ali-wip/Images/4.png " Less Expensive houses")


This categorization of data gives us a high level overview of price based on location. Our real-state concentration is on prices raging from 173,000$ to 907,000$ which makes our real-state unique because of helping people to find houses all over the King County with different prices. (it needs to be mentioned that there are houses that are more than 7 million dollar!).

---
Average prices in different cities (Descending)

![Image](https://github.com/alimahzoon/King-County-House-Sales/blob/Ali-wip/Images/4.png " Average Prices")

---
We have the information of 21,507 houses in the King county in Washington state, so if people want to know the price of a house in each city or even more accurate in each Zipcode, our real-state can find a similar house in that area and predict the price of the house.
The goodness of fit of our model ,R-Squared, after using stepwise selection with p-values and using interactions on our training set is 0.748.

In the following picture you can see the QQ-plot to keep track of residuals.

![Image](https://github.com/alimahzoon/King-County-House-Sales/blob/Ali-wip/Images/qq.png " QQ-plot")

---  
In statistics, a sequence of random variables is homoscedastic if all its random variables have the same finite variance. we can chceck the homoscedasticity assumption by using a regplot.

![Image](https://github.com/alimahzoon/King-County-House-Sales/blob/Ali-wip/Images/homo.png " homoscedasticity")

-----
### Conclusion
Houses located on North east are more expensive than houses located on south west. The most important feature of a house that has linear relationship with price of the house is the size of the house including having a basement, bedrooms, and bathrooms. Construction grade has a slightly linear relationship with price.

---
### Recommendations
If you are looking for a house in cities like Medina, Mercer Island, and Bellevue you probably end up having a house with the price more than 700,000$. However, if you are willing to buy a house in cities like Kent, Auburn, and Federal Way even by spending much less money (less than 300,000) you might even get a bigger house.  
