# Predicting European Soccer Transfer Prices
* In European Soccer, teams have the ability to make a cash offer to another team in order to acquire a player.
* It is a highly dynamic market
* It is the subject of much fanfare


### Notes about which Jupyter Notebooks are what:
* WebScrapping Includes webscrapping some statistics from wikipedia for goals and appearances, it is pretty messy.

* EDA and Modeling Notebook(main notebook to look at) has some graphs and all organized modeling, also has some building of additional features
* "Where I Scrubbed and joined Fifa Video Game Player Attributes...ipynb" is where I scrubbed and joined fifa video game player attributes
* I later merged these fifa video game attributes with the main transfer market price dataframe, and match statistics data frame in the main: "EDA and Modeling Notebook"

*Code in "EDA" at the bottom has pytrends(google trends api) attempt and that takes a while to run, the feathered dataframe there will show the results of bringing in this data, but as a I struggled to merge it well, I realized that the return number from the API was in relation to the player's own search volume history so, a 17 for Cristiano Ronaldo would not be the same as a 17 for Emille Heskey, so this number would not be helpful for the regression.

### Notes about feather files
* "DataFrameforEDAandRegression.feather" will be read in using feather library in EDA and Modeling Notebook"
* "fifa_df.feather" has fifa statistics, I join into the main dataframe with season stats and transfer price
* df_g_trends.feather has the results of the pytrends queries which I ended up not using due to reason mentioned above. 


### If any jupyter notebooks do not render in github you can always view them in https://nbviewer.jupyter.org/ if you copy and paste the github notebook link. 



