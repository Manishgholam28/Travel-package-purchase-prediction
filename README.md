
# Travel-package-purchase-prediction

In order to compute accurate predictions for travel package purchase in advance, we experiment with various statistical techniques and machine learning models to find an 
optimal approach for this problem.Tourism is one of the most rapidly growing global industries and tourism forecasting is becoming an increasingly important activity in planning and managing the industry. Because of high fluctuations of tourism demand, 
accurate predictions of purchase of travel packages are of high importance for tourism organizations. The goal is to predict whether the customer will purchase the travel or not


## Dataset Attributes

a)Customer details:

1)CustomerID: Unique customer ID

2)ProdTaken: Whether the customer has purchased a package or not (0: No, 1: Yes)

3)Age: Age of customer

4)TypeofContact: How customer was contacted (Company Invited or Self Inquiry)

5)CityTier: City tier depends on the development of a city, population, facilities, and living standards. The categories are ordered i.e. Tier 1 > Tier 2 > Tier 3

6)Occupation: Occupation of customer

7)Gender: Gender of customer

8)NumberOfPersonVisited: Total number of persons planning to take the trip with the customer

9)PreferredPropertyStar: Preferred hotel property rating by customer

10)MaritalStatus: Marital status of customer

11)NumberOfTrips: Average number of trips in a year by customer

12)Passport: The customer has a passport or not (0: No, 1: Yes)

13)OwnCar: Whether the customers own a car or not (0: No, 1: Yes)

14)NumberOfChildrenVisited: Total number of children with age less than 5 planning to take the trip with the customer

15)Designation: Designation of the customer in the current organization

16)MonthlyIncome: Gross monthly income of the customer

b)Customer interaction data:

1)PitchSatisfactionScore: Sales pitch satisfaction score

2)ProductPitched: Product pitched by the salesperson

3)NumberOfFollowups: Total number of follow-ups has been done by the salesperson after the sales pitch

4)DurationOfPitch: Duration of the pitch by a salesperson to the customer
## Building the Model

1)We will start with a Decision Tree model

2)Next, we will build two ensemble models - Bagging Classifier and Random Forest Classifier

3)Then, we will build three Boosting ensemble models - ADABoost, GradientBoost and XG Boost

4)We will first build them with their default parameters and later hypertune them for optimization.

5)We will also calculate all four metrics; Accuracy, Recall, Precision and F1Score which is the metric of interest

6)F1Score is the weighted average of Precision and Recall. Its takes both False positives and False negatives into account.


## Conclusion

 1)Hence Tuned Random Forest Classifier Model gives an overall generalised metric performace w.r.t F1 score and doesnt seem to be over-fitting.

2)The most importance features for this model are:

a)MonthlyIncome

b)Age

c)Passport_1(Customers with Passport)

d)Designation 

d)This model has an 71% accuracy rate, which is quite good despite the imbalance in data.
