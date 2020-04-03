#### *Repo to track learning after a course in Cost and Economics from University of Virginia*

# Step by step economics for pricing optimization

## STEP 1: Calculating Regressions

Regressions are fundamental in pricing optimizations. At the core of a regression calculation is the statistical relationship between two variables. In this case, we can use regression to calculate the relationship between price and quantity of a product. Having established a relationship with the regression analysis of past data (past sales quantities at specific prices), we are at a position to make a forecast about the next likely values for both price & quantity based on the trend uncovered by the analysis. 

1. Firstly consider the following data. 

2. Now run a regression on StatPlus or Excel and generate the following scatter chart and coefficients from the report:

#### *Scatter chart indicating the statistical trend*

![regression](https://i.ibb.co/h8ZwGm4/regression-2020-04-03-21-22-17.png)

#### *Coefficients*

![coefficients](https://i.ibb.co/qMHP7bM/coefficients-2020-04-03-21-35-03.png)

3. Interpret the regression analysis

To further analysize the statistical linear relationship depicted on the scatter graph we need to start from the coefficients. The two coefficients (intercept and price) depict an estimate of the intercept of the line (to the y-axis) and the slope of the line. Extrapolating from them, they indicate an estimate forecast of *units sold*. We can write this fomula as follows: 

```
 Forecast of Units Sold = Some Intercept Value + Some Slope Value * Price
  
      or simply:
      
   ~u = a + b * P

```

The regression analysis has provided us with coefficients *a* and *b* (the intercept coefficent and the price coefficient). So we can the substitute the formala for these values and get the estimated volume of sales for any given price:

```
What's the estimated sales volume if we are selling at $0.99?

  ~u =  61.38 + (-15.5) * 0.99
  ~u =  44.84

```

4. Having done this, we can add to our data the price points of a competitor and check how sales volumes are affected against two variables: fluctuations in our price, as well as our competitors. 

![competitor pricing](https://i.ibb.co/KjCTQT3/competitor-prices.png)

5. Running a regression again with the additional competitor pricing, a report will be generated with an additional coefficient, this time linked to our competitors price:

![competitor's coefficient](https://i.ibb.co/q55ph3Q/competitor-coefficient.png)

6. We can now interpret the formula for estimating our sales volume based on both our competitor's pricing and ours as follows:

```
 Forecast of Units Sold = Some Intercept Value + (Some Slope Value * Our Price) + (Some Sloe Value * Competititor's Price)
  
      or simply:
      
   ~u = a + (b * P) + (c * CP)

```

Substituting for all coefficients:

```
What's our estimated sales volume if we are selling at $0.99 and our competitor at $1.99?

 ~u = 59.83 + (-17.03 * 0.99) + (2.04 * 1.99)
 ~u = 47.04
 
```

In other words if we consider only our own price, we can estimate that our sales volume will reach 45 units as described in step 5 above. However, if we also consider our competitor's pricing, our estimates change. If our competitor's price 1 dollar higher than us, are sales will grow even further reach 47 units. The results of the regression analysis are expected since with contextualising on the elasticity of our demand, we can safely assume that as our competitor's price rises, our sales will increase. 

