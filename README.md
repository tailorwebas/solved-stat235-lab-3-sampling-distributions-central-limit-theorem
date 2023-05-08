Download Link: https://assignmentchef.com/product/solved-stat235-lab-3-sampling-distributions-central-limit-theorem
<br>
In this lab assignment, you will explore important properties of sampling distributions in the context of a quality control process and computer simulation. In particular, you will use the <em>Random Number Generation</em> tool to demonstrate the validity of the Central Limit Theorem. You will also have an opportunity to review some features of the Poisson distribution.

As in the previous lab assignment, you will be given a choice to use either the built-in statistical functions in Excel for normal and Poisson distributions or the instructional templates (interactive worksheets) that are included in the associated data file. The Excel functions for Poisson and normal distributions were discussed in the <em>Lab 2 Instructions</em>.

<h1>Flaws in Plastic Panels</h1>

A company makes plastic panels used in automobiles. In order  to minimize the  number of defective panels, a strict quality control process is being used in the company. Random samples of panels in the manufacturing process are taken every hour and the data provided by quality control inspectors is instantly analyzed against the target parameters. A quality inspector inspects panels to check for any slight flaws. The number of these flaws in a panel is often modelled by a Poisson distribution with a parameter . We will use Excel to simulate the outcomes of the quality control process.

The workbook <em>lab3.xls</em> available at http://www.stat.ualberta.ca/statslabs/index.htm (click <em>Stat 235</em> link, and <em>Data </em>for<em> Lab 3</em>) contains the templates and the data to be used in the lab assignment. The workbook consists of three worksheets: <em>Poisson Probabilities</em>, <em>Normal Probabilities</em>, and <em>Simulation.</em>

The worksheet <em>Poisson Probabilities</em> enables you to calculate Poisson probabilities and cumulative Poisson probabilities. The worksheet <em>Normal Probabilities</em> allows you to calculate normal probabilities provided the distribution parameters are entered. In order to eliminate the possibility of mistakenly deleting charts and formulas in the worksheets, some cells and interactive charts are protected and, therefore, read-only.

<ol>

 <li>Open the worksheet <em>Poisson Probabilities</em>. The worksheet contains a graph of the Poisson probability distribution function. The top of the worksheet contains the value of . Any change to the distribution parameter is immediately reflected in the probability distribution function. In this part, you will see how various choices of  affect the shape of the Poisson distribution.</li>

</ol>

Enter the value of  as 0.5, then 1, 2, 3, 4, 5, and finally 6. After each entry, carefully examine the shape of the corresponding density curve. You are not supposed to print the probability distribution functions.

Describe briefly the change in the appearance of the probability distribution function as  increases from 0.5 to 6. What does the increase mean to the panel manufacturing process?

<ol start="2">

 <li>In this question, you can use either the built-in Excel Poisson function or the worksheet <em>Poisson Probabilities</em>. Suppose that the number of flaws in a panel has a Poisson distribution with parameter</li>

</ol>

 = 0.5. This implies that the expected number of flaws per panel is 0.5. Answer the following questions:

<ul>

 <li>What is the probability that there are no flaws in a randomly selected panel? In other words, what is the percentage of panels in perfect condition?</li>

 <li>Panels with two or more flaws are considered defective and scrapped by the company. Use the template to determine the percentage of panels that need to be scrapped.</li>

 <li>What is the probability that a random sample of ten panels does not contain any defective panel (at most one flaw)?</li>

</ul>

<ol start="3">

 <li>In order to check on the manufacturing process, random samples of several panels are taken repeatedly. According to the Central Limit Theorem, if a random sample of size <em>n</em> is drawn from a population with mean  and variance <sup>2</sup>, the sample mean approximately follows a normal distribution with mean  and variance <sup>2</sup>/<em>n</em> if the sample size is sufficienly large.</li>

</ol>

Assume  = 0.5 and use either the Excel NORMDIST function or the worksheet <em>Normal Probabilities</em> to answer the following questions:

