Task3 
<h2>Dask queries</h2>
<h4>
  1) COUNT function: It is used to count any specific column from given dataset. 
      ex: Count of Order id = COUNT(Orders[Order ID])
  2) COUNTROWS function: It is used to count rows in given dataset. 
      ex: Count of rows = COUNTROWS(Orders)
  3) SUM function: It calculate the sum. 
      ex: Sum of orders quantity = SUM(Orders[Quantity])
  4) DISTINCTCOUNT function: If is used to count unique rows in rows. 
      ex: Unique rows = DISTINCTCOUNT(Orders[Order ID])
  5) SUM and Minus: ex: a)Total Profit = SUM(Orders[Quantity]) - SUM(Orders[Discount]) * 9 
                        b)Sum of Sales minus Sum of Discount = SUM('Orders'[Sales]) - SUM('Orders'[Discount])
  6) DIVIDE function: It gives division od any two specific columns.  
    ex: Sum of Quantity divided by Sum of Sales = DIVIDE(SUM('Orders'[Quantity]), SUM('Orders'[Sales]))
  7) MAX function: It calculate maximum no. of orders purchase by which customers by quantity.
     ex: Sum of Quantity max per Customer Name = 
      MAXX(
	        KEEPFILTERS(VALUES('Orders'[Customer Name])),
	        CALCULATE(SUM('Orders'[Quantity]))
        )
  </h4>

  
![image](https://github.com/user-attachments/assets/3476c766-e9a4-44f0-a079-d60c717a69b5)
