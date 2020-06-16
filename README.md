# Exploratory_analysis_PISA_2012
Exploratory analysis of differences in mathematics performance of Canadian, American and French students

## by Camille de The


## Dataset

The Programme for International Student Assessment (PISA) is a worldwide study by the Organisation for Economic Co-operation and Development (OECD)
 intended to evaluate educational systems by measuring 15-year-old school pupils' scholastic performance on mathematics, science, and reading. 
The dataset comes from PISA 2012 survey, which is the programme’s 5th survey. Around 510 000 students answered questionnaires to provide information
 about their background, school and learning experiences. 

We decided to focus on students in Canada, France and in the US with information on mathematical attitudes such as mathematical 
anxiety and self-concept. We deleted all rows with missing values. 

The final dataset consists in 8995 observations organized at the student level. Each row describes the learning context and outcomes of one student. 
The original dataset had 635 columns, our dataset has now only 14 columns. 

The dataset could be found here: https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisa2012.csv.zip&sa=D&ust=1554482573645000
The technical documentation here: https://www.oecd.org/pisa/pisaproducts/pisa2012technicalreport.htm
The list of variables: https://www.google.com/url?q=https://s3.amazonaws.com/udacity-hosted-downloads/ud507/pisadict2012.csv&sa=D&ust=1554482573645000

## Summary of Findings

In my investigations i found that American, Canadian and French students differ in many respects. The median result for performance in mathematics 
is lower in the US compared to Canada and France. The time spent studying math appears to be significantly different from one country to another. 
Canada has the highest median around 5 hours per week, France has the lowest median around 4 hours per week. The median of the socio economic index 
is higher in Canada, 
then comes the one of the US and last France's.  

Then we identified the main features that vary with math performance: the socio economic index,the mathematical self-concept (positive correlation) 
and mathematical anxiety (negative correlation). 
The variables linked to quality of math teaching (class management, support from the teacher, cognitive activation) display also a positive correlation 
with mathematical performance, though these effects appear to be weaker.

Among those main features that seem to be linked to math performance, we have been able to note some important national discrepancies. 
Anxiety appears to be more widespread in France than in Canada and the US and mathematical self-concept is similarly higher in the two North American
 countries. As far as the teaching quality is concerned, it appears that France's median results are below the ones of the US and Canada. 

While the relationships between the socio economic status of parents and mathematical performance is positive in each country, 
the slope of this association is much steeper in the French context than in the US or in Canada. It may mean that the French school system is less 
efficient to overturn social discrepancies.

We have also been able to see in this dataset the uneven progression of students from one grade to another in the three different countries. 
The US and Canada display a rather flatter progression of their students' math performance from one grade to another compared to France. 

Anxiety and mathematic performance appear to be strongly negatively correlated. Despite strong national differences both in math performance and anxiety, 
we surprisingly found that the relationship between anxiety and math performance appears to be similar accross the three countries. 
French students appear to suffer on average more badly from mathematical anxiety than North American students despite performing better on average in 
mathematics. This shows the cultural and social component of mathematical anxiety. This needs to be investigated more in depth through statistical analysis.

 
## Key Insights for Presentation

For the presentation, i chose to focus on the relationships of 5 variables: mathematical performance of students, their country, the socio economic index 
and the two variables capturing student's attitudes toward mathematics: self-concept and anxiety. I started with the distributions of mathematical 
performance, in all the three countries together and in each of them. I rotated the violinplot for the three national distribution to keep the same 
orientation as the histogram plot for the whole dataset. I included a table with the summary statistics with an improved format for better readability. 
Then i presented the distributions of the socio economic indexes before and after the transformation operated. I introduced the matrix of correlation 
of all the initial variables used in the exploration analysis to justify my focus on only 5 variables. I changed the name and the order of the columns of 
my dataset to ensure a good understanding of all the variables. 
Then i dived into the relationships between mathematical self-concept / anxiety and math performance in a cross country perspective. I added some titles 
to the graphs and to the axis of the different graphs presented. 
Finally i presented my findings on the relationships between socio economic index and math performance. I presented first the strong correlation between 
thos two variables. I added a scatterplot with the initial socio economic variable as a way to visually confirm the relevance of the operated transformation.
I then presented the French singularity: the steeper slope of association between socio economic status and math performance. I polished the faceted graphs 
in displaying the names of each country as titles. 
