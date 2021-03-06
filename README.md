# PROJECT NAME:

Logic Logistics Report

---

# PROJECT OBJECTIVES:

The stakeholders of a logistics company called logic logistics wishes to visualize it data asset and understand:

- the total number of cars in its collection
- the number of cars belonging to a particular type
- the minimum present price for each car belonging to a particular type
- the maximum present price for each car belonging to a particular type
- the total present price for cars belonging to a particular type
- the total present price for the total number of cars in the collection
- the minimum selling price for each car belonging to a particular type
- the maximum selling price for each car belonging to a particular type
- the total selling price for cars belonging to a particular type
- the total selling price for the total number of cars in the collection
- the most expensive car by present price
- the least expensive car by present price
- the most expensive car by selling price
- the least expensive car by selling price
- the mileage in kilometers covered by each car belonging to a particular type
- the profit/loss incurred overtime
- how the present price and selling price progressed overtime.

---

# DATA SOURCING:

The data asset is on-premise and stored as csv file.
The data was collected and loaded directly into Power Query for transformation using Microsoft Power BI.

---

# DATA TRANSFORMATION:

With the data set being denormalised, refactoring into dimensions and fact tables was imminent.
The permanent data representing the business entities was split into dimension tables named:
- Cars
- Seller Type

The continuous activity of the business was split into fact tables named:
- Sales
- Profit_and_Loss

In the Profit_and_Loss table,the DAX (Profit/Loss = 'Profit_and_Loss'[Selling Price] - 'Profit_and_loss'[Present Price]) was used to create a calculated column to determine the profit/loss.

Each column in each of the tables were validated to have the correct data type in order to ensure data accuracy.
Each table was formatted to avoid repeated(duplicate) values.

---

# FINDINGS AND RECOMMENDATIONS:



![logistics](https://user-images.githubusercontent.com/106287208/178383470-6bca05b4-e219-466c-84bf-564efeb8dab5.jpg)

From findings:

- The company has a total of 91K cars
- The company's total present price of the cars is over $967M
- The company's total selling price of the cars is over $906M
- It was then determined the company has been underperforming and incurred a loss of $65M dollars overtime.

Recommendation:

The selling price of the cars should be raised above the present price to bring about profit for the company.

