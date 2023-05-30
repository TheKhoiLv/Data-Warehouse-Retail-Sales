# Data Warehouse Retail Sales

## 1. Introduce
Building a sales data warehouse is an important activity for businesses today, especially in the analysis of sales data. Business data analytics plays an important role in improving warehouse management, chain stores, improving pricing decisions and marketing strategies. Using predictive analytics can help businesses reduce inventory management costs, increase shelf efficiency, focus resources on high-demand areas, and capture trends quickly. sales and optimize shipping.

### Dataset
- This is a descriptive dataset of sample sales data taken on www.kaggle.com including a lot of information about sales data, customer information, order information, revenue, delivery, etc.
- Link Dataset: https://www.kaggle.com/kyanyoga/sample-sales-data

## 2. Data Warehouse Design
### Introduce Dimention
- FactSales: Sales information
- DimTime: Time information of RetailSales dataset 
- DimProduct: Products information of RetailSales dataset
- DimCustomer: Customers information of RetailSales dataset
- DimSize: Size information of RetailSales dataset
- DimStatus: Status information of RetailSales dataset
- Diagram
![image](https://github.com/TheKhoiLv/Data-Warehouse-Retail-Sales/assets/134827421/e3f6b110-5638-4042-b2ea-9229b9c6f4e3)

## 3. Project
### 3.1 Building a data warehouse using the SSIS tool
-	Create a new packed named ExToSource.dtsx: Containing the original data
![image](https://github.com/TheKhoiLv/Data-Warehouse-Retail-Sales/assets/134827421/e63d304e-918d-467c-a0e8-2fb3593a92f3)
- Create a new packed named SourceToStage.dtsx: Select properties and dump original data to Stage tables
![image](https://github.com/TheKhoiLv/Data-Warehouse-Retail-Sales/assets/134827421/555b70d8-d95d-4d25-b6e9-90b1b64e7eea)
- Create a new package named StageToDW.dtsx: Data Warehouse
![image](https://github.com/TheKhoiLv/Data-Warehouse-Retail-Sales/assets/134827421/70efba9b-620b-4965-8a4d-40f5dd6bb0ec)
