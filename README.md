# Databel Customer Churn Dashboard

## Tools & Skills Used

![Tableau](https://img.shields.io/badge/Tableau-Dashboard-%235778a4)
![Tableau](https://img.shields.io/badge/Tableau-Data%20Analysis-%235778a4)
![Tableau](https://img.shields.io/badge/Tableau-Interactive%20Filtering-%235778a4)  

## Quick Access

- [Raw Data](/databel-data.csv)
- [Datacamp's Metadata Sheet](/databel-datacamp-metadata.pdf)
- [Tableau Workbook](/databel-customer-churn.twbx)
- [Tableau Public Dashboard](https://public.tableau.com/app/profile/annelize.krause/viz/DatabelCustomerChurn_17521508586280/customer-churn)

## Project Overview

This is a guided case study by DataCamp: [Analyzing Customer Churn in Tableau](https://app.datacamp.com/learn/courses/case-study-analyzing-customer-churn-in-tableau). I investigate a dataset for a telecom company Databel to analyze customer churn to figure out why customers are churning at the rate they are. The deliverable is a cohesive Tableau story containing the following dashboards with appropriate filters:

1. **Overview**

- KPIs for number of customers, number of churned customers, as well as the churn rate
- A bar graph showing the reasons customers churn
- A pie chart showing the churn by category
- A donut chart showing the customers by contract type
- A map visualization with the churn by state

2. **Age Bracket & Groups**

- A histogram showing number of customers in each age bracket with the churn rate overlayed
- A column chart showing the number of customers in groups with the churn rate overlayed

3. **Data & International Plan**

- A column chart comparing data usage grouped into categories to differentiate between customers on a data plan and those who are not
- Heatmap analyzing whether customers are on an international plan and actively calling internationally with the respective churn rate
- KPIs for number of customers, number of churned customers, total extra data charges, and total extra international charges

4. **Payment Method & Contract Type**

- Scatterplot analyzing churn rate against account length, payment methods and contract type
- KPIs for total number of customer service calls and average number of customer service calls

## My Approach & Design Decisions

While this project is based on DataCamp’s guided case study, I made several thoughtful customizations to improve the user experience and analytical clarity:

### Refined Churn Category & Reason Mapping

I cleaned the churn reason and category fields using calculated logic by:

- Clearly separating current customers from churned ones.
- Assigning `Unknown` to all blank reason and category fields.
- Reclassifying the ambiguous reason `Don't know` (originally under the `Other` category) to `Unknown` for consistency.

These changes significantly improved segmentation clarity, making patterns easier to interpret and filters more reliable across the dashboards.

### Dashboard Story Reorganization

Rather than following the original dashboard sequence, I designed four thematic dashboards with cleaner segmentation and more focused insights:

- **Overview:** KPIs and combined breakdown of churn category and churn reason, allowing removal of the now-redundant category chart and enabling the addition of a new perspective with an age demographic visualization.
- **Churn by Region:** A dedicated map with expanded real estate and filter controls for contract type and age demographics.
- **Customer Profiles:** Deeper segmentation by age, tenure, and gender.
- **Behavior & Support:** Combined age-based churn with behavioral factors like service calls, data usage, and extra charges, offering more actionable insights than payment method analysis.

### Interactivity Enhancements

I consistently used donut charts throughout for intuitive segmentation. These allow filtering by contract type, age group, gender, or data plan status depending on context, which makes the dashboards highly interactive and adaptable.

### Presentation Polish

I designed a cover and introductory page in Canva, embedded them as dashboard images, and included LinkedIn hyperlinks for professional visibility and portfolio continuity.

## Story Preview

Below is a preview of the final Tableau Story. Experience the full interactive story [here](https://public.tableau.com/app/profile/annelize.krause/viz/DatabelCustomerChurn_17521508586280/customer-churn).

![Story Preview](/databel-customer-churn.gif)

## Final Thoughts

This project evolved well beyond a guided exercise into a polished, data-driven storytelling experience. Every visualization was carefully curated to make the insights clearer, the interactions smoother, and the story more engaging. I’ve aimed to create a solution that’s both functional and actionable, and this project challenged me to think like a designer, analyst, and storyteller.
