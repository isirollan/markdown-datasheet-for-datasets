# Datasheet: *Your Dataset Name Here*

Author: *Datasheet: Isidora Rollán Zegers
Dataset created by: Eduardo Gonzalez*

Organization: *UC Berkeley*


## Motivation

*The questions in this section are primarily intended to encourage dataset creators to clearly articulate their reasons for creating the dataset and to promote transparency about funding interests.*

1. **For what purpose was the dataset created?** Was there a specific task in mind? Was there a specific gap that needed to be filled? Please provide a description.

	*This dataset was created with the objective to document all bicycle accidents in Great Bretain from 1979 to 2018. Particularly, documents road bikes casualties. It clasify this casualties by the person affected, date, time, number of casualties involved, vehicles involved, speed limit, road conditions, light and weather conditions. Although the original author of this database didn't give a clear task of why he created this database, the author that uploaded to Kaggle (John Harshith) wanted to demonstrate "being a big fan of the sport and the number of unfortunate accidents happening across Great Britain inspired me to share this Dataset"(Harshith)*
	
2. **Who created this dataset (e.g. which team, research group) and on behalf of which entity (e.g. company, institution, organization)**?

	*This dataset was created by Eduardo Gonzalez, Analytics Engineer based on Seattle*


3. **What support was needed to make this dataset?** (e.g. who funded the creation of the dataset? If there is an associated grant, provide the name of the grantor and the grant name and number, or if it was supported by a company or government agency, give those details.)

	*Not applicable*

4. **Any other comments?**

	*The source of information is not specified by the author. *


## Composition

*Dataset creators should read through the questions in this section prior to any data collection and then provide answers once collection is complete. Most of these questions are intended to provide dataset consumers with the information they need to make informed decisions about using the dataset for specific tasks. The answers to some of these questions reveal information about compliance with the EU’s General Data Protection Regulation (GDPR) or comparable regulations in other jurisdictions.*

1. **What do the instances that comprise the dataset represent (e.g. documents, photos, people, countries)?** Are there multiple types of instances (e.g. movies, users, and ratings; people and interactions between them; nodes and edges)? Please provide a description.

	*Each instance is a unique identification of the accident with all the details available of the moment of the accident. Some instance contain more detail about the weather and road type, all of them have the rest of information (vehicles involved, casualties involved, date, time, speed limit, road conditions, day of the week).
	There is a second instance about the characteristics of the person affected with the accident- biker - detailing their gender, age range and severity. The way to cross information between the two instances is by the accident index*

2. **How many instances are there in total (of each type, if appropriate)?**

	*The dataset contains 827,861 unique accidents and 827,871 unique bikers affected.*

3. **Does the dataset contain all possible instances or is it a sample (not necessarily random) of instances from a larger set?** If the dataset is a sample, then what is the larger set? Is the sample representative of the larger set (e.g. geographic coverage)? If so, please describe how this representativeness was validated/verified. If it is not representative of the larger set, please describe why not (e.g. to cover a more diverse range of instances, because instances were withheld or unavailable).

	*All possible instances between the years 1979 to 2018 are inscluded in the dataset. Now, there can be valuable information that can be added as new characteristics to the dataset (where the biker using helmet, where the car/biker respecting traffic laws) by the author.*

4. **What data does each instance consist of?** "Raw" data (e.g. unprocessed text or images) or features? In either case, please provide a description.

	*It consist of text associated with bike accidents and bikers involved. This can be seen as raw data since it has to be analyze to take conclusions of it.*

5. **Is there a label or target associated with each instance?** If so, please provide a description.

	*There is a label associated with each instance that it "Accident_index". This is the index that allows to identify each individual accident and associate with the biker involved int that particular accident.*

6. **Is any information missing from individual instances?** If so, please provide a description, explaining why this information is missing (e.g. because it was unavailable). This does not include intentionally removed information, but might include, e.g. redacted text.

	*There is information missing from some individual instances, specially in data closer to 1979. This is most probably because that information was unavailable:
	- Weather_conditions: it is labeled as "Unknown".
	- Road type: it is labeld as "Unknown". *

