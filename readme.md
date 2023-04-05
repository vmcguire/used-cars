# Project Readme

## Overview
In this project, we explored a dataset from Kaggle containing information on 426K used cars to understand what factors make a car more or less expensive. Our goal was to provide clear recommendations to our client, a used car dealership, as to what consumers value in a used car. To guide us through the project, we followed the CRISP-DM process.

## Data
We worked with a used cars dataset from Kaggle, which contained information on 426K used cars.

## Deliverables
After understanding, preparing, and modeling our data, we wrote up a basic report that details our primary findings. Our audience for this report is a group of used car dealers interested in fine-tuning their inventory. 

We have also included a table that ranks the features based on their importance in determining the price of a used car. The table is shown below:

| Feature                  | XGB Rank | RF Rank | Final Rank | Flipped | Flipped % | Cumulative % |
|--------------------------|---------|---------|------------|---------|-----------|--------------|
| cylinders_8 cylinders    | 2.0     | 1.0     | 3.0        | 205.0   | 1.874371  | 1.874371     |
| odometer                 | 1.0     | 2.0     | 3.0        | 205.0   | 1.874371  | 3.748743     |
| paint_color_silver       | 3.0     | 3.0     | 6.0        | 202.0   | 1.846942  | 5.595684     |
| year                     | 7.0     | 5.0     | 12.0       | 196.0   | 1.792082  | 7.387766     |
| type_pickup              | 6.0     | 8.0     | 14.0       | 194.0   | 1.773795  | 9.161562     |
| manufacturer_toyota      | 4.0     | 10.0    | 14.0       | 194.0   | 1.773795  | 10.935357    |
| fuel_diesel              | 5.0     | 13.0    | 18.0       | 190.0   | 1.737222  | 12.672579    |
| paint_color_grey         | 8.0     | 11.0    | 19.0       | 189.0   | 1.728079  | 14.400658    |
| condition_like new       | 10.0    | 9.0     | 19.0       | 189.0   | 1.728079  | 16.128737    |
| condition_good           | 12.0    | 7.0     | 19.0       | 189.0   | 1.728079  | 17.856816    |


The top 5 features that drive the price based on a combination of XGB and Random Forest are 8 cylinders, odometer, paint color silver, year, and type of vehicle is a pickup.

## Findings

Top 10 Features for Used Car

1. 8 Cylinder Vehicles - The amount of power a car has how drive the price of a car. Business knowledge would know a higher cylinder count is a more powerful car.
2. Odomoter - How much a car has been used ie. odomoter makes sense to drive price second most. More wear and tear means a car that might not have much life left and therefore less willingness for people to invest money into with a higher percieved probability of the car dying.
3. Silver Paint Color - Interesting that silver paint color drives the price but this was fairly consistent between all the models, including the Linear Regression and Ridge models that we discarded. 
4. Year - Makes sense that year is next. I like that odomoter is more of a factor than the year of the car. If someone is concerned about wear and tear, the amount it has been driven would be much more indicative than the year. However an older car has older technology and may just not be up to par. 
5. Pickup Type - Pickup type is interesting. There is an added utility for this type of car, and that market for this may not necessarily care about comfort, but if the vehicle can help with labor. 
6. Toyota - Interesting that people value toyota alot, but their reputation precedes themselves as one of the best used cars due to their reliability. This is well known in the industry.
7. Disel Fuel - Fuel diesel makes sense because diesel engines are just more expensive new. 
8. Grey Paint Color - Paint color grey, which is close to silver also makes sense. 
9. Condition Like-New - Clearly higher than just good.
10. Condition good - Impactful

Taking a step back and looking at these factors, it easy to see that a truck with power drives the price of used vehicles. Essentially, a used vehicle that has utility over luxury, or comfort items is most important. This may speak to the customer persona of used vehicles. They may be more blue collar and using the vehicle for work. Whereas someone that wants comfort and that "new car" feeling is going to purchase a new car instead. It also appears there is a strong driver for a person to desire reliability when buying a used car.
