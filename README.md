# Statistics-101


### Descriptive versus inferential statistics

Descriptive statistics is the branch of statistics aiming at describing and summarizing a set of data in the best possible manner, that is, by reducing it down to a few meaningful key measures and visualizations—with as little loss of information as possible. In other words, the branch of descriptive statistics helps to have a better understanding and a clear picture about a set of observations thanks to summary statistics and graphics. With descriptive statistics, there is no uncertainty because we describe only the group of observations that we decided to work on and no attempt is made to generalize the observed characteristics to another or to a larger group of observations.

Inferential statistics, one the other hand, is the branch of statistics that uses a random sample of data taken from a population to make inferences, i.e., to draw conclusions about the population of interest. In other words, information from the sample is used to make generalizations about the parameter of interest in the population.

The two most important tools used in the domain of inferential statistics are:

* hypothesis test , and
* confidence interval 

### Motivation and Reason

I have realized that many students (especially in introductory statistic classes) struggle to perform hypothesis tests and interpret the results. It seems to me that these students often encounter difficulties mainly because hypothesis testing is rather unclear and abstract to them. One of the reason it looks abstract to them is because they do not understand the final goal of hypothesis testing—the “why” behind this tool. They often do inferential statistics without understanding the reasoning behind it, as if they were following a cooking recipe which does not require any thinking. However, as soon as they understand the principle underlying hypothesis testing, it is much easier for them to apply the concepts.

For this reason, I though it would be useful to write an article on the goal of hypothesis tests (the “why?”), in which context they should be used (the “when?”), how they work (the “how?”) and how to interpret the results (the “so what?”). Like anything else in statistics, it becomes much easier to apply a concept in practice when we understand what we are testing or what we are trying to demonstrate beforehand.

In this article, I present—as comprehensibly as possible—the different steps required to perform and conclude a hypothesis test by hand. These steps are illustrated with a basic example. This will build the theoretical foundations of hypothesis testing, which will in turn be of great help for the understanding of most statistical tests.

Hypothesis tests come in many forms and can be used for many parameters or research questions. The steps I present in this article are not applicable to all hypothesis test, unfortunately. They are however, appropriate for at least the most common hypothesis tests—the tests on:

* One mean: μ
* Two means:
* independent samples: μ1 and μ2
* paired samples: μD
* One proportion: p
* Two proportions: p1 and p2
* One variance: σ2
* Two variances: σ21 and σ22

The good news is that the principles behind these 6 statistical tests (and many more) are exactly the same. So if you understand the intuition and the process for one of them, all others pretty much follow.

### Hypothesis test . Why?

Unlike descriptive statistics where we only describe the data at hand, hypothesis tests use a subset of observations, referred as a sample, to draw conclusions about a population.

One may wonder why we would try to “guess” or make inference about a parameter of a population based on a sample, instead of simply collecting data for the entire population, compute statistics we are interested in and take decisions based upon that. The main reason we actually use a sample instead of the entire population is because, most of the time, collecting data on the entire population is practically impossible, too complex, too expensive, it would take too long, or a combination of any of these

In practice, we take some measurements of the variable of interest—representing the sample(s)—and we check whether our measurements are likely or not given our assumption (our belief). Based on the probability of observing the sample(s) we have, we decide whether we can trust our belief or not.

When?
Hypothesis tests have many practical applications. Here are different situations illustrating when the 6 tests mentioned above would be appropriate:

One mean: suppose that a health professional would like to test whether the mean weight of Belgian adults is different than 80 kg (176.4 lbs).
Two means:
Independent samples: suppose that a physiotherapist would like to test the effectiveness of a new treatment by measuring the mean response time (in seconds) for patients in a control group and patients in a treatment group, where patients in the two groups are different.
Paired samples: suppose that a physiotherapist would like to test the effectiveness of a new treatment by measuring the mean response time (in seconds) before and after a treatment, where patients are measured twice—before and after treatment, so patients are the same in the 2 samples.
One proportion: suppose that a political pundit would like to test whether the proportion of citizens who are going to vote for a specific candidate is smaller than 30%.
Two proportions: suppose that a doctor would like to test whether the proportion of smokers is different between professional and amateur athletes.
One variance: suppose that an engineer would like to test whether a voltmeter has a lower variability than what is imposed by the safety standards.
Two variances: suppose that, in a factory, two production lines work independently from each other. The financial manager would like to test whether the costs of the weekly maintenance of these two machines have the same variance. Note that a test on two variances is also often performed to verify the assumption of equal variances, which is required for several other statistical tests, such as the Student’s t-test for instance.
Of course, this is a non-exhaustive list of potential applications and many research questions can be answered thanks to a hypothesis test.

One important point to remember is that in hypothesis testing we are always interested in the population and not in the sample. The sample is used for the aim of drawing conclusions about the population, so we always test in terms of the population.

Usually, hypothesis tests are used to answer research questions in confirmatory analyses. Confirmatory analyses refer to statistical analyses where hypotheses—deducted from theory—are defined beforehand (preferably before data collection). In this approach, the researcher has a specific idea about the variables under consideration and she is trying to see if her idea, specified as hypotheses, is supported by data.

On the other hand, hypothesis tests are rarely used in exploratory analyses.2 Exploratory analyses aims to uncover possible relationships between the variables under investigation. In this approach, the researcher does not have any clear theory-driven assumptions or ideas in mind before data collection. This is the reason exploratory analyses are sometimes referred as hypothesis-generating analyses—they are used to create some hypotheses, which in turn may be tested via confirmatory analyses at a later stage.
