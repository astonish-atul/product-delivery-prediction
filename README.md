## E-Commerce Supply Chain: Predictive Delivery Analytics
### Objective: 
Developed a predictive framework to forecast shipment delays, enabling an international e-commerce company to optimize logistics and improve customer satisfaction.
## 1. The Challenge: Logistics Bottlenecks
Late deliveries are the primary cause of customer churn in e-commerce.<br/>
**The Problem**: Identifying which shipments are at risk of delay before they leave the warehouse.<br/>
**The Goal**: Build a model that categorizes shipments into "On-Time" or "Delayed" using raw logistics data (Weight, Cost, Shipment Mode, and Customer Behavior).<br/>
## 2. Findings
Instead of just using raw data, I engineered features to uncover hidden patterns:<br/>
**Discount Impact**: Found a correlation where products with >10% discounts were prioritized and delivered more reliably.<br/>
**Customer Interaction**: Discovered that the number of Customer Care Calls is a leading indicator of shipment distress.<br/>
**Warehouse Analysis**: Identified that Warehouse F handles the highest volume, acting as a critical node in the supply chain.<br/>
**Weight Matters**: The analysis showed that weight matters—products between 1kg-2kg and 4kg-6kg are statistically more likely to be delayed.<br/>
<img height=500 width=600 src="https://raw.githubusercontent.com/astonish-atul/product-delivery-prediction/refs/heads/main/img/download%20(4).png"><br/>
<img height=500 width=600 src="https://raw.githubusercontent.com/astonish-atul/product-delivery-prediction/refs/heads/main/img/download%20(1).png"><br/>
<img height=300 width=250 src="https://raw.githubusercontent.com/astonish-atul/product-delivery-prediction/refs/heads/main/img/Screenshot%202026-01-11%20171854.png"><br/>
## 3. Workflow
**Model Selection**: Evaluated multiple classifiers including Decision Tree Classifier, Logistic Regression, Random Forest, and KNN.<br/>
**Hyperparameter Tuning**: Utilized GridSearchCV to fine-tune the Decision Tree Classifier, which emerged as the top performer.<br/>
**The Pipeline**: Implemented a clean preprocessing flow involving Label Encoding for categorical blocks (Shipment Mode, Warehouse) and Scaling for numerical costs using minmaxscaler.<br/>
## 4. Key Takeaways
<img height=600 width=600 src="https://raw.githubusercontent.com/astonish-atul/product-delivery-prediction/refs/heads/main/img/download%20(3).png"><br/>
**Top Predictors**: Discount Offered , Weights, Customer Care Calls, Prior Purchases, and Product Cost.<br/>
**Business Value**: Moving from random shipping to priority-based logistics, potentially saving thousands in customer compensation costs.<br/>
## 5. Model Evaluation
<img height=600 width=600 src="https://raw.githubusercontent.com/astonish-atul/product-delivery-prediction/refs/heads/main/img/download%20(2).png"><br/>
