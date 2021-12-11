# DATA ANALYST SQLProjectForEducationForAll


Project Description<br>
I am a Data Analyst working for an NGO, <bold>named Education for All</bold>,
<br> I have been asked by the head of Fundraising to present the Data for Donor insights and Donor rates<br>
The Problem
My Job role intertwines with working with the fundraising team, and we are set with the following Objectives below:
<br> • Increase the number of donors in your database</br>
<br> • Increase the donation frequency of your donors.</br>
<br> • Increase the value of donations in your database.</br>
Your root cause analysis process
<b>In analyzing the business problem, I asked myself the following questions.</b>
  <li>• Why do persons of Certain Professions and Career Paths have Different Paths?</li>
  <li>• Which Profession had the highest Frequency of Donation?</li>
  <li>• Amongst both Genders who had the highest Donation?</li>
<li>• Based on insights how do we reach out to Donors to encourage them to donate more especially the Donors who frequently donate?</li>
<b>Insights from the dataset (including your SQL Code)</b><p>
1. Getting the top donors from the dataset I used the following SQL code:<br>
<b><i>SELECT donation_data.first_name, donation_data.donation, donation_data.gender, donation_data.state, donor_data. donation_frequency, donor_data.university
FROM donation_data
JOIN donor_data
on donation_data.id = donor_data.id
ORDER BY donation_data.donation DESC
  <i></b>
  
  
  <p>
From the dataset I deduced that two males Beverlie and Wallie has the largest Donation, both from Michigan and New York respectively.
    <p>
2. Which Profession had the highest number of Donors<br>
      <p>
<b> <i>SELECT donation_data.first_name, donation_data.donation, donation_data.gender, donation_data.state, donor_data.donation_frequency, donor_data.university, donation_data.job_field
FROM donation_data
JOIN donor_data
on donation_data.id = donor_data.id
  ORDER BY donation_data.donation DESC</i></b>
      <p>
From the dataset I deduced that Wallie and Beverlie who are amongst the two largest donors work in both Project Management and Support respectively.<br>
        <p>
3. Why do persons of Certain Professions and Career Paths have Different Paths? <br>
          <b> <i> The have varying donations based on the purchasing power as individuals </i> </b>
          <p>
4. Based on insights how do we reach out to Donors to encourage them to donate more especially the Donors who frequently donate?<br>
            
<b> <i> SELECT donation_data.first_name, donation_data.donation, donation_data.gender, donation_data.state, donor_data.donation_frequency, donor_data.university, donation_data.job_field, donation_data.shirt_size
FROM donation_data
JOIN donor_data on donation_data.id = donor_data.id
            ORDER BY donation_data.donation DESC </i> </b>
            <p>
From the SQL statement we can send customized messages to each donor in their native languages since we can find it from the data thanking them for the effort in donating and also encouraging them to donate more, and since we have the shirt sizes of each of them we can share personalized thank you tshirts too our top donors, showing our appreciation for their kind guesture
              <p>
4. Tableau visualizations of these insights
.
From the table above,
                <li> Males had the highest donors, though the donated yearly,</li>
                <li> Females where the least donors though the donated daily</li>
                ![image](https://user-images.githubusercontent.com/36554181/145657465-42754dcf-9598-433e-8c81-8fefa01b1225.png)

In Relation to Job Roles:

                <li> Persons in Product Management, Human Resources and Marketing were the highest Donors</li>
                <li> Persons in Legal where the least Donors</li>
In relation to states with highest Donors:
                <li>California had the highest Donors, followed by Texas and New York</li>
5 Important findings and recommendations to solve the business problem In relation to the business problem, I would proffer the following solutions
                <li> Since we have the Tshirt of all donors, we can make customized t-shirts and send to those in states who made the highest donations such as New York, Texas and California this would further serve as an encourage to them to donate more.</li>
                ![image](https://user-images.githubusercontent.com/36554181/145657331-ef5646d0-32c3-45ce-9cb3-9b092dac5f1a.png)

<li>Persons in Product Management, Human Resources and Marketing where the highest Donors should be incentivized so as to encourage them to donate more.</li>
       <li> Messages should be sent to both Genders especially the females to encourage them to donate more since the donate daily and have a higher rate in donation</li>
                <p>
                  
                  <b>Tableau visualizations of these insights</b>
               ![image](https://user-images.githubusercontent.com/36554181/145657236-d82fe640-d724-42e3-83fa-d02d47d6cced.png)


                  
                <b> IN CONCLUSION</b>
                  <p>
In order to boost the rate and frequency of donation at all fronts, those who have frequently donated, should be encourage
