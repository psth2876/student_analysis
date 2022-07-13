# student_analysis

# Part 1: Analysis of Student Performance Dataset 

Data analytics refers to the process of extracting useful insights from
datasets to draw conclusions about the information they contain. It
provides valuable ideas from raw datasets and uncovers different
patterns for every field. Here, we are using Python programming language
to analyze various information and gain results from the processed data.
Datasets regarding student performance in secondary education of two
Portuguese schools namely Gabriel Pereira and Mourinho da Silveira has
been given. The main objective of the coursework is to prepare data for
further analysis and visualization study.

## 1\. Data Understanding 

The dataset included in this coursework is student.csv which contains
data of two Portuguese school’s student achievements in secondary
education. Schools mentioned are : Gabriel Pereira and Mousinho da
Silveira. Some other data attributes are provided which includes student
grades (in mathematics), demographic, social and school related
features.

<table>
<thead>
<tr class="header">
<th><blockquote>
<p>S.N.</p>
</blockquote></th>
<th>Attribute</th>
<th><blockquote>
<p>Description</p>
</blockquote></th>
<th>Attribute Type</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><blockquote>
<p>1</p>
</blockquote></td>
<td>School</td>
<td><blockquote>
<p>It has two categorical values (“GP” - Gabriel Pereira and “MS” - Mousinho da Silveira).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>2</p>
</blockquote></td>
<td>Sex</td>
<td><blockquote>
<p>It contains two categorical values (“M” as Male and “F” as Female).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>3</p>
</blockquote></td>
<td>Age</td>
<td><blockquote>
<p>It has multiple numerical integer values.</p>
</blockquote></td>
<td>discrete</td>
</tr>
<tr class="even">
<td><blockquote>
<p>4</p>
</blockquote></td>
<td>Address</td>
<td><blockquote>
<p>It represents student’s home address type and has two categorical values (“U” – urban or “R” – rural).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>5</p>
</blockquote></td>
<td>Famsize</td>
<td><blockquote>
<p>It represents family size of students and has two categorical values (“LE3” – less or equal to 3 or “GT3” – greater than 3).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>6</p>
</blockquote></td>
<td>Pstatus</td>
<td><blockquote>
<p>It represents parent’s cohabitation status and has two categorical values (“T” – living together or “A” – Apart).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>7</p>
</blockquote></td>
<td>Medu</td>
<td><blockquote>
<p>It represents mother’s education and contains multiple categorical values (“higher education”, ”primary education”, ”secondary school”, ”5<sup>th</sup> to 9<sup>th</sup> grade” , “none”).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>8</p>
</blockquote></td>
<td>Fedu</td>
<td><blockquote>
<p>It represents father’s education and contains multiple categorical values (“higher education”, ”primary education”, ”secondary school”, ”5<sup>th</sup> to 9<sup>th</sup> grade” , “none”).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>9</p>
</blockquote></td>
<td>Mjob</td>
<td><blockquote>
<p>It represents mother’s job and contains multiple categorical values (“at home”, ”health”, ”other”, ”services” , “teacher”).</p>
</blockquote></td>
<td>categorical</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr class="header">
<th><blockquote>
<p>10</p>
</blockquote></th>
<th>Fjob</th>
<th><blockquote>
<p>It represents father’s job and contains multiple categorical values (“at home”, ”health”, ”other”, ”services” , “teacher”).</p>
</blockquote></th>
<th>categorical</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><blockquote>
<p>11</p>
</blockquote></td>
<td>Reason</td>
<td><blockquote>
<p>It represents reason behind choosing the school and has multiple categorical values (“at home”, ”health”, ”other”, ”services” , “teacher”).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>12</p>
</blockquote></td>
<td>Guardian</td>
<td><blockquote>
<p>It represents who is responsible for student’s guardian and has multiple categorical values (“Father”, ”Mother”, ”Other”).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>13</p>
</blockquote></td>
<td>Traveltime</td>
<td><blockquote>
<p>It shows the travelling time for students from home to school and has multiple categorical values</p>
<p>(“15 to 30 min”, ”&lt;15 min”,” 30 min to 1 hour”, “&gt;1 hour”).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>14</p>
</blockquote></td>
<td>Studytime</td>
<td><blockquote>
<p>It shows the weekly study time for students and has multiple categorical values (“ 5 to 10 hours”, ” &lt;2 hours”,” &gt;10 hours”,” 2 to 5 hours”).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>15</p>
</blockquote></td>
<td>Failures</td>
<td><blockquote>
<p>It shows number of past class failures for students and has multiple numerical values (“0,1,2,3”).</p>
</blockquote></td>
<td>discrete</td>
</tr>
<tr class="even">
<td><blockquote>
<p>16</p>
</blockquote></td>
<td>Schoolsup</td>
<td><blockquote>
<p>It shows extra educational support of students and has multiple categorical values (“yes ”, “no”).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>17</p>
</blockquote></td>
<td>Famsup</td>
<td><blockquote>
<p>It refers to the family supported education provided to students. It has two variables “yes” or “no”.</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>18</p>
</blockquote></td>
<td>Paid</td>
<td><blockquote>
<p>It refers to details if student had paid for extra classes, the value is either “yes” or “no”.</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>19</p>
</blockquote></td>
<td>Activities</td>
<td><blockquote>
<p>It indicates if the student has extracurricular activities in school. The value is either “yes” or “no”.</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>20</p>
</blockquote></td>
<td>Nursery</td>
<td><blockquote>
<p>It represents if the students have attended nursery school or not. It has two variables either “yes” or “no”.</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>21</p>
</blockquote></td>
<td>Higher</td>
<td><blockquote>
<p>It represents if the students want to take higher education in the future or not. It has values either “yes” or “no”.</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>22</p>
</blockquote></td>
<td>Internet</td>
<td><blockquote>
<p>It represents either student have internet access at home. The value is “yes” or “no”.</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>23</p>
</blockquote></td>
<td>Romantic</td>
<td><blockquote>
<p>It has information about the student romantic relationship. The value available is “yes” or “no”.</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>24</p>
</blockquote></td>
<td>Famrel</td>
<td><blockquote>
<p>It has multiple categorical values ( “2 to 5 hours”, ”5 to 10 hours”, ”&lt;2 hours”, ”&gt;10 hours” ).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>25</p>
</blockquote></td>
<td>Freetime</td>
<td><blockquote>
<p>It has multiple categorical values ( “2 to 5 hours”, ”5 to 10 hours”, ”&lt;2 hours”, ”&gt;10 hours” ).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>26</p>
</blockquote></td>
<td>Goout</td>
<td><blockquote>
<p>It has multiple categorical values ( “low”,</p>
<p>”medium”, ”very low”, ”high”, ”very high” ).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>27</p>
</blockquote></td>
<td>Dalc</td>
<td><blockquote>
<p>It has multiple categorical values ( “low”,</p>
<p>”medium”, ”very low”, ”high”, ”very high” ).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>28</p>
</blockquote></td>
<td>Walc</td>
<td><blockquote>
<p>It has multiple categorical values ( “low”,</p>
<p>”medium”, ”very low”, ”high”, ”very high” ).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>29</p>
</blockquote></td>
<td>Health</td>
<td><blockquote>
<p>It has multiple categorical values ( “good”,</p>
<p>”excellent”, ”very bad”, ”bad”, ”very good” ).</p>
</blockquote></td>
<td>categorical</td>
</tr>
<tr class="even">
<td><blockquote>
<p>30</p>
</blockquote></td>
<td>Absences</td>
<td><blockquote>
<p>It has numerical values ranging from (0 to 75) and represents number of school absences.</p>
</blockquote></td>
<td>discrete</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>31</p>
</blockquote></td>
<td>G1</td>
<td><blockquote>
<p>It represents first period grades which has numerical values ranging from (0 to 20).</p>
</blockquote></td>
<td>discrete</td>
</tr>
<tr class="even">
<td><blockquote>
<p>32</p>
</blockquote></td>
<td>G2</td>
<td><blockquote>
<p>It represents second period grades which has numerical values ranging from (0 to 20).</p>
</blockquote></td>
<td>discrete</td>
</tr>
<tr class="odd">
<td><blockquote>
<p>33</p>
</blockquote></td>
<td>G3</td>
<td><blockquote>
<p>It has numerical values ranging from (0 to 20) and represents final grade.</p>
</blockquote></td>
<td>discrete</td>
</tr>
</tbody>
</table>

