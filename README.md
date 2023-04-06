# Kickstarting with Excel

## Overview of Project
In this project we have a dataset of Kickstarter projects and their outcome. The client, Louise, had her play come close to its fundraising goal quickly but is interested in seeing how project timing and goals have affected other Kickstarter projects. I have the task to assess how campaigns fared depending on their launch date and their funding goals. To help assess these outcomes I have produced graphs to visualize the outcomes so the client and others can see and assess what the data contains in a condensed manner.

### Purpose
The purpose of this analysis is to visualize and analyze the dataset of Kickstarter projects using VBA and determine how different campaigns fared in relation to their launch dates and funding goals. In this analysis I have produced two deliverables. Deliverable 1 shows the relationship between campaign outcomes and launch dates, and in deliverable 2, I've shown the relationship between campaign outcomes and funding goals.

## Analysis and Challenges
Below are the analyses produced with the Kickstarter project data. An analysis of outcomes based on launch date as well as goal amount and the challenges faced to reach these findings.
### Analysis of Outcomes Based on Launch Date
This analysis was completed by extracting the year from the "Date Created Conversion" column into a newly created "Years" column. Using the new Years column I was able to create a pivot table which included filtering the data into successful, failed, and canceled categories. This data was filtered by month of the year for the analysis and with the parent category filtering to only show results from "theater" projects. Using this pivot table I produced a line chart, shown below, to visualize how a project's launch date relates to its chance for success.
![Theater Outcomes vs Launch](https://github.com/zbarham/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)
This chart shows the number of Successful, Failed, and Canceled projects by its launch month.

### Analysis of Outcomes Based on Goals
This analysis was completed by separating the data into goal ranges, increments of $5,000, as well as the number and percent of projects by their outcome. Using the function countifs I pulled the number of goals successful, failed, or canceled in the subcategory plays. Using the sum of total projects to generate a percentage for each category, I was able to display the gathered information in a meaningful way which was output to the line chart shown below.
![Outcomes vs Goals](https://github.com/zbarham/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)
This chart shows the Percentage of Successful, Failed, and Canceled projects by the monetary goal in increments of $5,000.

### Challenges and Difficulties Encountered
Most challenges in this analysis are based around growing my skills with VBA and pivot tables in excel, my speed was not to the level of someone who does this on a regular basis. The hint segments helped me learn some new tools by guiding me to the excel documentation and showing how to use the countif() function. After reviewing the documentation and video I learned how to use this function to filter down the data that I wanted to analyze in the outcomes based on goal deliverable.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
	- The conclusions that I have drawn from the outcomes based on launch date are that the best time to launch a play is late spring and summer, more specifically April through August with a peak in May, and that more projects are started on Kickstarter during this time period.

- What can you conclude about the Outcomes based on Goals?
	- The conclusions that I have drawn from the outcomes based on goals are that the monetary goal can have a large impact on the success of a project, small projects are generally successful up to $1,000 and this trends down as you approach the $5,000 mark, and that large projects have a sweet spot for success between $35,000 and $45,000 with projects more costly than this having a poor success rate as well as ones over less costly but over the $5,000 mark having a lower percentage of success overall as well.

- What are some limitations of this dataset?
	- Some limitations of this dataset are the inconsistency of projects started in different months, December having under half the count of projects as May which happens to be the least successful and most successful months respectively. This has a potential to have influenced the outcome as more data would reduce the influence of individual projects. A similar issue shows itself in the goals outcome with larger goal projects having significantly less entries than lower goal ones. The total goals in the upper end of $25,000 and above have single digit or just into the teens projects to look at to assess an average, only a single project from the $45,000 to $49,999 category. With lower goals such as $1,000 to $4,999 having over 500 entries' it helps reduce the influence of single entries compared to the heavy influence of single projects in the high end of goals.

- What are some other possible tables and/or graphs that we could create?
	- Some other tables or graphs that we could create with this data could be how close the pledged amount was to the goal amount both under and over to see how close a project was to succeeding or if some goals were funded significantly over the goal, this would be best assessed on a goal category like outcomes based on goals. This assessment would give an idea if certain cost categories bring almost enough or significantly more money than requested, this can help people see how profitable a project size might be or give an idea of how to adjust a goal for success. We could assess other categories such as film & video to see if they have different outcome trends than theater.
