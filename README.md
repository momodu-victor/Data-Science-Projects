# Predicting-the-out-of-state-total-cost-for-US-public-and-private-universities-and-colleges

## Introduction/ Background of Study
The US is characterized to be one of the intellectual factories of the 21st century as it has more than 5,300 colleges and universities. As the cost of university education in the USA increases every year, it is important for students to understand what this implies when deciding on their "dream school." Although various factors should be considered when choosing a university, such as academic reputation and distance from home, "cost" should be strongly evaluated as it is dependent on the state the student lives in. There is often a significant price difference when comparing private and public universities as well as students that are residents of the state vs. those who live in a different state. The present project aims to provide prospective university students with data that will enable them to evaluate the cost of university attendance by predicting the out of state total which many times can be financed or defrayed depending on the state the student comes from. Nonetheless, first it is important to understand the context in which we will be analyzing the research question.

Firstly, we should understand what is the difference between an in-state and out-of-state student. The US education system is controlled directly by each individual state rather than by the federal government. The public institutions within the state are financed by the taxes the state residents pay. As a consequence, state residents can attend these public schools for a lower cost, often referred as "in-state tuition", than those who do not live in the state that pay "out-of-state tuition." For the 2010–2011 academic year, the average tuition for an in-state student at a four year public school for an undergraduate student was $ 6,752. The average tuition for an out-of-state student at a four year public school for an undergraduate student was $ 15,742. This means that, on average, it cost $8,990 more for students to attend a college or university in a state where they are not a resident (National Center for Education Statistics, 2013).

Due to the significant price difference between in-state and out-of-state students, some states tend to be more stringent with regards to who qualifies to in-state tuition. For example, the policy on in-state tuition for the State University System of Maryland requires that a student have lived in the state for at least one year, did not move to the state solely to attend college, make Maryland their permanent residence indefinitely, and completely abandon the student’s previous home state (Heath Resource Center at the National Youth Transitions Center, n.d.). Yet, students may have the opportunity of applying for reciprocity programs that are agreements between states that reduce the cost of university attendance for out-of-state students by limiting the out-of-state tuition rate to 150% of the in-state tuition rate. As a student, you have to be aware that these reciprocity programs are competitive as they have a limited number of open positions. Use the following report to inform yourself on the cost of attendance per university so that you are able to apply early and take advantage of the cost savings!

**Source**: https://www.heath.gwu.edu/state-vs-out-state-tuition
National Center for Education Statistics. (2013). Search for schools, colleges, and libraries. Washington, DC: U.S. Department of Education Institute of Education Sciences. Retrieved from http://nces.ed.gov/globallocator/

## Purpose of Study.

Most prospective students and their respective guardians oftern have questions that revolve around the following:

- How much will it cost?

- How much do we save?

These are the most critical challenges in higher education planning.

According to The College Board’s Trends in College Pricing 2018, the average annual cost of out-state tuition, fees, room, and board at a four-year public institution is $25,370 for the academic year 2018–2019. For a private institution, the cost of tuition, fees, room, and board is $ 48,510. Both public and private colleges and universities experienced an increase of nearly 3% (2.8% for public and 3.2% for private) from the prior year, 2017–2018. Although the average tuition increase at private four-year schools is 3.3%, many students in this sector attend institutions with tuition increases of between 3% and 6%.If the cost of a college education increases by 6% annually, and your child enters a private college in the 2035–2036 academic year, the estimated tuition could be $57,544.

For young families, skyrocketing cost projections can lead to sticker shock, but there are strategies that can help you keep pace with tuition hikes

This project would help estimate the approximate annual out_of_state_total cost for a two or four-year undergraduate education for either a choice for public or private institution.

Hence, using the US education data, we are offering a solution by predicting the out-of-state total cost for public and private universities and colleges. This would facilitate data-driven decision making for the prospective student and improve planning and budgeting.

## Methodology

### a. Business Understanding:

Determining what the cost would be for higher education is one of the most critical challenges in the educational system. Hence,using the US education data,we want to predictthe cost of the out_of_state total cost would be as this would improve planning and budgeting for propsective students.
b. Data Retrieval: The data used for this project was retrieved in a csv format consisting the latest records of US education data for public and private universities and colleges.

The university dataset contains several higher education parameters.

**Attribute Information**:

**name**: The name of the university.

**total_enrollment**: Total number of students enrolled.

**state**: the state where the university is situated.

**n_native**: Number of students that are natives.

**n_asian**: Number of students that are asian.

**n_black**: Number of students that are black.

**n_hispanic**: Number of students that are hispanic.

**n_pacific**: Number of students that are pacifics.

