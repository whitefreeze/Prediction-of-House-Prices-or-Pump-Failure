# Pump It Up: Pump Failure Prediction

> Predict the operating condition of a waterpoint/pump for each record in the dataset.

The Ministry of Water in Tanzania is responsible for keeping rural water supply infrastructure operational on behalf of the rural areas and villages. There are thousands of water points / wells and it is a logistical challenge to maintain a list of up-to-date information on the status of the wells across the vast distances with reporting issues and varying levels of connectivity. 

The goal of this study is to more accurately anticipate when a well or pump will need servicing and categorize the pump status into one of the following categories:

* Functional
* Functional, but in need of repairs
* Nonfunctional

The source of this data is from a dataset on Kaggle, but the original source linked to was on Driven Data. There was also a related paper that I came across discussing how Tanzania has been working to modernize its water point / well status reporting system. 

[Pump It Up Challenge : Driven Data on Kaggle](https://www.kaggle.com/datasets/sumeetsawant/pump-it-up-challenge-driven-data)

[Pump it Up: Data Mining the Water Table on Driven Data](https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/page/25/)

[Monitoring Rural Water Points in Tanzania with Mobile Phones: The Evolution of the SEMA App](https://www.mdpi.com/2220-9964/6/10/316)

The dataset has 59,400 observations and 40 features.

Each observation is a separate water point or well. 

The features have information about almost every aspect of the well possible, except maintenance information. The features describe:

* Water point funding organization
* Water point installation entity & year built
* Water point operating entity
* Water point location information
* Water point type & water source
* Water quality information

## Visualization #1: "Population Using Pump"

### Visualization

![Screenshot 2023-06-18 at 8 08 01 PM](https://github.com/whitefreeze/Pump-It-up-Pump-Failure-Prediction/assets/13343127/012f5d2c-0982-47f5-9181-0da3c7a4f6fe)

### Explanation 

This graph shows the population around each water point/water pump. As this chart is scaled logarithmically for the number of pumps, it can be seen that for populations over four or five thousand, there are only a handful of pumps in those denser population areas. On the other hand, hundreds, thousands, and even tens of thousands of pumps are located in very small towns and villages, perhaps even where there are no people living, but only small herds of local livestock passing through. 

## Visualization #2: "Water Supply Sufficiency"

### Visualization

![Screenshot 2023-06-18 at 8 30 16 PM](https://github.com/whitefreeze/Pump-It-up-Pump-Failure-Prediction/assets/13343127/902bae02-0345-4f75-a361-54af79189283)

### Explanation

This graph shows that most of the water points have enough water, but around half of that number are insufficient. Of the water points with insufficient supply, around two thirds of that number are either dry or seasonal. All together, almost half of the water supply levels are either not able to meet water demand levels or are simply not able to be used, at all. 

Water is an incredibly necessary resource and when almost half of the wells are unable to supply the water needed, people suffer. This can be even more starkly felt in rural areas where water cannot be easily imported or distributed. 

## Visualization #3: "Plotting Latitude vs Longitude"

### Visualization

![Screenshot 2023-06-18 at 8 33 26 PM](https://github.com/whitefreeze/Pump-It-up-Pump-Failure-Prediction/assets/13343127/a65ff8f3-fe4f-41fc-bc59-72cefea290ac)

### Explanation

By plotting the latitude and longitude for each water pump in the country, we can see what resembles an outline of Tanzania (or a head...)! From this visualization we can see that there are pumps all over the country, and probably not just in the cities. This makes checking on each pump regularly, to see if it requires maintenance or not, a very difficult task. This would probably be a difficult undertaking for even the most advanced countries. People need access to good, clean water for their families, animals, gardens and farms. Achieving the goal of being able to predict maintenance needs proactively will help reduce the amount of time people will be without access to this life-giving resource.



