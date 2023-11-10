I've crafted a tool for the nonprofit foundation Alphabet Soup to assist in choosing funding applicants with the best chance of success in their endeavors. Using my expertise in machine learning and neural networks, I developed a binary classifier based on the provided dataset. Our target was a minimum accuracy of 75% for the model. Alphabet Soup's business team provided me with a CSV file containing information on over 34,000 organizations that have received funding. This dataset includes several columns capturing metadata about each organization, such as: 
●	EIN and NAME—Identification columns
●	APPLICATION_TYPE—Alphabet Soup application type
●	AFFILIATION—Affiliated sector of industry
●	CLASSIFICATION—Government organization classification
●	USE_CASE—Use case for funding
●	ORGANIZATION—Organization type
●	STATUS—Active status
●	INCOME_AMT—Income classification
●	SPECIAL_CONSIDERATIONS—Special considerations for application
●	ASK_AMT—Funding amount requested
●	IS_SUCCESSFUL—Was the money used effectively

What variable(s) are the target(s) for your model?
The target variable is the 'IS_SUCCESSFUL' column from application_df


What variable(s) are the features for your model?
The feature variables for the model are derived from the "application_df" dataframe by excluding the "IS_SUCCESSFUL" column, meaning that every other column in the dataframe is considered a feature variable.


What variable(s) should be removed from the input data because they are neither targets nor features?
Both 'EIN' and 'NAME' columns.


How many neurons, layers, and activation functions did you select for your neural network model, and why?
In the initial trial, I randomly selected 9 hidden nodes for the first layer and 6 hidden nodes for the second layer. These choices were arbitrary and intended for refinement in the subsequent attempt.


Were you able to achieve the target model performance?
I was not able to achieve the targeted 75%.


What steps did you take in your attempts to increase model performance?
I made several adjustments to my approach, such as adding layers, removing columns, introducing more hidden nodes, and changing activation functions for each layer. 

Summary
In summary, the deep learning model achieved approximately 72% accuracy in addressing the classification problem. Improving the correlation between input and output is key for enhancing prediction accuracy. This can be accomplished through thorough upfront data cleanup and experimenting with different activation functions in the model, iterating until a higher accuracy is attained.