<ul>

 <li>Can we safely assume that the sampling distribution of the average number of flaws in a random sample of 10 panels follows approximately a normal distribution ? Why or why not? Assuming it does apply, what is the probability that the average number of flaws in a random sample of 10 panels does not exceed 0.30?</li>

 <li>Can we safely assume that the sampling distribution of the average number of flaws in a random sample of 30 panels follows approximately a normal distribution ? Why or why not? Assuming it does apply, what is the probability that the average number of flaws in a random sample of 30 panels does not exceed 0.30?</li>

</ul>

In Questions 4 and 5, you must use Excel in a Windows environment to obtain data (different data may be produced by the <em>Random Number Generator</em> in Excel on MAC OS). Excel 2010 or higher version should be used in this part (earlier versions may produce different sequence of random numbers for the same seed).

Now suppose that the quality inspector is going to take a random sample of several panels to estimate the average number of flaws. How likely will his estimate be close to the true value? Which estimate is more likely to be better: one based on a sample of 10 panels or one based on a sample of 30 panels? We will answer the above questions by simulation.

<ol start="4">

 <li>Open the worksheet <em>Simulation</em>. The worksheet allows you to simulate the outcomes of the quality control process for 60 random samples of panels. Use the <em>Random Number Generation</em> feature (Poisson, seed 1000) to generate 60 samples of size <em>n</em> = 10 from the Poisson distribution with the parameter  = 0.5. This corresponds to selecting 60 samples, each consisting of 10 panels from the production run. The data will be entered in the form of 60 columns, each consisting of 10 rows into the range B9:BI18. In other words, the range contains the outcome of quality testing for 600 panels.</li>

</ol>

Once the data are entered, the values of the variables AVERAGE and COUNT are automatically displayed in rows 40 and 42, respectively.

<ul>

 <li>Use the COUNTIF function to determine the percentage of perfect panels (no flaws) among the 600 panels. Compare the value with the probability obtained in part (a) of Question 2. Should the values be identical? Explain briefly. The COUNTIF function was discussed in the <em>Lab 2 Instructions</em>.</li>

 <li>The variable COUNT in row 42 counts the number of defective panels in each sample. Use the values to determine the percentage of samples of ten panels containing no defective panels (at most one flaw)? Compare the value with the probability obtained in part (c) of Question 2. Should the values be identical?</li>

 <li>The variable AVERAGE in row 40 shows the average number of flaws for each sample. Obtain and print a histogram of the average number of flaws using the following bins: 0.0, 0.1, …, 1.2. The format of your histogram should be the same as the format of the sample histogram in the <em>Lab 1 Instructions</em> (labels, title, no gaps between bars). Describe the shape of the histogram.</li>

 <li>The worksheet <em>Simulation</em> also displays <em>Summary Statistics</em> for the variable AVERAGE. Use the feature to obtain the mean and standard deviation of the average number of flaws for the 60 samples. Compare them with the values predicted by theory. Should the values be identical? Explain briefly.</li>

</ul>

<ol start="5">

 <li>Now we repeat parts (c) and (d) of Question 4 with <em>n</em> = 30. First, clear the range B9:BI18 in the worksheet <em>Simulation</em>. Use the <em>Random Number Generation</em> feature (Poisson, seed 2000) to generate 60 samples of size <em>n</em> = 30 from the Poisson distribution with the parameter  = 0.5. The data will be entered into the range B9:BI38 in the form of 60 columns, each consisting of 30 rows.</li>

</ol>

<ul>

 <li>Obtain and print a histogram of the average number of flaws using the following bins: 0.3, 0.4, …, 0.8. Describe the shape of the histogram, comparing to the histogram obtained in part (c) of Question 4.</li>

 <li>Obtain the mean and standard deviation of the average number of flaws for the 60 samples. Compare them with the values predicted by theory and relate to the similar comparison in part (d) of Question 4. What do you conclude? State your findings briefly.</li>

</ul>