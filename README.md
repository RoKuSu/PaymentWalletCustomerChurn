# PaymentWalletCustomerChurn
Customer Churn Prediction & Customer Segmentation for a payment wallet (column names: changed)

I have used a csv file but you can connect to your DB as well using your favourite client. Code will be somewhat similar to this,

import pandas as pd
import your_DB_client
cursor = your_DB_client.connect(host='ip_address',port='8000',user='root',password='password',db='your_db')
df = pd.read_sql("Select * from your_table",cursor)             # if using SQL DB
df = pd.DataFrame(list(cursor['collection'].find(your_query))   # if using NoSQL DB
