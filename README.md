## Will the Customer Accept the Coupon?

### Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

### Description

Imagine driving through town and a coupon is delivered to your cell phone for a restaurant near where you are driving. Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?


### Data

This data is from the UCI Machine Learning Repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, and passenger, and then asks people whether they will accept the coupon if they are the driver. 
There are three possible answers people can choose from:

1. “Right away” 
2. “Later, before the coupon expires” 
3. “No, I do not want the coupon”

The first two responses are labeled as “Y = 1,” and the third is labeled as “Y = 0.” There are five different types of coupons: Less expensive restaurants (under $20), coffee houses, carryout and takeaway, bars, and more expensive restaurants ($20–$50).

### Data Description

The attributes of this data set include:

1. User attributes
- Gender: male, female
- Age: below 21, 21 to 25, 26 to 30, etc.
- Marital Status: single, married partner, unmarried partner, or widowed
- Number of children: 0, 1, or more than 1
- Education: high school, bachelors degree, associates degree, or graduate degree
- Occupation: architecture & engineering, business & financial, etc.
- Annual income: less than $12500, $12500 - $24999, $25000 - $37499, etc.
- Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
- Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
- Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
- Number of times that he/she eats at a restaurant with average expense less than $20 per person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
- Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8

2. Contextual attributes
- Driving destination: home, work, or no urgent destination
- Location of user, coupon and destination: we provide a map to show the geographical location of the user, destination, and the venue, and we mark the distance between each two places with time of driving. The user can see whether the venue is in the same direction as the destination.
- Weather: sunny, rainy, or snowy
- Temperature: 30F, 55F, or 80F
- Time: 10AM, 2PM, or 6PM
- Passenger: alone, partner, kid(s), or friend(s)

3.Coupon attributes
   - time before it expires: 2 hours or one day

### Summary of Findings

After analyzing dataset and reviewing charts:
- Around 56% of total customers accepted coupons.
- Around 4.5% of total customers may accept Bar coupons
- Around 4.5% of total customers may accept Restaurant(20-50) coupons
- Around 15% of total customers may accept Coffee House coupons
- Around 15.5% of total customers may accept Carry Out & Take away coupons
- Around 17.5% of total customers may accept Restaurant(<20) away coupons
- Customers who are single, alone, married partners or do not have urgent work could be the most potential customers to accepts coupon. There are few other categories that are available in actual charts.

### Project URL
- GIT: https://github.com/sugandhpurohit/BHMLAI_Module5_Practical
- Notebook: https://github.com/sugandhpurohit/BHMLAI_Module5_Practical/blob/main/CustomerCoupons.ipynb

### Next steps and recommendations:

- Car Column: Car column to know customer can download onstar app to get coupon is very important. Given data set has maximum null values in Car column. And that too data with Y == 1 is even smaller.
- Location Columns: Since car data is not enough, location data (0 or 1) could be customer that are just passengers in others car or other method of commute and reach to destination. Or who just have the coupon and plan to utilize later even if its far or in opposite direction.
- Coupon Value: Everybody likes savings/discounts. It would be great if dataset has coupon value so customer can decide manage trip route based on their preference. Example: if coupon value is $20 per person for a new opening of restaurant and serve buffet, customer would be willing to go for manageable trip distance.
