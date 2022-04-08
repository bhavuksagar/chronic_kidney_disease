# chronic_kidney_disease
<h3>Challenges in Dataset:</h3>
<ul>
<li>Dataset has many missing values.</li>
<li>Datatype of the columns also incorrect</li>
<li>All missing values are assigned with “?” and “ ?” which is in string format.</li>
<li>Some data are stored with spacing in front of the starting letter. ex: “ yes” &
“yes”.</li>
<li>Outliers in the dataset</li>
</ul>
<br>
<h3>Data Preprocessing And EDA</h3>
<li>All the missing values are in “?” string format so we replace all the “?” values with nan.</li>
<li>Datatype of all the columns is in object/string format so we change the datatype of numeric value columns into the float for calculation.</li>
<li>Map the categorical feature into 1 and 0 format for model input.</li>
<li>Fill the missing values with mode/median and mode according to the box plot</li>
and distribution graph plot.</li>
<li>Check the correlation of columns with the target column and found that our
features have both positive and negative correlation with our target value which
is a good for training.</li>
<li>In fig 1 it shows that some of the features contain a high number of outliers. So
we filled those columns missing values with the median.</li>
<li>In fig 2 it shows that a few columns are creating bell curves and equally</li>
distributed but most of them are following left skewed and right skewed patterns.
<li>Fig 3 contains the correlation values of the features. It shows how the features
are correlated with each other and we found that features are correlated with the target columns but not so much correlated with each other which is good for the model.</li>
<br>
<img src="imgs/box_plot.png ">
<img src="imgs/dis_plot.png ">
<img src="imgs/heat_map.png ">
<h3>Model Building</h3>
<ul>
<li>We use different algos for building the model like:- random forest, extra tree, LogisticRegression etc.</li>
<li>We got 99% accuracy with Random forest and Extra tree algo.</li>
<li>We divide the dataset into 75% training and 25% test.</li>
</ul>