# family-library-dataset-analisys
Family Library Dataset Project for the Diploma in Data Analysis Using SPSS at Alison Learning

#### The project contains:
* >Dataset Folder .\dataset\
* >Results Folder .\results\

## Final - Case Study
Analyses and Results are presented, but you will need to reproduce the same Results and then interpret them.
The Audience is required to decide on the Type of Data for Appropriate Analysis.
For some Concepts, hints are also provided.

A Family Library contains 800 Books.
Suppose that the Owner is interested in exploring some Features of the Existing Books through a Short Survey.
Thirty Books have been Selected and THREE Characteristics have been measured.
That is, the Number of Pages (Page), Weight in Grams (Weight) and Type of each Book (Type) have been recorded.
The Full Dataset is provided.
  - >Project Folder .\dataset\Dataset-Family-Library.jpeg

### The following Specific Objectives have been identified:
 -   (i) Summary Statistics
 -  (ii) Exploratory Data Analysis
 - (iii) Establish the Relationship between Weight and Page Number.
>_Also, predict the Page Number for a Weight of 200 Grams._
 -  (iv) Is the Average Number of Pages per Book in the Library less than 100?
 -   (v) Is the Average Weight per Book Significantly Bifferent from 200 Grams?
 -  (vi) Are the Average Numbers of Pages different for Different Types of Books?

As done in the previous Lesson, we need to input the following Data from 30 Books Selected from a Library.
There are THREE variables, namely Paper, Weight, and Type.

##### GNU PSPP
  We could use a free option, GNU PSPP, instead of IBM SPSS
  (there are some differences between the two statistical applications).
 * [IBM SPSS](https://www.ibm.com/products/spss)
 * [GNU PSPP](https://www.gnu.org/software/pspp/)

  And finally, another free option, Wessa.net.
 * [Wessa.net](https://www.wessa.net/)

### Analyses
 * Different Analyses of SPSS Dataset

##### Data Entry
>For the Variable Type, we select:
 - 1 = “Religious”
 - 2 = “Story”
 - 3 = “Science”

##### Reports/Graphs
 * Main Statistics
 * Pie Chart
 * Histograms
 * Boxplots

##### Scatterplot of Weight versus Page
  Here we will consider Simple Linear Regression and Multiple Linear Regression Analysis.
  At first, we would like to fit a Regression Line of Weight on the Page.
  That is, we consider Weight as the Dependent Variable and Page as the Independent Variable.

  Skewness/Obliqueness
  Distribution of Weight: Symmetric, Positively Skewed, or Negatively Skewed
  _NOTE: Make it Symmetric through Log Transformation.
        Variable=lnWeight
		→ Transform → Compute Variable (lnWeight)_

  Now, we will fit the Regression Model of lnWeight on Page
    and then take the Exponent of the Predicted Value for getting Prediction in the actual Unit.

##### Residual Analysis
 * Final Fitted Mode,
   If we put Page = 200 in the above Equation, we obtain the Predicted Value of Weight.

##### Multiple Regression Analysis
  Now, consider Page and Type both to be Independent Variables.
  So the Results will be one the Report.

##### One-Tailed Test (T-Test)
  As the Distribution of Page is Symmetric, we can use a T-Test.
  If we will can test “Less than 100”; that is, it refers to a Left-Tailed Test...
    Output T-Statistic is Negative.
  _NOTE: The Output is for a Two-Tailed Test, but we need a One-Tailed Test.
  So, the Final P-Value will be HALF of the Value._

##### Non-Parametric Test
  As the Distribution of Weight is NOT Normal, Parametric T-Test is not feasible here.
  We need to use Non-Parametric Test.
  We want to test whether the Median Weight is Different from 200 Grams or NOT.
  _NOTE: Hypothesis Test Summary_

##### ANOVA / Multiple Comparisons
  We need to test the Equality of THREE Means.
