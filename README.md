# R-Attitudes-about-Science-and-Faith-Project
 This project explores whether knowledge about science and age are associated with attitudes towards science and faith. To examine these relationships, we will use a subset of data from the 2005 Eurobarometer 63.1 survey.  In this project we try to model this relationship with a linear regression and create confidence intervals using bootstrapping.

### Data
This project uses three variables from the Eurobarometer 63.1 survey:
##### Features
+ `Science Score`: Score on a science quiz composed of 13 true/false items.
+ `age`: Age measured in years.
##### Target
+ `Attitude`: Attitude to science and faith (question wording: “We rely too much on science and not enough on faith”; responses on a 5-point scale from strongly disagree to strongly agree).

### Results

##### **Bootstrap Results**
The bootstrap confidence intervals table also reports that the 95% confidence intervals for both slope estimates do not include 0. This leads us to reject both null hypotheses at the 5% significance level, and conclude that there appear to be relationships for both age and science knowledge with attitude to science and faith.

##### **Intercept**
The results in the table report an estimate of the intercept as equal to approximately 2.79.  The independent variable science knowledge has only a handful of respondents that score zero, and no one is aged zero, so the constant by itself does not tell us much.

##### **Science knowledge slope**
The estimated value for the slope coefficient linking knowledge to attitude is estimated to be approximately -0.08. This represents the average marginal effect of knowledge on attitude. Every increase in quiz score by one point is associated with a decrease in attitude score of about -0.08, adjusted for age.

##### **Age slope**
The slope coefficient linking age to attitude is estimated to be approximately 0.002. This represents the average marginal effect of each additional year on attitude. That means that for every year older a person is, their attitude score is expected to increase by 0.002, controlling for science knowledge. This may seem like a very small effect, but remember that this is the effect of only one additional year.

