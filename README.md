# Modeling Instagram Data

# Group Members (21479_8)
• Hannah Kelly

• [Emma Dolson](https://github.com/eld49325/EmmaDolson_MIST4610_GroupProject1)

• [Shir Kochi](https://github.com/shirkorchi/GroupProject1)

• [Kaden Williams]()

• [Donovan Vanderpool](https://github.com/donovanv2/MIST4610/)

# Problem Description
Our data model represents the social media app, Instagram. The model consists of user accounts, which have associated profiles, content, and followers/following relationships. Each post can have multiple associated media, such as images or videos, which users can interact with through likes, comments, and shares. Instagram also supports messaging between users and the creation of stories, which are temporary posts that expire after a set time period. Tracking user activity helps Instagram generate personalized recommendations and trends to improve user experience. Despite being one of the most popular social media platforms in the world, Instagram does not allow its users to schedule posts in advance or to create communities of niche interests. From a backend perspective, our model demonstrates how users would interact with these two features and new insights Instagram could gain from them.

# Data Model
<img width="978" alt="Screenshot 2023-03-30 at 8 16 49 PM" src="https://user-images.githubusercontent.com/129444082/228992019-5361b9e6-338c-46cf-a6bd-bbe885eeeddb.png">
• 1:M Relationships: users have many accounts, users can send many messages, users can receive many messages, content schedule can schedule multiple content, accounts can have many shares, content can have many shares, accounts can have many comments, comments can be added to multiple content, accounts can have many likes, likes can be given to multiple content.


• M:M Relationships: accounts can belong to many communities and communities can have many accounts, communities can have many community types and community types can have many communities


# Data Dictionary
[Data.Dictionary.pdf](https://github.com/hannahkelly98765/MIST-4610/files/11117067/Data.Dictionary.pdf)

# SQL Queries
TP_Q1: This query converts the user's date of birth into their age as an integer and then returns the names of users who are younger than the input age. A query like this is helpful for censoring content like rated R movie trailers or explicit music for underage users.

![228975952-f234cea1-e0df-4a5a-81ec-e56ddce18d3f](https://user-images.githubusercontent.com/129444082/229138266-7b51f087-0690-4aee-b1ee-6c7b16b5301f.png)


TP_Q2: This query returns the username of accounts that have more followers than the average amount of followers for all accounts. A manager may be interested in this information to improve its algorithm and search engine.

![228975924-504bf5ab-16bc-4833-bd52-2227b2c1594b-1](https://user-images.githubusercontent.com/129444082/229138585-8476f7df-0b5a-4a67-8bf0-16cbfa87bfb3.png)



TP_Q3: This query returns the number of messages a community has sent if the message was sent during the day (12:00-18:00). A query like this is can be helpful in determining when communities are most active or when messaging servers could potentially reach capacity.


![229004811-b77e18de-98ee-4b82-8ca8-c96d945fcd10](https://user-images.githubusercontent.com/129444082/229138847-8df236c9-c6aa-4305-8fdc-7f889f7c4ac3.png)




TP_Q4: This query returns the number of messages each account has sent in descending order given that the account has more than 500 followers. A manager may be interested in this data to gauge how active a particular account is.


![229005627-4a5c8a5b-46de-4986-a430-f6c0ccfd0bc2](https://user-images.githubusercontent.com/129444082/229139020-2205586d-8889-4aa8-bc6c-6965c93ded7a.png)



TP_Q5: This query returns the account handles that start with the letter "c," if any, as well as the name of the corresponding user and the community they belong to. A manager may be interested in this data to view information about accounts with related names quickly (by replacing “c” with whichever letter they choose).

![229006480-c3de6787-1171-41a0-a86c-a4966375d4a7](https://user-images.githubusercontent.com/129444082/229139934-b22ec6ca-f7fe-42a0-abea-93a9c9888754.png)



TP_Q6: This query returns all attributes pertaining to accounts and the community they're a part of if the account uses content scheduling. A query like this may be helpful in determining certain attributes (type of account, number of posts, etc.) that may play a factor in determining whether or not the account uses the content scheduling feature.

![229006685-cdd56a3e-5c13-4649-8cb8-c1b6a8cbff48](https://user-images.githubusercontent.com/129444082/229139952-1ae34fa2-8707-4f5c-9418-8490f81bf9fe.png)


TP_Q7: This query will list the name and DOB of users that send messages with vanish mode and use content scheduling in order of oldest to youngest. A query like this is useful for tracking the use of some of the new features on Instagram. In more serious cases, this can also help track messages with illegal content back to their sender even if they attempt to hide the message by using vanishing mode.

![229009731-0c72005f-2083-4c19-ae5f-b2ad2dc292e2](https://user-images.githubusercontent.com/129444082/229140026-291263da-e5a0-4095-bac8-384bf5112d28.png)


TP_Q8: This query will list accounts’ ID, handle, and the user’s name and email address associated with the accounts that have no video content posted. A query like this is useful for being able to identify and contact individuals to promote Instagram’s video functionality.

![229010324-79f27bde-239a-46be-b596-25f9dc809473](https://user-images.githubusercontent.com/129444082/229140098-f0101a59-ca4e-43f9-a872-5a1840f31909.png)



TP_Q9: This query returns the account type and number of times each account type schedules content. A query like this could be helpful for adding possible features that cater towards account types that are frequent users of the content scheduler (ex. If a sports team has games every Saturday at noon, they can schedule a recurring post for each week of the season).

![229010798-223b204b-95b7-42eb-8501-2d9e88078e57](https://user-images.githubusercontent.com/129444082/229140148-39f9a4de-7d7a-446f-80b1-8b387707e11e.png)



TP_Q10: This query returns the number of shares for each content type. A manager may be interest in this data to determine what type of content is shared the most among users (could be useful for ad monetization, promotions, etc.).

![229012597-cf0cbdfa-f5da-46da-b5d9-66b192682852](https://user-images.githubusercontent.com/129444082/229140197-84eba843-a272-4f30-97dd-6fff6b160187.png)


# Query Matrix
[Query.Matrix.pdf](https://github.com/hannahkelly98765/MIST-4610/files/11122382/Query.Matrix.pdf)


![229013936-f2de64e6-3d0b-4abb-a739-bc9479cf21f6](https://user-images.githubusercontent.com/129444082/229136546-cd0cc594-d3d0-435f-a149-f6cf05164e20.png)

# Database Information
• Name: ns_21479_8

• Procedure format: TP_QX
