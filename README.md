# AMZN_Forecasting
This Python script is pulling data out of a Rapid API's for yahoo finniance, if you are wanting to run this script you will need to get our own API key. The data come's in JOSN formate which is then convereted into a Pandas Dataframa. 
The data is of Amazon stock price over the last 5 year's and is the close on a weekly freequence.
There are statisical test to see if there seasonilty and trend to the stock price, since the data show's that there is seasinalty in the stock price I decided to go with
as sariama model. The stock data come back as Homoskedastic, so I didn't enforce stationiar into the stock data. 
When doing the hyperprameter tunning, i was running into memory problem's, so to fix that any time that running a certain configuration come with a warning, that an exception would be hit, and that particular instance would be hit into the garbage collector. This serioulsy improved the efficanicy of the model. 
