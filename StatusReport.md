

Updated Timeline:

Now that we are at the interim report deadline of 11/16, we have approximately 2 working weeks before the final project deadline of 12/7 (excluding Fall break). After receiving feedback from our original project plan, we refined our project dataset and question to reflect the current stated goal of understanding the relation between air fares, flight delays, and weather. 

So far, we have:

1) **Completed** step 1 of loading in the 3 different datasets. We followed the breakdown that was established in the project plan to do so. We utilized similar column names to ease the process of combining the three datasets. A general review has also been done to confirm that there are no mistakes in loading and cleaning the 3 datatsets.
   - Cleaned Dataset 1: https://drive.google.com/file/d/1bkkLNLhGYTZp0vq7RHAfgzmdAU26i4tp/view?usp=drive_link
   - Cleaned Dataset 2: https://drive.google.com/file/d/1_NBXFiq1sdnEnZ5BHLfdfkALgZXk-aqv/view?usp=drive_link
   - Cleaned Dataset 3: https://drive.google.com/file/d/1_1e9WZg-BZ1dbj6xe0yQMMA_Nk5X1-21/view?usp=drive_link
2) **Completed** step 2 of meeting as a team and comparing datasets to confirm the scope of our research question. We were able to determine that these 3 datasets are able to be combined together to answer our research question, and we are now moving on to the following steps. This leads us to the interim deadline of 11/16, and our main interim deliverable is the combined dataset.
3) **Completed** step 3 of combining the three cleaned datasets into one dataset, so that we can analyze the relationships between air fares, flight delays, and weather.
   - Combined Dataset: https://drive.google.com/file/d/1vf7kaRPKSrCpz_n8FhRd-dS9TZhtr0yj/view?usp=sharing
4) **Completed** Sample visualization to answer part of research question: https://colab.research.google.com/drive/1xGWvY1AsbH96FOnRjU55DPNqUrE7lvFS?usp=sharing

Up next:

3) Arianna will load in the 3 datasets into a combined file after determining that all 3 datasets have been adequately cleaned. Anna, Amy, and Sophie will review this combined file to ensure that all team members agree with the compatibility and combination of the dataset. We will then meet again to discuss the patterns that we notice from the dataset. At this point, we will start understanding the analysis and discussing what visualizations will be most effective and efficient to communicate the information of the dataset. We will also address any major limitations or gaps at this time.
4) Once we have determined what visualizations to commit, we will execute and refine the final deliverable so that it is a strong final project. This will be completed by the final deadline of 12/7. We will also do a final review of the limitations and gaps present, addressing as many as we can to ensure a strong deliverable by the deadline. 

Since we have reached the interim deadline, at this point we do not expect any further modifications to our timeline. This is the timing of deliverables from here on out, and we will be following this timeline closely to ensure we are complete with the project by 12/7.

Changes to the Project Plan:

This project has undergone many changes since it has started. The main change is that the entire research question and topic has been shifted. It originally attempted to analyze museum art data, and compare it to different museums across the world in terms of funding, accessibility to visit the museums, and how funding affects the museums galleries. After receiving feedback from the second milestone, we realized that our data of different museums would not integrate with each other as the datasets were all on the same playing field and we needed them to work with each other to solve our research question. We attempted to keep the same topic and just adjust datasets, but this was proven to be very challenging, so we shifted topics entirely. We have now moved to work with weather, airline delay, and airfare data. This topic has much more prevalent data available and allows us to integrate the three chosen datasets together
to answer our research question. As for the rest of our project plan, it remains to be very similar. We have divided up the datasets to clean, and are on path of combining the datasets and analyzing the patterns found within. Our timeline, however, is still not final and is subject to change as seen fit. 

Any challenges or problems you have encountered so far:

We initially had problems with narrowing the scope of our project to make it feasible to be completed within the semester. We decided to shift our focus from museum galleries to airport and weather data as it proved to have data that was easier to combine and develop a research question with. From there, the following challenge was being able to have consistent schema and specifically column data in order to combine the three datasets, but overall, it was handled well by our team members. We did find limitations found in the combined dataset specifically when beginning to develop a visualization that answers a part of our research question. We found that some flights had no weather data however we accounted for this by using only flights that had a matched weather record when creating our first visualization. Also, rainy hours are something that tend to happen at larger airports, so the chart cannot claim that rain causes delay, but rather that is an association that cannot simply be boiled down to causal relationship. We also know that our data is limited to the scheduled departure hour and not the actual departure time, so we noted that in our visualization to normalize it across all observations that that is the time we are using. Finally, delay rate counts flown flights only (cancelled flights are excluded from that rate); cancellation rate counts all scheduled flights. 



Team Member Summaries

Amy - My main responsibility is understanding and cleaning the Air Fare dataset. Because the original dataset that we chose for this purpose was unexpectedly invalid, I also had to find another dataset that would fit our scenario and help answer our research question. When cleaning the Air Fare dataset, I focused on the same dates and quarters as established by Anna's weather data, and I changed the columns to the pre-decided standardizations to ensure seamless integration with the other datasets. 

Anna - My main responsibility is understanding and cleaning the Delayed Flight dataset. I was the first in the group to clean my dataset, so I was able to pick the months that we would analyze in the data. These months were January and June of 2025. After cleaning the dataset, I provided my other teammates with steps they can take in cleaning their dataset so that the information pulled was consistent within each individually cleaned dataset. This allowed for the integration of all three datasets to be much smoother. I also contributed to this milestone by answering the changes to our project plan section. I also contributed to the revision of our second milestone by partaking in the meeting with the TA to discuss the original issues, meeting with the team separately to plan out our new project plan, and adjusting the gaps section of the project proposal as needed to work with our new data. 

Sophie - My main responsibility is understanding and cleaning the Weather dataset. I focused on extracting relevant weather measurements from the NOAA hourly weather data for January and June 2025. While cleaning the dataset, I had to handle missing values and fix the formatting for timestamps. In order to make the merging step easier, I mapped the weather stations in the dataset to the airports they were connected to. Finally, I attended the meeting with the TA and all of the group meetings, to help refine our research question and plan the next steps in the project. 

Arianna - My responsibility was to look over the cleaned datasets to make sure there weren't any discrepancies. Once the cleaned datasets were consistent, I was able to combine them into one dataset using pandas and google colab, and used assertions in python to confirm that no data was lost in the process. Once that was complete, I was able to summarize any challenges or problems we've encountered so far including a shift in our original project plan, as well as clarifications to the limitations in the current combined dataset. I was then able to provide a sample visualization as the TA we discussed with was hoping to see what visualizations we would be able to come up with given our current research question. 
