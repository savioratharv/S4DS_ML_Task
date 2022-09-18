# S4DS_ML_Task
Created by Atharv Patawar (SAP ID: 60009210176)
<li>
The first scatterplot comparing manufacturers and average review rating doesn't tell us a lot mainly because there are way too many manufacturers on the X axis. But it does tell us roughly the price distribution. This was the first graph I plotted and certainly not something a business owner or a consumer can use for any meaningful inferences.
</li>

<li>
The second scatterplot is a bit more civilized in nature in that it successfully tells us the relation between the price and rating. It may also be useful in certain cases for a manufacture to know their general rating but not very feasible for that purpose since seaborn groups multiple manufacturers. One thing we can infer from this plot is that price and rating are not related but higher priced products generally don't have a bad rating and some of the lower priced products do have bad ratings.
</li>
<li>
The third graph is miles ahead of the previous two in terms of aesthetics and readibility. Its a bar graph showing the average price and rating of categories and sub categories. It may prove useful for a manufacturer getting into the market to decide what price will fetch a paticular product the most ratings in its respective category so its quite a useful graph. But the categories and sub categories are quite long and finding what you are looking for in there may be a tedious task. I think we can do a bit better in this department.
</li>
<li>
The next graph may look familiar as it compares the price and rating like the second graph but without the maunfacturers. The main motive behind plotting this graph was to check if a ML model can be used to predict price and all I could infer from it sadly is that it cannot as there is no definite realtionship. And there are way too many manufacturers or sub categories to one hot encode.
</li>
  
<li>
After finding the specific and super categories of a product by using the simple good old string functions, the data started to make more sense and new possiblities started to come to mind. The first plot after that is comparing the specific categories with the prices and rating using a Bar Graph. The inference here is quite similar to the third graph. But this time around its more readable. A manufacturer can now decide what price should the product be for getting the best rating according to the specific category the product belongs to.
</li>
  
<li>
The next bar graph, comparing the super/main categories with the price and rating, does what the previous did but for main categories. This is something not only manufacturers but also amazon can use to check how popular each category is and stocking warehouses depending on that. This inference is also shared by the previous two graphs of specific categories and category and sub category.
</li>
  
<li>
After creating a new column of popularity which is nothing but the number of reviews multiplied with the average rating, I proceeded to use my newly found knowledge about groupby and after many errors and searches on stackoverflow, I ended up with two beautiful bar graphs which compared the price and average review rating and popularity. The caveat here being it only covers the first few rows so inferences derived from it are quite limited. But one thing we can see is how vastly equally rated products vary in popularity mainly because of the difference in the number of reviews. This re-instates the importance of the populariy column and something consumers should pay attention to to gauge how good a product actually is. Many a times, people end up buying products which have a 5 star rating (but less number of reviews) because they thought its an outstanding product as it has 5 stars and then later on repent on their purchase as the product wasn't as good as the rating made it look like. Such consumers are in dire need of assistance in their buying decision and that's exactly where the tool I next developed comes into the picture.
</li>
<li>
Introducing the Product Recommender! This tool makes buying the right product easy, depending on what you are comfortable with, you either a related keyword or the specific category or the super category of the product you are looking for and voila! You are gifted with the product you should consider buying along with further recommendations related to that product that people buying that product also bought. This has been made possible by the use of simple lists and sorting a dictionary formed by combining two lists. The beauty of this tool lies in the fact that it converts seemingly simple python concepts to achieve something really helpful in everyday life.
</li>
<li>
Note: All bar graphs in this analysis skip the error lines in order to make the graphs more presentable and aesthetically pleasing.
</li>
