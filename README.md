# Student Performance Dataset analysis using Python 

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


![image](https://user-images.githubusercontent.com/23220212/178697034-7deaeddd-bd7c-4454-8dbc-1492c46a1e75.png)

*Figure: Comparison of total students on school as per gender*

**From the above comparison figure, we can clearly state that the total
number of students in GP and MS schools have a huge difference which can
make a bias decision while performing further analysis.**

![image](https://user-images.githubusercontent.com/23220212/178695740-00509b04-0f7e-4322-9946-7c1275795be0.png)

*Figure: Students according to gender in dataset*

**The number of female students is greater than male students in both
schools which can be considered normal as its ratio is considerable for
further analysis.**

### Data Preparation 

Student dataset is stored in a csv file with different
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

*Figure: Heatmap displaying correlation between different variables.*

## 4\. Data Exploration and Visualization 

### 4.1 Code to show histogram and box plots of different variables 

![image](https://user-images.githubusercontent.com/23220212/178696088-af8cc896-3e7a-4114-9c63-25b191a8e052.png)

> *Figure: Histogram to display students age variables*

In this histogram we are displaying total number of students with their
age variables starting from 15 to 22. We are creating bins according to
the range defined from minimum age value to maximum age values. Majority
of the students are of age 15 to 19 while maximum age is 16 to 17 and
very few students are of age 20 to 22.

![image](https://user-images.githubusercontent.com/23220212/178696190-05ad22de-07a9-49fa-888c-fa60c54c3d96.png)

> *Figure: Histogram to display student absences in days.*

In this histogram we are plotting to display number of students and
their absences in days. It has minimum values ranging from 0 to maximum
value 75 absences which is used to create bins range. Majority of the
students have few absences up to 5 days while some have absences ranging
from 5 days to 25 days.

![image](https://user-images.githubusercontent.com/23220212/178697787-79ef0ec6-da40-45dc-8a9d-9f32eb1fde06.png)

> *Figure: Histogram to display students grades of G3*

In this histogram we are displaying total number of students with their
final grades G3 which represents the Result of students either passed or
not. Large number of students have grades ranging from 8 to 16 which
concludes many students are passed. Almost 35 to 38 students have lowest
level of grades i.e. 0 to 1.

![image](https://user-images.githubusercontent.com/23220212/178697867-b115092e-3623-4740-b6d9-bcc8dcdc9597.png)

*Figure: Displaying boxplots for age*

From above box plot we can describe the lower age is 15 while the higher
age is 22. For median, upper quartile and lower quartile we can observe
that 17, 18 and 16 respectively.

![image](https://user-images.githubusercontent.com/23220212/178698032-62bbda4f-d37b-4729-87e6-e324d472abc8.png)

*Figure: Displaying boxplot for absences*

In this box plot above, the absence for lower quartile is 0, upper
quartile is 10, median ranges from 0 to 10 and maximum is 70 above.

![image](https://user-images.githubusercontent.com/23220212/178698268-3aea56ca-abbe-4a0e-978f-d29ee98aeade.png)

*Figure: Display boxplots of G3*

From above box plot we can describe the minimum and maximum value of
grade is 0 and 20 respectively while the ranges for upper quartile,
lower quartile, median are 12.5 to 15, 7.5 to 10 and 10 to 12.5.

### 4.2 Code to display bar graph of passed students. 

![image](https://user-images.githubusercontent.com/23220212/178698413-6aecbb61-6137-419b-81d2-7afb496b42b1.png)

> *Figure: Bar graph of passed students school wise.*

In this bar graph we are displaying total number of passed students
based on schools. By observing the chart, we can say large number of
students are passed of GP school while very few students are passed from
MS school. According to the dataset we also know that there is huge
difference in students’ data available of both schools.

### 4.3 Code to show students failed in final term. 

![image](https://user-images.githubusercontent.com/23220212/178698520-cba6e203-4fb6-41a8-97c5-6c6e5d29b99f.png)

> *Figure: Bar graph of students failed according to weekly study
> time*

In this bar graph we are displaying total number of failed students with
their weekly studying time based on final grades result i.e., G3. By
observing the chart, we can say large number of students are fail whose
weekly study time is less than 2 hour and up to 5 hours while few
students are getting fail if they study 5 to more than 10 hours weekly.

## 5.Further Analysis 

![image](https://user-images.githubusercontent.com/23220212/178705857-eaa2c318-25a2-49c3-82d7-eba64d4b385d.png)

*Figure: Pie chart to show student’s parent cohabitation status*

In the above pie chart, the pink color represents Parents cohabitation
status as Together while green color as Apart. It shows that almost 90 %
of student parents are living together while Remaining 10 % students’
parents are living apart from each other. This cohabitation status of
parents might have effect on student daily life which we will be
findings further analysis in the report.

![image](https://user-images.githubusercontent.com/23220212/178705698-d905ed65-e87e-492a-a981-1c95ecb09c8d.png)

*Figure: Pie chart of student's address*

In the above pie chart, the dark red color represents Student address in
Rural area while dark yellow color as Urban area. It shows that almost
78 % of student are living in urban area while Remaining 22% student are
living in rural areas.

![image](https://user-images.githubusercontent.com/23220212/178705631-a0e51f8b-2ecd-4486-ae5c-e74cff17b8c1.png)

*Figure: Pie chart of student's grouped by schools*

In the above pie chart, the pink color represents total number of
students in MS school while green color represents total number of
students in GP school. It shows that almost 88 % of the students are in
GP school while remaining 12 % are from MS school. This shows that there
is huge difference in data of school of GP and MS.

![image](https://user-images.githubusercontent.com/23220212/178705481-8650e168-22fa-49b5-aa95-5ff37e46a8a5.png)

*Figure: Total number of Students result as per gender.*

The above bar graph represents number of students passed or fail on G3
i.e., Final Grade grouped by sex. This graph clearly shows that total
number of male students passed, and female students passed are almost
equal while for failed students there is slight difference in which male
are comparatively less in number than female students. The total number
of students according to gender was 47 % male and 53 % female which can
be considered for analysis.

![image](https://user-images.githubusercontent.com/23220212/178705396-fc16edb9-bfb7-42c1-84ea-fa3f6a802be3.png)

> *Figure: Number of Students weekly study time with respect to
> failures according to gender .*

The above graph represents that number of male students who study less
than two hours tends to fail more in number than female students. While
a greater number of female students are getting failures even after they
study for 10 hours weekly. We can conclude that male is not able to
study for good number of hours every week while female are not able to
focus on their study time.

![image](https://user-images.githubusercontent.com/23220212/178705146-7b1e8b86-6423-4a98-8e9d-6c4a21457c79.png)

*Figure: Number of students and their father occupation according to
Result.*

The above graph represents the total number of students and their
father’s occupation with respect to Result of G3 i.e., Passed or not.
Many students father job is categorized in other and services in which
many of them are passed. and fathers’ job in health, at home or as a
teacher have low number of failed students. Also, we can also conclude
that passing percentage is higher in services and other job.

![image](https://user-images.githubusercontent.com/23220212/178705048-c85767e7-d21a-46b9-8b4d-0a0cd22964f8.png)

> *Figure: Number of students and their mother occupation according
> to Result.*

The above graph represents the total number of students and their
mother’s occupation with respect to Result of G3 i.e., Passed or not.
Many students mother job is categorized in other and services in which
many of them are passed. and mother’s job in health, at home or as a
teacher have low number of failed students. Also, we can also conclude
that passing percentage is higher in services and other job.

![image](https://user-images.githubusercontent.com/23220212/178699395-ec8ac5b6-5cff-4396-9b0b-da3b68da14ba.png)

> *Figure: Students final grade result according to father and mother
> education.*

The above bar plots represent father and mother education details and
compares them with student’s final grades to check for result either
passed or not. The bar pot in each diagram describes that parent having
no education background have full passing percentage of their children’s
as they might give sufficient time for their children’s to look after
them and help optimize their time in studying. While parents having
primary education to secondary education have failed children in their
final as they cannot give time or either they might be doing jobs.

![image](https://user-images.githubusercontent.com/23220212/178699259-290f6118-643f-4f62-964a-4279e9b111e0.png)

*Figure:Number of students according to Mothers job and family
relationship.*

The above graph represents total number of student relationship with
family based on Mother Job. We can describe maximum students have very
good, excellent, and good relationship with family, while very few
students have bad relationship with their family members working in all
job sectors. Students mother job in other and services have larger
number of students with very good, excellent, and good relationship with
family.

![image](https://user-images.githubusercontent.com/23220212/178699137-f78f2b7d-6d23-4add-b3f6-b817dc55a026.png)

*Figure: Number of students according to father’s job and family
relationship.*

The above graph represents total number of student relationship with
family on basis of Father job. We can describe maximum students have
very good, excellent, and good relationship with family, while very few
students have bad relationship with their family members working in all
fields. Students father job in other and services have comparatively
large number of students with very good, good, and excellent
relationship with family.

![image](https://user-images.githubusercontent.com/23220212/178699053-6f76fc38-f812-4ed1-984c-99862b7900ae.png)

*Figure: Boxplot for analysis of Final grade of students compared to
internet.*

The above figure represents final grade of students with respect to the
internet connection at home. In the above box diagram, green color
represents students not having internet and yellow represents students
having internet. The box plot shows students having internet i.e.,
yellow plots perform well in their final grade as we can see upper
quartile, lower quartile and median all are significantly higher than
green plots. Also, student with internet have higher maximum value than
student with no internet.

![image](https://user-images.githubusercontent.com/23220212/178698945-456d7031-d97f-4d45-8e2d-51b70e14272a.png)

*Figure: Attendance of students comapring result with absences as per
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

![image](https://user-images.githubusercontent.com/23220212/178698872-687272a0-de2d-4db3-bfba-7ed70bf8cb4d.png)

*Figure: Swarm plot to sgow the ECA of students as genderwise*

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
