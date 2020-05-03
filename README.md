# ia_liquor_sales

- source: Google BigQuery Public Datasets (https://console.cloud.google.com/bigquery)
  - Table ID: `bigquery-public-data:iowa_liquor_sales.sales`
  - query:
  
&emsp;SELECT <br>
&emsp;&emsp;date, store_number, store_name, city, 'IA' as state, zip_code, <br>
&emsp;&emsp;item_number, category_name, vendor_name, item_description, <br>
&emsp;&emsp;pack, bottle_volume_ml, state_bottle_cost, state_bottle_retail,   <br>
&emsp;&emsp;bottles_sold, sale_dollars <br>
&emsp;FROM \`bigquery-public-data.iowa_liquor_sales.sales\` <br>
&emsp;WHERE date = '2012-01-31';
