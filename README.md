# Market-Basket-Analysis
![](images/market_basket.jpg)

## 1. Introduction
 - **Goal**: Identify products that are frequently bought together.
 - **Application**:
   - **Retail**: Determine product bundling strategies. For example, if bread and butter have a high positive correlation, stores can place these items near each other or offer bundle deals.
   - **E-commerce**: Enhance recommendation systems by suggesting items that are often purchased together.
  
## 2. Methodology
I used Python on Google Colabs to analyze this project. Steps such as loading data, making a pivot table, handling missing values ​​and calculating correlation between each item are all executed using Python code.
And here is the correlation matrix to analyze the relationship between each product:

![](images/correlation_matrix.png)

## 3. Analyzing the result and give actionable insights
Firstly, I will focus on those who have strong positive correlation. Specifically as follows:

**1) Bread and Butter**
- Correlation: 0.66
- Insight: There is a strong positive correlation between bread and butter, meaning that the customers are likely to buy both products together. Obviously, a toast cannot be complete without one of these two ingredients.

**2) Cheese and Jam**
- Correlation: 0.63
- Insight: Same as the first pair, there is also a strong positive relationship between cheese and jam. This a common pair of products.

**3) Eggs and Milk**
- Correlation: 0.39
- Insight: Another combo package, we can see these two ingredients appearing a lot in cooking and baking recipes.

=> **Actionable insights**
- Suggest discounted combo packages or bundle deals for these product pairs to increase sales. For instance:
  - When a customer purchases Bread, we can recommend them to buy Butter at a discount.
  - When a customer buys Cheese, we can suggest Jam as an additional item.
- For a supermarket or retail store, we can place these products close together to increase the likelihood of customer buying both.

Next, I will focus on the products that have strong negative correlation:

**1) Cheese & Milk and Jam & Milk**
- Correlation: - 0.44
- Insight: They have strong negative relationship, meaning that when customer buys Cheese or Jam, they are less likely to buy Milk. They may choose one of the two instead of buying both.
  
**2) Apple & Banana**
- Correlation: - 0.27
- Insight: They have a moderate negative correlation, meaning that customers are likely to buy just one fruit and not both.

=> **Actionable insights**
- For online shopping, we can suggest alternative product when a customer does not choose a certain product (e.g: "Not buying Cheese ? Try Milk at a discount !").
- For retail stores, we can place these products separately to reduce direct competition and increase the chance of selling both.
- If we still want to sell these combos, for example Apple & Banana, we may create combo promotions to encourage customers to purchase.

All detailed steps are done in this code link: [HERE](https://colab.research.google.com/drive/1I7C8or3W88WdFjfxCe7WZVQQMgclWfvF?usp=sharing)