7. **Are relationships between individual instances made explicit (e.g. users' movie ratings, social network links)?** If so, please describe how these relationships are made explicit.

	*Not applicable*

8. **Are there recommended data splits (e.g. training, development/validation, testing)?** If so, please provide a description of these splits, explaining the rationale behind them.

	*There is no recommended data splits*

9. **Are there any errors, sources of noise, or redundancies in the dataset?** If so, please provide a description.

	*There are some information label as "Unknown" and "Missing Data" that needs to be unify*

10. **Is the dataset self-contained, or does it link to or otherwise rely on external resources (e.g. websites, tweets, other datasets)?** If it links to or relies on external resources, a) are there guarantees that they will exist, and remain constant, over time; b) are there official archival versions of the complete dataset (i.e., including the external resources as they existed at the time the dataset was created); c) are there any restrictions (e.g. licenses, fees) associated with any of the external resources that might apply to a future user? Please provide descriptions of all external resources and any restrictions associated with them, as well as links or other access points, as appropriate.

	*It is self-contained. The original source is from https://data.world/gonzandrobles/bicycleaccidentsuk/discuss/bicycleaccidentsuk/timsmnv4 but it is also availabel in Kaggle with the same information.*

11. **Does the dataset contain data that might be considered confidential (e.g. data that is protected by legal privilege or by doctor-patient confidentiality, data that includes the content of individuals' non-public communications)?** If so, please provide a description.

	*No, all information is public. The details of the bikers affected are very broad which does not affect the privacy of individuals.*

12. **Does the dataset contain data that, if viewed directly, might be offensive, insulting, threatening, or might otherwise cause anxiety?** If so, please describe why.

	*In the bikers instance there is a "severity" - fatal, serious, slight -  category that might sound strong to some users. Specially if you relate fatal with some age rang. However, the fatal accidents are a very little portion of the dataset. *

13. **Does the dataset relate to people?** If not, you may skip the remaining questions in this section.

	*Yes, it is relate to people*

14. **Does the dataset identify any subpopulations (e.g. by age, gender)?** If so, please describe how these subpopulations are identified and provide a description of their respective distributions within the dataset.

	*Yes it describes subpopulations by age range (6-10 (8.2%), 11-15 (20.5%), 16-20 (14.8%), 21-25 (10.5%), 26-35 (17.5%), 36-45 (12.5%), 46-55 (8.9%), 56-65 (5.1%), 66-75 (1.9%)) and gender (male (79.7%), female (20.3%), other (0.0%)*

15. **Is it possible to identify individuals (i.e., one or more natural persons), either directly or indirectly (i.e., in combination with other data) from the dataset?** If so, please describe how.

	*Each biker or group of bikers has associtaed a Accident_index. This relate them with the particular accident, but no further details are given.*

16. **Does the dataset contain data that might be considered sensitive in any way (e.g. data that reveals racial or ethnic origins, sexual orientations, religious beliefs, political opinions or union memberships, or locations; financial or health data; biometric or genetic data; forms of government identification, such as social security numbers; criminal history)?** If so, please provide a description.

	*The dataset does not contain data that might be considered sensitive in any way*

17. **Any other comments?**

	*No further comments*


## Collection

*As with the previous section, dataset creators should read through these questions prior to any data collection to flag potential issues and then provide answers once collection is complete. In addition to the goals of the prior section, the answers to questions here may provide information that allow others to reconstruct the dataset without access to it.*

1. **How was the data associated with each instance acquired?** Was the data directly observable (e.g. raw text, movie ratings), reported by subjects (e.g. survey responses), or indirectly inferred/derived from other data (e.g. part-of-speech tags, model-based guesses for age or language)? If data was reported by subjects or indirectly inferred/derived from other data, was the data validated/verified? If so, please describe how.

	*It was inferred from other data and organized in single dataset.*

2. **What mechanisms or procedures were used to collect the data (e.g. hardware apparatus or sensor, manual human curation, software program, software API)?** How were these mechanisms or procedures validated?

	*Unkown*

3. **If the dataset is a sample from a larger set, what was the sampling strategy (e.g. deterministic, probabilistic with specific sampling probabilities)?**

	*Not applicable*

4. **Who was involved in the data collection process (e.g. students, crowdworkers, contractors) and how were they compensated (e.g. how much were crowdworkers paid)?**

	*Unknown*

5. **Over what timeframe was the data collected?** Does this timeframe match the creation timeframe of the data associated with the instances (e.g. recent crawl of old news articles)? If not, please describe the timeframe in which the data associated with the instances was created. Finally, list when the dataset was first published.

	*Data is from bike casualties from 1979-01-01 to 2018-12-20. This time frame is associated with the date of each instance of the dataset. This dataset was first published in 2020-09-19.*

7. **Were any ethical review processes conducted (e.g. by an institutional review board)?** If so, please provide a description of these review processes, including the outcomes, as well as a link or other access point to any supporting documentation.

	*Not applicable*

8. **Does the dataset relate to people?** If not, you may skip the remainder of the questions in this section.

	*This dataset contain basic demographic of people related in "bikers" instance.*

9. **Did you collect the data from the individuals in question directly, or obtain it via third parties or other sources (e.g. websites)?**

	*Unknown.*

10. **Were the individuals in question notified about the data collection?** If so, please describe (or show with screenshots or other information) how notice was provided, and provide a link or other access point to, or otherwise reproduce, the exact language of the notification itself.

	*Unkown.*

11. **Did the individuals in question consent to the collection and use of their data?** If so, please describe (or show with screenshots or other information) how consent was requested and provided, and provide a link or other access point to, or otherwise reproduce, the exact language to which the individuals consented.

	*Unknown.*

12. **If consent was obtained, were the consenting individuals provided with a mechanism to revoke their consent in the future or for certain uses?** If so, please provide a description, as well as a link or other access point to the mechanism (if appropriate).

	*Unkown.*

13. **Has an analysis of the potential impact of the dataset and its use on data subjects (e.g. a data protection impact analysis) been conducted?** If so, please provide a description of this analysis, including the outcomes, as well as a link or other access point to any supporting documentation.

	*Unkown.*

14. **Any other comments?**

	*The information of people involved in the dataset is very broad. It cannot identify a single individual from the information given about people. It is unknown if the dataset author ask for consent of any kind.*


## Preprocessing / Cleaning / Labeling

*Dataset creators should read through these questions prior to any pre-processing, cleaning, or labeling and then provide answers once these tasks are complete. The questions in this section are intended to provide dataset consumers with the information they need to determine whether the “raw” data has been processed in ways that are compatible with their chosen tasks. For example, text that has been converted into a “bag-of-words” is not suitable for tasks involving word order.*

1. **Was any preprocessing/cleaning/labeling of the data done (e.g. discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)?** If so, please provide a description. If not, you may skip the remainder of the questions in this section.

	*The information was organized to standarize its content. This make users to more easily analyze data and take insights from it:
	From bikers instance:
	1. Asigning the bikers to an according age range.
	2. Asigning casualties into 3 categories of severity: slight serious or fatal.
	
	From Accidents instance:
	1. Asgining weather conditions as clear, rain, clear and windy, raind an windy, fog, snow, snow and windy and Unknown when there is no information.
	2. Asigning road type as single carriageway, roundabout, dual carriageway, one way street, slip road or unknown when ther is no information.
	3. Asigning light conditions according the date and time of the year as daylight, darkness lights lit, darkness no lights.*

2. **Was the "raw" data saved in addition to the preprocessed/cleaned/labeled data (e.g. to support unanticipated future uses)?** If so, please provide a link or other access point to the "raw" data.

	*The data saved is only the preprocessed, labeled data*

3. **Is the software used to preprocess/clean/label the instances available?** If so, please provide a link or other access point.

	*Not Applicable*

4. **Any other comments?**

	*No comments.*


## Uses

*These questions are intended to encourage dataset creators to reflect on the tasks  for  which  the  dataset  should  and  should  not  be  used.  By  explicitly highlighting these tasks, dataset creators can help dataset consumers to make informed decisions, thereby avoiding potential risks or harms.*

1. **Has the dataset been used for any tasks already?** If so, please provide a description.

	*This dataset has been used to analyze the characteristics of bike casualties during the period 1979 to 2018. In that analysis it is shown that most of accidents are related to men, in single carriageway, with clear weather, mostly young people (11 to 35 years), most accidents are slight, they increase during summer season, most casualties ocurrs during weekday between 7 to 10 am and 3 to 7 pm.*

2. **Is there a repository that links to any or all papers or systems that use the dataset?** If so, please provide a link or other access point.

	*This analysis uses the dataset. https://www.kaggle.com/code/khsamaha/eda-bicycle-accidents-in-great-britain-1979-2018/report
	No other direct link to this dataset was found.*

3. **What (other) tasks could the dataset be used for?**

	*This could be used as a way to see what is causing major casualties to educate bikers and drivers to respect each other.*

4. **Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses?** For example, is there anything that a future user might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g. stereotyping, quality of service issues) or other undesirable harms (e.g. financial harms, legal risks) If so, please provide a description. Is there anything a future user could do to mitigate these undesirable harms?

	*Your Answer Here*

5. **Are there tasks for which the dataset should not be used?** If so, please provide a description.

	*Your Answer Here*

6. **Any other comments?**

	*Your Answer Here*


## Distribution

*Dataset creators should provide answers to these questions prior to distributing the dataset either internally within the entity on behalf of which the dataset was created or externally to third parties.*

1. **Will the dataset be distributed to third parties outside of the entity (e.g. company, institution, organization) on behalf of which the dataset was created?** If so, please provide a description.

	*Your Answer Here*

2. **How will the dataset will be distributed (e.g. tarball on website, API, GitHub)?** Does the dataset have a digital object identifier (DOI)?

	*Your Answer Here*

3. **When will the dataset be distributed?**

	*Your Answer Here*

4. **Will the dataset be distributed under a copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?** If so, please describe this license and/or ToU, and provide a link or other access point to, or otherwise reproduce, any relevant licensing terms or ToU, as well as any fees associated with these restrictions.

	*Your Answer Here*

5. **Have any third parties imposed IP-based or other restrictions on the data associated with the instances?** If so, please describe these restrictions, and provide a link or other access point to, or otherwise reproduce, any relevant licensing terms, as well as any fees associated with these restrictions.

	*Your Answer Here*

6. **Do any export controls or other regulatory restrictions apply to the dataset or to individual instances?** If so, please describe these restrictions, and provide a link or other access point to, or otherwise reproduce, any supporting documentation.

	*Your Answer Here*

7. **Any other comments?**

	*Your Answer Here*


## Maintenance

*As with the previous section, dataset creators should provide answers to these questions prior to distributing the dataset. These questions are intended to encourage dataset creators to plan for dataset maintenance and communicate this plan with dataset consumers.*

1. **Who is supporting/hosting/maintaining the dataset?**

	*Your Answer Here*

2. **How can the owner/curator/manager of the dataset be contacted (e.g. email address)?**

	*Your Answer Here*

3. **Is there an erratum?** If so, please provide a link or other access point.

	*Your Answer Here*

4. **Will the dataset be updated (e.g. to correct labeling errors, add new instances, delete instances)?** If so, please describe how often, by whom, and how updates will be communicated to users (e.g. mailing list, GitHub)?

	*Your Answer Here*

5. **If the dataset relates to people, are there applicable limits on the retention of the data associated with the instances (e.g. were individuals in question told that their data would be retained for a fixed period of time and then deleted)?** If so, please describe these limits and explain how they will be enforced.

	*Your Answer Here*

6. **Will older versions of the dataset continue to be supported/hosted/maintained?** If so, please describe how. If not, please describe how its obsolescence will be communicated to users.

	*Your Answer Here*

7. **If others want to extend/augment/build on/contribute to the dataset, is there a mechanism for them to do so?** If so, please provide a description. Will these contributions be validated/verified? If so, please describe how. If not, why not? Is there a process for communicating/distributing these contributions to other users? If so, please provide a description.

	*Your Answer Here*

8. **Any other comments?**

	*Your Answer Here*
