# Instagram

# 21479_8 Members
- [Emma Dolson](https://github.com/eld49325/EmmaDolson_MIST4610GroupProject1)
- [Hannah Kelly](https://github.com/hannahkelly98765/MIST-4610)
- [Shir Kochi](https://github.com/shirkorchi/GroupProject1)
- [Kaden Williams](https://github.com/kadenwilliams1/21479_-8)
- [Donovan Vanderpool](https://github.com/donovanv2/MIST4610/)

# Problem description
Our data model represents the social media app, Instagram. The model consists of user accounts, which have associated profiles, content, and followers/following relationships. Each post can have multiple associated media, such as images or videos, which users can interact with through likes, comments, and shares. Instagram also supports messaging between users and the creation of stories, which are temporary posts that expire after a set time period. Tracking user activity helps Instagram generate personalized recommendations and trends to improve user experience. Despite being one of the most popular social media platforms in the world, Instagram does not allow its users to schedule posts in advance or to create communities of niche interests. From a backend perspective, our model demonstrates how users would interact with these two features and new insights Instagram could gain from them.

# Data Model
![Screen Shot 2023-03-30 at 12 29 34 AM](https://user-images.githubusercontent.com/128401988/228729940-6e1e7645-8a3e-4d5b-ad53-8462281e5100.png)

A user can have many accounts but an account can only have one user. An account can send and receive many messages but a message can only have one sender and one receiver. The content scheduler can schedule multiple instances of content but an instance of content can only have one schedule. Accounts and content can have many shares but each share can only belong to one account that shares one instance of content. Accounts can make many comments but one comment can only be made by one account. Content can have many comments but one comment can only be added to one instance of content. Accounts and content can have many likes but a like can only belong to one account and one instance of content. Accounts can belong to many communities and communities can have many accounts. Communities can have many community types and community types can have many communities.
 
# Data Dictionary
[Data Dictionary.pdf](https://github.com/eld49325/EmmaDolson_MIST4610_GroupProject1/files/11107723/Data.Dictionary.pdf)

# Queries
TP_Q1: This query converts the user's date of birth into their age as an integer and then returns the names of users who are younger than the input age. A query like this is helpful for censoring content like rated R movie trailers or explicit music for underage users.
![Screen Shot 2023-03-30 at 6 10 37 PM](https://user-images.githubusercontent.com/128401988/228975952-f234cea1-e0df-4a5a-81ec-e56ddce18d3f.png)


TP_Q2: This query returns the username of accounts that have more followers than the average amount of followers for all accounts. A manager may be interested in this information to improve its algorithm and search engine.
![Screen Shot 2023-03-30 at 6 14 42 PM](https://user-images.githubusercontent.com/128401988/228975924-504bf5ab-16bc-4833-bd52-2227b2c1594b.png)

TP_Q3: This query returns the number of messages a community has sent if the message was sent during the day (12:00-18:00). A query like this is can be helpful in determining when communities are most active or when messaging servers could potentially reach capacity.
![Screen Shot 2023-03-30 at 10 04 36 PM](https://user-images.githubusercontent.com/128401988/229004811-b77e18de-98ee-4b82-8ca8-c96d945fcd10.png)

TP_Q4: This query returns the number of messages each account has sent in descending order given that the account has more than 500 followers. A manager may be interested in this data to gauge how active a particular account is.
![Screen Shot 2023-03-30 at 10 15 04 PM](https://user-images.githubusercontent.com/128401988/229005627-4a5c8a5b-46de-4986-a430-f6c0ccfd0bc2.png)

TP_Q5: This query returns the account handles that start with the letter "c," if any, as well as the name of the corresponding user and the community they belong to. A manager may be interested in this data to view information about accounts with related names quickly (by replacing “c” with whichever letter they choose). 
![Screen Shot 2023-03-30 at 10 20 38 PM](https://user-images.githubusercontent.com/128401988/229006480-c3de6787-1171-41a0-a86c-a4966375d4a7.png)

TP_Q6: This query returns all attributes pertaining to accounts and the community they're a part of if the account uses content scheduling. A query like this may be helpful in determining certain attributes (type of account, number of posts, etc.) that may play a factor in determining whether or not the account uses the content scheduling feature.
![image](https://user-images.githubusercontent.com/128401988/229006685-cdd56a3e-5c13-4649-8cb8-c1b6a8cbff48.png)

TP_Q7: This query will list the name and DOB of users that send messages with vanish mode and use content scheduling in order of oldest to youngest. A query like this is useful for tracking the use of some of the new features on Instagram. In more serious cases, this can also help track messages with illegal content back to their sender even if they attempt to hide the message by using vanishing mode.
![Screen Shot 2023-03-30 at 10 43 56 PM](https://user-images.githubusercontent.com/128401988/229009731-0c72005f-2083-4c19-ae5f-b2ad2dc292e2.png)

TP_Q8: This query will list accounts’ ID, handle, and the user’s name and email address associated with the accounts that have no video content posted. A query like this is useful for being able to identify and contact individuals to promote Instagram’s video functionality.
![Screen Shot 2023-03-30 at 10 48 31 PM](https://user-images.githubusercontent.com/128401988/229010324-79f27bde-239a-46be-b596-25f9dc809473.png)


TP_Q9: This query returns the account type and number of times each account type schedules content. A query like this could be helpful for adding possible features that cater towards account types that are frequent users of the content scheduler (ex. If a sports team has games every Saturday at noon, they can schedule a recurring post for each week of the season).
![Screen Shot 2023-03-30 at 10 51 43 PM](https://user-images.githubusercontent.com/128401988/229010798-223b204b-95b7-42eb-8501-2d9e88078e57.png)

TP_Q10: This query returns the number of shares for each content type. A manager may be interest in this data to determine what type of content is shared the most among users (could be useful for ad monetization, promotions, etc.).
![Screen Shot 2023-03-30 at 11 02 51 PM](https://user-images.githubusercontent.com/128401988/229012597-cf0cbdfa-f5da-46da-b5d9-66b192682852.png)

# Query Matrix
[Query Matrix.pdf](https://github.com/eld49325/EmmaDolson_MIST4610GroupProject1/files/11124917/Query.Matrix.pdf)

![Screen Shot 2023-03-31 at 2 28 49 PM](https://user-images.githubusercontent.com/128401988/229201894-21c90eaf-5bf3-4fa3-8654-3159203245b8.png)

# Database information
- Name: ns_21479_8
- Procedure format: TP_QX