![image](https://user-images.githubusercontent.com/23220212/178695454-87d504c1-9165-42de-8fa6-e75d38aa1757.png)

**From the above comparison figure, we can clearly state that the total
number of students in GP and MS schools have a huge difference which can
make a bias decision while performing further analysis.**

![image](https://user-images.githubusercontent.com/23220212/178695740-00509b04-0f7e-4322-9946-7c1275795be0.png)

*Figure 2: Students according to gender in dataset*

**The number of female students is greater than male students in both
schools which can be considered normal as its ratio is considerable for
further analysis.**

### Data Preparation 

For part 1, Student dataset is stored in a csv file with different
attributes. Python has many libraries so we can use some of them for
data preparation. Pandas is an inbuilt library which is used to read csv
file as required and load int into a data frame. Further we can use more
libraries such as matplotlib, seaborn and NumPy.

### Libraries 

### Pandas 

Pandas is an open source and most popular library which is used mostly
for data analysis/science and machine learning jobs. It provides high
performance, easy to use data structures and data analysis tools for the
python programming language and is built on top of NumPy. It has
functions for analyzing, cleaning, exploring, manipulating data and
allows users to analyze big data which further make conclusions based on
statistical theories. (ActiveState, 2020)

### NumPy 

It is an open-source library in python, which consists of powerful data
structure i.e., multidimensional array objects and process those arrays.
We can perform mathematical, scientific, statistical, and logical
operations on arrays by using NumPy. Its main aim is to work with
Ndimensional array, linear algebra, random number etc. It is fast,
memory efficient and very convenient to work with matrix multiplication.
(Palo, 2021)

### Matplotlib 

Matplotlib is a cross-platform, open-source data visualization and
graphical plotting library available in python. It is a cross-platform
library for making 2D plots from data in arrays. It provides an
object-oriented API which helps in embedding plots in applications using
Python GUI toolkits. It can be used in Python and IPython shells,
Jupyter notebook and web application servers. It can represent data in
different format of visualization reports such as histogram, maps, bar
plots, pie charts, scatter plots etc. (Thetechwriters, 2021)

### Seaborn 

Seaborn is an open-source library used for visualization of statistical
graphics plotting in Python. It provides beautiful styles and color
palettes to make statistical plots more attractive and easier to
understand. It is built on the top of matplotlib library and is
integrated to the data structures from pandas. It provides
dataset-oriented APIs which allows us to switch between different visual
representations for same variables for better understanding of dataset.
(GeeksforGeeks, 2020)

### 3.2 Correlation between different variables using Heatmap 

![image](https://user-images.githubusercontent.com/23220212/178695975-6a2a510d-37ea-4299-a64f-b00a8ad74223.png)

*Figure 37: Heatmap displaying correlation between different variables.*

## 4\. Data Exploration and Visualization 

### 4.1 Code to show histogram and box plots of different variables 

![image](https://user-images.githubusercontent.com/23220212/178696088-af8cc896-3e7a-4114-9c63-25b191a8e052.png)

> *Figure 38: Histogram to display students age variables*

In this histogram we are displaying total number of students with their
age variables starting from 15 to 22. We are creating bins according to
the range defined from minimum age value to maximum age values. Majority
of the students are of age 15 to 19 while maximum age is 16 to 17 and
very few students are of age 20 to 22.

![image](https://user-images.githubusercontent.com/23220212/178696190-05ad22de-07a9-49fa-888c-fa60c54c3d96.png)

> *Figure 39: Histogram to display student absences in days.*

In this histogram we are plotting to display number of students and
their absences in days. It has minimum values ranging from 0 to maximum
value 75 absences which is used to create bins range. Majority of the
students have few absences up to 5 days while some have absences ranging
from 5 days to 25 days.

![Chart, histogram Description automatically
generated](media/image6.jpg)

> *Figure 40: Histogram to display students grades of G3*

In this histogram we are displaying total number of students with their
final grades G3 which represents the Result of students either passed or
not. Large number of students have grades ranging from 8 to 16 which
concludes many students are passed. Almost 35 to 38 students have lowest
level of grades i.e. 0 to 1.

![Chart, box and whisker chart Description automatically
generated](media/image7.jpg)

*Figure 41: Displaying boxplots for age*

From above box plot we can describe the lower age is 15 while the higher
age is 22. For median, upper quartile and lower quartile we can observe
that 17, 18 and 16 respectively.

![Chart, box and whisker chart Description automatically
generated](media/image8.jpg)

*Figure 42: Displaying boxplot for absences*

In this box plot above, the absence for lower quartile is 0, upper
quartile is 10, median ranges from 0 to 10 and maximum is 70 above.

![Chart, histogram Description automatically
generated](media/image9.jpg)

*Figure 43: Display boxplots of G3*

From above box plot we can describe the minimum and maximum value of
grade is 0 and 20 respectively while the ranges for upper quartile,
lower quartile, median are 12.5 to 15, 7.5 to 10 and 10 to 12.5.

### 4.2 Code to display bar graph of passed students. 

![Chart Description automatically generated](media/image10.jpg)

> *Figure 44: Bar graph of passed students school wise.*

In this bar graph we are displaying total number of passed students
based on schools. By observing the chart, we can say large number of
students are passed of GP school while very few students are passed from
MS school. According to the dataset we also know that there is huge
difference in students’ data available of both schools.

### 4.3 Code to show students failed in final term. 

![Chart Description automatically generated](media/image11.jpg)

> *Figure 45: Bar graph of students failed according to weekly study
> time*

In this bar graph we are displaying total number of failed students with
their weekly studying time based on final grades result i.e., G3. By
observing the chart, we can say large number of students are fail whose
weekly study time is less than 2 hour and up to 5 hours while few
students are getting fail if they study 5 to more than 10 hours weekly.

## 5.Further Analysis 

![Chart, pie chart Description automatically
generated](media/image12.jpg)

*Figure 46: Pie chart to show student’s parent cohabitation status*

In the above pie chart, the pink color represents Parents cohabitation
status as Together while green color as Apart. It shows that almost 90 %
of student parents are living together while Remaining 10 % students’
parents are living apart from each other. This cohabitation status of
parents might have effect on student daily life which we will be
findings further analysis in the report.

![Chart, pie chart Description automatically
generated](media/image13.jpg)

*Figure 47: Pie chart of student's address*

In the above pie chart, the dark red color represents Student address in
Rural area while dark yellow color as Urban area. It shows that almost
78 % of student are living in urban area while Remaining 22% student are
living in rural areas.

![Chart, pie chart Description automatically
generated](media/image14.jpg)

In the above pie chart, the pink color represents total number of
students in MS school while green color represents total number of
students in GP school. It shows that almost 88 % of the students are in
GP school while remaining 12 % are from MS school. This shows that there
is huge difference in data of school of GP and MS.

![Chart, bar chart Description automatically
generated](media/image15.jpg)

*Figure 48: Total number of Students result as per gender.*

The above bar graph represents number of students passed or fail on G3
i.e., Final Grade grouped by sex. This graph clearly shows that total
number of male students passed, and female students passed are almost
equal while for failed students there is slight difference in which male
are comparatively less in number than female students. The total number
of students according to gender was 47 % male and 53 % female which can
be considered for analysis.

![Chart, bar chart Description automatically
generated](media/image16.jpg)

> *Figure 49: Number of Students weekly study time with respect to
> failures according to gender .*

The above graph represents that number of male students who study less
than two hours tends to fail more in number than female students. While
a greater number of female students are getting failures even after they
study for 10 hours weekly. We can conclude that male is not able to
study for good number of hours every week while female are not able to
focus on their study time.

![Chart, bar chart Description automatically
generated](media/image17.jpg)

*Figure 50: Number of students and their father occupation according to
Result.*

The above graph represents the total number of students and their
father’s occupation with respect to Result of G3 i.e., Passed or not.
Many students father job is categorized in other and services in which
many of them are passed. and fathers’ job in health, at home or as a
teacher have low number of failed students. Also, we can also conclude
that passing percentage is higher in services and other job.

![Chart, bar chart Description automatically
generated](media/image18.jpg)

> *Figure 51: Number of students and their mother occupation according
> to Result.*

The above graph represents the total number of students and their
mother’s occupation with respect to Result of G3 i.e., Passed or not.
Many students mother job is categorized in other and services in which
many of them are passed. and mother’s job in health, at home or as a
teacher have low number of failed students. Also, we can also conclude
that passing percentage is higher in services and other job.

![Chart, bar chart Description automatically
generated](media/image19.jpg)

> *Figure 52: Students final grade result according to father and mother
> education.*

The above bar plots represent father and mother education details and
compares them with student’s final grades to check for result either
passed or not. The bar pot in each diagram describes that parent having
no education background have full passing percentage of their children’s
as they might give sufficient time for their children’s to look after
them and help optimize their time in studying. While parents having
primary education to secondary education have failed children in their
final as they cannot give time or either they might be doing jobs.

![Chart, bar chart Description automatically
generated](media/image20.jpg)

*Figure 53:Number of students according to Mothers job and family
relationship.*

The above graph represents total number of student relationship with
family based on Mother Job. We can describe maximum students have very
good, excellent, and good relationship with family, while very few
students have bad relationship with their family members working in all
job sectors. Students mother job in other and services have larger
number of students with very good, excellent, and good relationship with
family.

![Chart Description automatically generated](media/image21.jpg)

*Figure 54: Number of students according to father’s job and family
relationship.*

The above graph represents total number of student relationship with
family on basis of Father job. We can describe maximum students have
very good, excellent, and good relationship with family, while very few
students have bad relationship with their family members working in all
fields. Students father job in other and services have comparatively
large number of students with very good, good, and excellent
relationship with family.

![Chart, box and whisker chart Description automatically
generated](media/image22.jpg)

*Figure 55: Boxplot for analysis of Final grade of students compared to
internet.*

The above figure represents final grade of students with respect to the
internet connection at home. In the above box diagram, green color
represents students not having internet and yellow represents students
having internet. The box plot shows students having internet i.e.,
yellow plots perform well in their final grade as we can see upper
quartile, lower quartile and median all are significantly higher than
green plots. Also, student with internet have higher maximum value than
student with no internet.

![Chart Description automatically generated](media/image23.jpg)

*Figure 56: Attendance of students comapring result with absences as per
gender in violin plot*

In the above Violin plot, blue color refers to the rate of passed
student with their absence rate as per sex whereas red color refers to
the rate of failed student with their absence rate as per sex. The white
dot in above plot is the median value. The violin plot represents that
maximum number of value points is present in between 0 to 20. Also,
there is wide range of absence values in the female group while male
student has less absence as compared which shows higher number of males
have passed the exam. From above we can conclude that both male and
female students having high absence days are also able to get good
grades in exam.

![A picture containing table Description automatically
generated](media/image24.jpg)

*Figure 57: Swarm plot to sgow the ECA of students as genderwise*

In the swarm plot above, the blue filled circle represents the failed
students and the pink filled circle represents the students who
graduated. The graph on the left represents the students resulting in
final grade according to their gender who do not participate in
extracurricular activities while the graph on the right represents the
students resulting in final grade as per their gender who participate in
extracurricular activities. Male students tend to participate more in
extracurricular activities than female students according to the graph
above. The failure rate in the final grade of male students
participating in extracurricular activities is also lower than that of
the female students participating in extracurricular activities. The
graph above reflects that, in their final grade, women who do not engage
in any extracurricular activities have high pass rate.
