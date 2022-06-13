# cryto-plaything
## Development Blog

I need a project to help me keep up my python data science skills and give me a reason to continue refining my workflow on Github. Creating a tool for analyzing cryptocurrency meets both requirements.

### Stage 1 Goal: Create a data cleaning script to quickly export cryptocurrency data into a useable format.

Crypto provides a wealth of numerical data with which I can experiment, if I can only get it in a useful format. While cryptocurrency histories are widely available in interactive graphs, they are usually only available in CSV format for a fee. I noticed that all the relevant data on Live Coin Watch was sent to my client locally in a single file rather than sent piecemeal when I moused over their interactive graph. I will leverage this knowledge to create a simple script that exports the trading information from the data files sent to my browser client to CSV.

Conclusion: Created a script capable of formatting data pulled from Live Coin Watch by using regular expressions to identify relevant strings. 

### Stage 2 Goal: Calculate rates of change utilizing arbitrary windows of time for each price data point in the lifetime of Bitcoin.

Now that I have easy access to Bitcoin’s price history, the math to derivate the rates of change for each data point should be trivial. Once I know the rates of change, I can start making predictions about whether the price of the coin will go up or down in the near future. Because I eventually want to feed this information into a regression model, I want to be able to fine-tune the windows used to calculate the rates of change. I will write a function in python that accepts csv data formatted by the previous step and a window size to calculate the rate of change for each data point.

In Progress