**n_nonresident**: Number of students that are are not legal residents in the state where the university situated.

**n_total_minority**: Number of students that are minority.

**n_multiracial**: Number of students that are multiracial.

**n_unknown**: Number of students that are their demographic is unknown

**n_white**: Number of students that are white

**n_women**: Number of students that are women.

**state_code**: Unique state code for US states.

**type**: Type of university either public, private, for profit

**degree_length**: The duration of the course of study.

**room_and_board**: This is usually the accomodation and rent cost.

**in_state_tuition**: Tuition paid by students who are residents of state where the university situated.

**in_state_total**: This is the total cost for students who are legal residents in the state. It consist of the in_state tuition + room and board

**out_of_state_tuition**: Tuition paid by students who are non-residents of state where the university situated.

**out_of_state_total**: This is the total cost for students who are not legal residents in the state. It consist of the out_of_state tuition + room and board

**early_career_pay**: This is the average income a student who graduates from the university earns in the early years of career. This is usualy 1-2 years post graduation.

**mid_career_pay**: This is the average income a student who graduates from the university earns in the mid years of career. This is usualy 3-6 years post graduation.

**make_world_better_percent**: This is the percentage of the students who believe are making the world better.

**stem_percent**: This is the percentage of the students who studied STEM related programs.

Also, to build a robust predictive model, also used some other dataset in this project.

**tuition_income data**: This gives information on the total price, net cost, income level of all enrolled students for each university in the US.

Also, the **Human development index (HDI)** for each US state was used in the project. https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_Human_Development_Index

### c. Data Cleaning:

As a next step, this project will evaluate the missing values within the data set to better understand how to deal with them. First, we search for patterns within the variables through visual inspection. There, we speculate how the distribution of the missing values would look like if they were available by discussing if the missing data is “missing completely at random”, “missing at random” or “not missing at random.” Also data types are checked, to ensure that accuracy in the analysis. Before doing the analysis and prediction, the data is checked if it is normalized. Furthermore, it is ensured that all column names are well described.

### d. Data Exploration:

From the data set we explore basic questions to have a better understanding of the data. For example,which demographic characteristics are more pronounced for more expensive universities? How does the number of students from a particular region affect the total enrollement in states. Which groups are attracted to more expensive universities and so on.

### e. Data Visualization:

Several plots and charts are used to further understand the relationships between the features and out of state total cost.

### f. Feature Engineering/Selection: The following new features were included in the data set for better prediction of the out_of_state total

**n_men**: This is the number of enrolled students that are men.

**n_stem**: This is the number of enrolled students who studied a STEM programs.

**n_make_world_better**: This is the number of enrolled students who studied programs they believe make the world better.

**avg_net_cost**: The average total cost a student pays and subtracts any possible scholarships for which the student may receive.

**avg_total_price**: This average total cost of the universities over the years.

**HDI**: The Human Development Index of each state.

### g. Predictive Modelling:

At this point, we use a regression model to predict the possible out of state total cost. Every year, the model can be run and it helps prospective student determine the out of state total cost.

### h. Data-Driven Insights:

From the analysis, we gave data-driven insights and recommendation to prospective students as it relates to planning and budgeting the out-of-state cost.

## Key Findings and Insights

- There is total of 425 unversities in the top 10 US states by HDI. Out of which 211 are private, 197 are public and 17 are for profit.
- Most universities enrolled less than 10,000 students.
- Most universities enrolled less than 100 native students.
- Most universities enrolled less than 50 asian students. However,some universities above 1000 asian students that were enrolled.
- Most room and board cost between 12,000 and 16,000 dollars.
- Most students earn between 45,000 and 58,000 dollars in their early career.
- Less than 25% of students studied STEM related program at the university.
- Most natives attend less expensive universities.
- Non resident students attend the most expensive universities which could be private for profit universties.
- The number of women being enrolled in the universities is increasing.
- White students are kind of evenly distributed in the type of universties they attend in terms of cost. A good number go to expensive as well as less expensive schools.
- The out_of_state_tuition is the most relevant to determine the out_of_total cost.
- All cost variables (in_state_tuition, in_state_tuition total,average total price, average net cost, room and board ) important in predicting the out_of_state total.
- The number of non_residents students in the universities play a key role in predicting the out_of_state total.

## Recommendations based on the insights
- Start a disciplined savings plan now from the results of the prediction. It will better positioned to meet future education needs.
- Ensure that the school you plan on attending is one that your financial pockets can afford as you have ample time to plan since the expected out of total cost has been forecasted.
- Women could apply to less expensive universities as there is a high admission rate for the femine gender. Possibly applying to STEM courses could be a good option.
