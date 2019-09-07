## Project Title - RetailProductPriceOptimization
The objective of  this case study is to optimize the price level of products for an online vendor. 

## Case Study

The owner of an online grocery store sells 250 products online. A conventional methodology has been applied to determine the price of 
each product. And, a simple methodology is applied – price the product at par with the market price of the product.

This case is to leverage analytics to determine pricing to maximize the revenue earned.

Out of 100000 people who visit the website, only 5000 end up purchasing the products. 
Now, all those who made a purchase, we have obtained their buying patterns, including their average unit purchased etc.

To understand the impact of price variations, we tried testing different price points for each product. The impact can be broken down into two aspects:

1. A lower price point increases the volume of the purchased product.
2. Customers compare price points of a few products more than others, to make a decision whether to buy products from your portal or not.

Now, we want to find the optimum price points for each of the product to maximize the total profit earned. In this case study, we are provided with a table with all 250 items

## Following are the variables available in the data set

Average Price/Unit : Market price of the product
Cost/Unit : Current cost of the product
Average Profit/Unit : Profit for each unit
Average units sold : Average number of units of product sold to a customer who makes a purchase
Incremental acquisition : For every 10% decline in unit price, this is the increase in total customer response rate. Note that overall response rate initially is 5% (5000 out of 100000 make a purchase). You are allowed to decrease the price of a product maximum by 10% by market laws.
Increase in sale volume : For every 10% decline in unit price of product, this is the increase in volume. Again, you are allowed to decrease the price of a product maximum by 10% by market laws.

## The attached R code uses the below methodology to determine Net Profit

1. We start with a vector of all zeros for each 250 products incremental sales price.
2. We now increase/decrease each of the product’s incremental sales price by 1% to see the impact on total profit.
3. For an increase in profit, we keep the incremental sales. Now we start with this vector to find further marginal increment.
