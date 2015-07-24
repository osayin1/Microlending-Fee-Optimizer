# Microlending-Fee-Optimizer

This repository contains an IPython Notebook I created for my Insight Data Science (www.insightdatascience.com) project that I completed in three weeks. I worked with an online microlending nonprofit during this period, and the specific goal of the project was to help the nonprofit choose a fee they call the "loan loss reserve fee" to be used in the new business model they have recently adopted. Basically, instead of paying interest, first-time borrowers will pay this one-time fee that goes to a reserve fund which is used for compensating lenders for default losses. 

Predictive modeling of losses from loans was performed with a Random Forest model that used pre-disbursement features as well as features that reflected the current repayment behavior. Validation was carried out on an independent test set which yielded a predicted-R<sup>2</sup> of 0.70. Though the performance is not perfect, it is reasonably robust for the purpose of this project as what ultimately matters is the aggregate loss (per country) which is used in computing the proposed fee. To this end, total predicted loss deviated by only 2.3% from the actual on the validation set. 

The slides that describe the project in more detail can be found at: http://www.slideboom.com/presentations/1274240/Ozan-Sayin---Insight-Data-Science-Project

The source of the data is a proprietary MySQL database; hence the queries I wrote to manipulate tables and to create new ones I am unable to share. The front end (intended for the company itself) I created that proposes a fee for each country based on the state of the active loans can be found at: http://www.zidishafeeoptimizer.com/ 





