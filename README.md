# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis

### Problem Statement
According to an article published by Inside Higher Ed on May, 2021, ([*source*](https://www.insidehighered.com/quicktakes/2021/05/17/no-more-sat-or-act-u-california)), following a court ruling, the University of California system will not be considering SAT and ACT scores in admissions decisions. The university system will be able to review test scores if students choose to submit them, but they are not mandatory in the application process. 

Some of the institutions within the University of California system, including the University of California - Los Angeles, are among the top ranked public institutions in the U.S. News Best Colleges rankings, a rankings system of academic quality among four year colleges in the United States ([*source*](https://www.usnews.com/best-colleges/rankings/national-universities?schoolName=University+of+California+Los+Angeles)) making this change one that has the potential to set a precedent for future college admissions and scholarship decisions. 

According to Inside Higher Ed, the number of test optional institutions grew from 1,040 prior to the COVID-19 pandemic to around 1,700 for the Fall 2021 semester. This trend has been welcomed by some who believe that applicants from underserved communities do not have access to SAT and ACT preparation services, automatically setting them at a disadvantage when competing for admission and scholarships.

The President, Vice President and Provost, and Dean of Academic Affairs at Bright Future University (BFU) in Washington, DC, a small liberal-arts college, have commissioned a research study to evaluate their admissions decisions process and consider adopting the test optional model. Key inputs in this decision will be whether: 

* Nationally the SAT and ACT tests are still relevant among the U.S. population of college applicants as measured by participation rates over time.
* There is an association between SAT and key student outcomes including first-year retention rates and graduation rates and net revenues per full-time equivalent student
* Whether these associations also apply for students from lower socio-economic backgrounds, including those who receive Pell grants.

If the SAT assessment is not correlated with key outcome measures for the BFU's Administrators, there may be preliminary evidence to support that SAT's are not adequate predictors of student success and thus their role in the admissions process should be reconsidered.

This document will document the evidence for these research questions and will conclude with a set of recommendations for BFU.

### Analysis Plan:
To answer these research questions, SAT and ACT participation rates and average scores across all U.S. states from 2017-2019 will be analyzed and visualized to contextualize usage and performance nationally in these assessments. The institutional characteristics data from the College Scorecard will be used to:

* Summarize and visualize the relationship between SAT composite scores and graduation and first-year retention rates.
* Analyze the relationship between SAT and ACT composite scores and graduation and first-year retention rates for Pell-grant recipients or students who demonstrate a high level of financial need ([*source*](https://studentaid.gov/understand-aid/types/grants/pell)).
* Analyze the relationship between SAT and ACT composite scores and institutions' net tuition revenue per full-time equivalent student.

### Data Sources
|Data Set | Source |File name|Description|
|:---|:---|:---|:---|
|Average ACT scores by State (2017) | College Board |`act_2017.csv` |Average ACT scores and participation rates by state and for U.S. in English, Math, Reading, Science, and Composite sections in 2016-2017 academic year|
|Average ACT scores by State (2018) | College Board |`act_2018.csv` |Average ACT scores and participation rates by state and for U.S. in Composite sections in 2017-2018 academic year|
|Average ACT scores by State (2019) | College Board |`act_2019.csv` |Average ACT scores and participation rates by state and for U.S. in Composite sections in 2018-2019 academic year|
|Average SAT scores by State (2017) | College Board |`sat_2017.csv` |Average SAT scores and participation rates by state and for U.S. in Evidence-Based Reading and Writing and Math sections and composite score in 2016-2017 academic year|
|Average SAT scores by State (2018) | College Board |`sat_2018.csv` |Average SAT scores and participation rates by state and for U.S. in Evidence-Based Reading and Writing and Math sections and composite score in 2017-2018 academic year|
|Average SAT scores by State (2019) | College Board |`sat_2019.csv` |Average SAT scores and participation rates by state and for U.S. in Evidence-Based Reading and Writing and Math sections and composite score in 2018-2019 academic year|
|Institutional Characteristics Data for Higher Education Institutions from the 19-20 Academic Year |U.S. Department of Education (The College Scorecard) |`institution-data-college-scorecard-2019_20_PP.csv` |Collection of higher education institution facts related to degree completion rates, SAT and ACT scores, first-year retention rates, average net revenues and more. These data are compiled by the U.S. Department of Education from the Integrated Postsecondary Data System, the National Student Loan Data System and more.|
|State abbreviations|Roger Allen's repository ([*source*](https://gist.github.com/rogerallen/1583593))|`state_abbreviations.csv`|Miscellaneous file used to generate geo map|

### Data Dictionary

A data dictionary for the College Scorecard data will be provided before to provide more detail on the variables that will be used for considered for use in this analysis. This data dictionary is adapted from the College Scorecard's website ([*source*](https://collegescorecard.ed.gov/data/documentation/)). All features below with the exception of the institution name are float numeric type variables and are the features used for this analysis.

|Feature|Description|
|:---|:---|
|unitid|Unit ID for institution|
|instnm|Institution name|
|sat_avg_all|Average SAT equivalent score of students admitted for all campuses rolled up to the 6-digit OPE ID|
|tuition_fte|Net tuition revenue per full-time equivalent student|
|pct_undergrad_pell_grant|Percentage of undergraduates who receive a Pell Grant|
|completion_rate|Completion rate for first-time, full-time students at four-year institutions (150% of expected time to completion)|
|full_time_retention_rate|First-time, full-time student retention rate at four-year institutions|
|openadmp|Open admissions policy indicator|

### Summary:
This project set out to understand the relevance of the SAT and ACT college entrance exams tests in today's quickly changing landscape of higher education. As many higher education institutions are opting to become test-optional in their admissions decisions, BFU requested advice on whether it should adopt a test optional admissions policy. To guide this decision, this analysis answered BFU's main research questions. The conclusions and recommendations are provided below.

### Conclusions and Recommendations:

The following are the conclusions from this analysis:
* Overall, there seems to be a direct and linear relationship between higher SAT scores and key outcomes of interest such as first year retention rates, graduation rates, and net revenues per FTE student
* Further analysis especially of peer regional organizations is necessary to better understand how they have faced the increasing trend of test-optional admissions. At this time, the university does not have sufficient evidence to adopt the test-optional policy as SAT scores appear to be strongly correlated with key academic outcomes such as degree completion and graduation rates.
* Students who receive a Pell grant tend to have financial needs that may prevent them for acquiring tutoring services to prepare for the SAT/ACT. The University should take into account the growing need to provide opportunities for admissions for well qualified students from diverse socio-economic backgrounds including students who receive Pell grants. Overall, the correlation of these key outcomes and the SAT is not as strong for students who receive Pell grants, which suggests that the University should promote policies that guarantee its commitment to the future academic success of the institutions and students from all backgrounds.
* Even though large university systems like the University of California system will be conducting test-optional admissions, the ACT and SAT tests are still prevalent in the U.S. and each has a greater share of the market in certain states.
