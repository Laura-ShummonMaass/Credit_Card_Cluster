## Data Science Project 3 - Credit Card Customer Classification
**Created by:** Andy Luc and Laura E. Shummon Maass  
**Student Pace:** Full-Time Data Science  
**Scheduled project review date/time:** 05/31/2019  
**Instructors:** Miles Erickson & Greg Damico  
**Slide Deck Presentation**

### Business Case:
Determine appropriate customers to market loans to. Find the main customer segments and target the customers we feel would be most interested and eligible for credit approvals. 


### Data Set:   
We used a dataset continaing 6 months worth of credit card data. The data contained 17 feature columns and 9,000 rows which corresponded to customer ID.


### Process:   
We started off with K-Means Clustering to locate the primary customer groups. The silhouette graph recommonded we use 5 unique clusters. Since we had 8 features to cluster on we needed to use principle component analysis (PCA) to collapse the features into 2 dimensions. This gave us a clear visual to the 5 groups. 

In order to see the differences between the features of each group we needed to make a radar plot for each group. This was how we were able to define the groups into the various labels:
* Inactive
* Irresponsible
* Only Loans
And our target groups:
* Responsible
* Wealthy

### Additional Modeling:
We wanted to run both a logistic and k nearest neighbors model on a target classification feature column called Credit Approval. This column was a 1 if the customer:
* Had a credit limit over 3,000
* Had a balance over 1,000
* Had cash advances below 100

The F1 results we recieved with the logistic regression model were around 0.60 mark while the k nearest neighbors F1 score was almost 0.85. 

### Final Recommendation:
We will target customers that fall into the "Responsible" group with main stream credit card marketing options.
We will target customers that fall into the "Wealthy" group with our premium credit card marketing options.
We will use k nearest neighbors to determine individual qualification.


