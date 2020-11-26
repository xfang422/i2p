# Data Biography

## Student Number: 20141163

---

### 1. Who collected the data?

The data utilizes public information compiled from the Airbnb website. The data scientists behind Airbnb and their empowered teams collate the data on their clients. 

---

### 2. Why did they collect it?

The data in the list gives information on housing sources and market feedback, which we can see how Airbnb is being used to compete with the residential housing market[1].

---

### 3. How was it collected?

It scrapes data from the Airbnb website for a city (labeled a search area), and stores the result in a database. Each collection of a single city is called a survey. A single database holds many separate surveys, including some of the same city. The database system used is now PostgreSQL[2].


---

### 4. What useful information does it contain?


* Host information: the host's basic identity information, self-description, response rate, and evaluation information, etc.

* House Information: the location and neighborhood of the house, the type of house and room, the number of people to accommodate, and the basic configuration of the room.

* Rental time and price: the longest and shortest rental days for different properties and the number of days available for the whole year.

* Reviews feedback: the number of reviews over different periods, the score feedback from different aspects of the house, and the overall experience evaluation.


---

### 5. What useful information is it missing?


* guest information: no guest information is collected, like gender，name，require license，guest profile picture，phone verification, etc. So we can not analyze the Characteristics of Airbnb's target audience.

* Specific reviews: no specific feedbacks, both good and bad reviews, to describe the living experience more objectively. Adding corresponding reviewers' name/ID is necessary to avoid vicious competition.

* Marketing channels: only a single promotion platform link, no different client registrations, the number of registrations in different promotion channels, the number of registrations in different marketing content, conversion rate in different promotion channels; conversion rates for different marketing content, etc.


---

### 6. To what extent is the data 'complete'?

“Completeness” refers to how comprehensive the information is and whether all of the data you need is available[3]. In terms of host information and housing information, the data provided by the data set is relatively complete, and the reliability. It can be classified and studied in terms of the location, type, facilities, rental time, and other aspects of the house. However, in terms of user feedback and marketing data, the data set is incomplete. Although the data set gives general feedback and evaluation, the information and specific evaluation of consumers are missing. Therefore, we cannot improve specific feedback or analyze the characteristics of market customers. In the part of marketing and promotion information, it is missing. So we can not be the follow-up development of the focus of the promotion.


---

### 7. What kinds of analysis would this support?

Based on the known information provided in the data set, we can have a basic understanding of the basic information of the host and the condition of the house. By ranking the different rating reviews and combining them with the situation of house amenities and host information, summarize their popular factors and characteristics and propose improvement Suggestions for the houses with lower scores. Besides, By clustering analysis of the longest and shortest rental time of different housing sources, different housing sources can be classified according to long and short time rental, combined with the location to provide consumers with the optimal rental time choice.

According to the location of the house information, combined with municipal geographical maps (eg, ESRI shapefiles of neighborhood boundaries), the data can be used to analyze listings by neighborhood within a city[1]. It also can summarize the impact of Airbnb on nearby areas, such as rent prices or changes in real estate.


---

### 8. What kinds of analysis would it _not_ support?

Due to we lack specific comments, we cannot know the real reasons for users to give relevant reviews scores, so we cannot make promotion and improvement on what users are satisfied and bored with, making targeted improvements is hard. If we know more user's personal information, according to the differences in age, gender, geographical distribution, and other aspects of customers, we can timely adjust the promotion methods and platforms, to improve the quantity and quality of new users.

On the other hand, if we get corresponding data on promotion channels. Through analysis, we can sort out which channels have better effects, to timely adjust and increase the input of this channel, which channels are not effective so that timely find the reasons and give solutions.


---

### 9. Which of the uses presented in Q.7 and Q.8 are _ethical_?

In the supported analysis, when we study the popularity of different properties, the host's information must be taken into account. Some of the analysis will violate the right of portrait and privacy of the householder. A recent study on Airbnb listings in New York City provides supporting evidence for our assertion by suggesting that personal photos might facilitate racial discrimination. Specifically, the authors find that non-black hosts in New York City charge higher prices than their black counterparts, and suggest that this effect is driven by the use of photos, which reveal the hosts' race[4]. On the contrary, analysis based on objective facts, such as the relationship between geographical location and urban structure and the length of the lease, can bypass the defects of ethics and morality.

In the unsupported analysis, getting comments that users post publicly is within the bounds of ethics. As Kozinets notes, the "download of existing posts do not strictly qualify as human subjects research[5]. It is only where interaction or intervention occurs that consent is required"[6]. Similarly, Marketing information is also based on real data and has no privacy or security implications. However, if users' personal privacy information is involved in analysis, data analysis without users' consent will violate the moral bottom line to a certain extent.

 

### References

[1] http://insideairbnb.com/about.html 
 
[2] Tomslee, "Airbnb Data Collection: Methodology and Accuracy ", 2020. [Online]. Available: https://tomslee.net/airbnb-data-collection-methodology-and-accuracy. 

[3] N. Emran, "Data Completeness Measures", 2015. [Online]. Available: https://www.researchgate.net/publication/280722439_Data_Completeness_Measures. 

[4] B. G. Edelman and M. Luca, “Digital Discrimination: The Case of Airbnb.com,” SSRN Electron. J., 2014, doi: 10.2139/ssrn.2377353. 

[5] W. He, H. Wu, G. Yan, V. Akula, and J. Shen, “A novel social media competitive analytics framework with sentiment benchmarks,” Inf. Manag., vol. 52, no. 7, pp. 801–812, 2015, doi: 10.1016/j.im.2015.04.006. 

[6] N. Hookway, "'Entering the blogosphere': some strategies for using blogs in social research - Nicholas Hookway, 2008", SAGE Journals, 2020, pp. 91-113. [Online]. Available: https://journals.sagepub.com/doi/abs/10.1177/1468794107085298.