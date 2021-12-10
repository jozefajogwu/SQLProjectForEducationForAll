# SQLProjectForEducationForAll


Project Description
I am a Data Analyst working a Hypothetical NGO, named Education for All, I have been asked by the head of Fundraising to present the Data for Donor insights and Donor rates
The Problem
My Job role intertwines with working with the fundraising team, and we are set with the following Objectives below: • Increase the number of donors in your database • Increase the donation frequency of your donors. • Increase the value of donations in your database.
Your root cause analysis process
In analyzing the business problem, I asked myself the following questions.
• Why do persons of Certain Professions and Career Paths have Different Paths?
• Which Profession had the highest Frequency of Donation?
• Amongst both Genders who had the highest Donation?
• Based on insights how do we reach out to Donors to encourage them to donate more especially the Donors who frequently donate?
Insights from the dataset (including your SQL Code)
1. Getting the top donors from the dataset I used the following SQL code:
SELECT donation_data.first_name, donation_data.donation, donation_data.gender, donation_data.state, donor_data. donation_frequency, donor_data.university
FROM donation_data
JOIN donor_data
on donation_data.id = donor_data.id
ORDER BY donation_data.donation DESC
From the dataset I deduced that two males Beverlie and Wallie has the largest Donation, both from Michigan and New York respectively.
2. Which Profession had the highest number of Donors
SELECT donation_data.first_name, donation_data.donation, donation_data.gender, donation_data.state, donor_data.donation_frequency, donor_data.university, donation_data.job_field
FROM donation_data
JOIN donor_data
on donation_data.id = donor_data.id
ORDER BY donation_data.donation DESC
From the dataset I deduced that Wallie and Beverlie who are amongst the two largest donors work in both Project Management and Support respectively.
3. Why do persons of Certain Professions and Career Paths have Different Paths?
The have varying donations based on the purchasing power as individuals
4. Based on insights how do we reach out to Donors to encourage them to donate more especially the Donors who frequently donate?
SELECT donation_data.first_name, donation_data.donation, donation_data.gender, donation_data.state, donor_data.donation_frequency, donor_data.university, donation_data.job_field, donation_data.shirt_size
FROM donation_data
JOIN donor_data on donation_data.id = donor_data.id
ORDER BY donation_data.donation DESC
From the SQL statement we can send customized messages to each donor in their native languages since we can find it from the data thanking them for the effort in donating and also encouraging them to donate more, and since we have the shirt sizes of each of them we can share personalized thank you tshirts too our top donors, showing our appreciation for their kind guesture
4. Tableau visualizations of these insights
.
From the table above,
• Males had the highest donors, though the donated yearly,
• Females where the least donors though the donated daily
In Relation to Job Roles:
• Persons in Product Management, Human Resources and Marketing were the highest Donors
• Persons in Legal where the least Donors
In relation to states with highest Donors:
California had the highest Donors, followed by Texas and New York
5 Important findings and recommendations to solve the business problem In relation to the business problem, I would proffer the following solutions • Since we have the Tshirt of all donors, we can make customized t-shirts and send to those in states who made the highest donations such as New York, Texas and California this would further serve as an encourage to them to donate more.
• Persons in Product Management, Human Resources and Marketing where the highest Donors should be incentivized so as to encourage them to donate more. • Messages should be sent to both Genders especially the females to encourage them to donate more since the donate daily and have a higher rate in donation IN CONCLUSION
In order to boost the rate and frequency of donation at all fronts, those who have frequently donated, should be encourage
