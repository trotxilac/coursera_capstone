# Coursera Applied Data Science Capstone


## SpaceX Falcon 9 first stage landing prediction

The rocket Falcon 9, developed by SpaceX, is the first orbital class rocket capable of reflight. It is composed by two-stage and the capability of reflight means it is possible to reuse their first-stage in safety. Because of this possibility of reuse of expensive parts of the rocket, the cost of a launch is diminished. The goal of this capstone is to predict if the Falcon 9 first stage will land successfully. The possibility to determine if the first stage will land implies in the possibility to determine of the cost of a launch, in such a way that an alternate company could use this information to compete with SpaceX to launch a rocket and “win the space race”.

The goal of this capstone is to predict if the Falcon 9 first stage will land successfully. SpaceX advertises Falcon 9 rocket launches on its website, with a cost of 62 million dollars; other providers cost upward of 165 million dollars each, much of the savings is because SpaceX can reuse the first stage. Therefore if we can determine if the first stage will land, we can determine the cost of a launch. This information can be used if an alternate company wants to bid against SpaceX for a rocket launch.

### Exploratory Data Analysis (EDA)

The launch data from SpaceX REST API is gathered performing a get request using the requests library and web scraping Wiki pages related with Falcon 9 launch data using Python BeautifulSoup package. The data is converted into a dataframe and then some data wrangling is performed.

### Interactive Visual Analytics and Dashboard

A dashboard is build to analyze launch records interactively with Plotly Dash. Then an interactive map is built to analyze the launch site proximity with Folium.

### Predictive Analysis (Classification)

Using machine learning the success of the first stage of Falcon 9 landing is determined. The data is split into training and test data, then four different models - Logistic Regression, Support Vector Machine, Decision Tree Classifier and K nearest Neighbors - are trained and the best hyperparameters are selected using GridSearchCV. The accuracy is calculated using score method and the Confusion Matrix is obtained for each model.
