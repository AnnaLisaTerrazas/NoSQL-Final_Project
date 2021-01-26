# Lesson 5 Hands On 19 points

# Directions

Welcome to the last project for the NoSQL course! Great job making it this far! This hands on will be different from the hands on projects you have previously seen in a couple of different ways. You will be putting together the numerous topics you have learned into one large project. It is designed to mimic real problems which you may face in your career, so it may be a challenge for you and will also take several hours. Take this project step-by-step and be aware that the project description below is written to be a bit less specific than previous Hands-Ons. The hands on is supposed to challenge you to do some problem solving to figure out how to accomplish a task. You can always review past lessons or use a Google search if needed. Good luck!

# Caution!

Do not submit your project until you have completed all requirements! You will not be able to resubmit.

# Requirements

For this hands on, you will be working through several real-life scenarios within new collections. This Hands-On is structured into two parts, and each part will ask you to run multiple queries. After each query, please take a screenshot and add it to a text document (or an equivalent) and name this file Lesson5handson. This way, you will be able to submit your answers to each part all at once.

# Part 1

You have just been hired at a startup company. They currently only have ten employees, but they need to be included in the database. So far, they have only been tracked within an excel sheet. Your boss would like you to create a new collection in Atlas named employees. Take a look at the following data and the notes listed below before inserting any data:

Name	Birthday	Address	City	State	Position Name	Remote	Full Time
Alison Davidson	04/05/75	874 W. Oak Place	Gary	Indiana	Customer Support	Yes	Yes
Henry Chapelton	09/29/80	9324 E. Vista Way	Tempe	Arizona	Customer Support	No	Yes
Alex Miller	11/22/83	244 Price Road	Mesa	Arizona	Customer Support	No	No
Carly Nielson	08/04/87	678 W. Westward Road	Phoenix	Arizona	Office Manager	No	Yes
Tom Talbot	12/30/89	12 Oakland Way	Chandler	Arizona	Inventory Manager	No	Yes
Mary Crawley	07/06/80	1010 Granite Way	Charlotte	North Carolina	Human Resources	Yes	Yes
Daisy Baxter	09/09/87	990 E. 84th St.	Tempe	Arizona	CEO	No	Yes
William Coyle	10/11/91	944 W. 16th St.	Phoenix	Arizona	Intern	No	No
Edith Bates	07/28/90	7 E. 20th Pl.	Chandler	Arizona	Customer Support	No	Yes
Gwen Harding	10/11/86	234 W. 48th. St.	Phoenix	Arizona	Office Assistent	No	Yes
Notes:

The Birthday field should have a data type of Date.
The Position Name, Remote, and Full Time fields should be within an embedded document called position.
Remote and Full Time fields should have boolean values.
It's been about a month since you have inserted all employees into the database. There have been a couple of changes to the company. The CEO decided that he no longer wants remote employees, so they have transferred the remote employees and they are now living in Arizona. Alison Davidson now lives at 777 E. 1st St. # 120 Tempe, AZ and Mary Crawley now lives at 8322 W. Vista Pl. Scottsdale, AZ. Since all employees now all live in Arizona, there is no need to have a field named "state" within this collection, so please remove it. Lastly, they would like very efficient searching using the "position" field (remember that field includes a document with three other fields).

# Part 2

You are currently working for a company who wants to build an app similar to Spotify. Below is a list of data for different songs. Please insert this data into a new collection named songs.

SongId	Title	Artist	Album	ReleaseYear
1	Girls Just Want To Have Fun	Cyndi Lauper	She's So Unusual	1983
2	Hips Don't Lie	Shakira feat. Wyclef Jean	Oral Fixation Vol. 2	2006
3	Poker Face	Lady Gaga	The Fame	2008
4	Wannabe	Spice Girls	Spice	1996
5	California Gurls	Katy Perry feat. Snoop Dogg	Teenage Dream	2010
6	Bye, Bye, Bye	NSYNC	No Strings Attached	2000
7	I Will Always Love You	Whitney Houston	I Will Always Love You: The Best of Whitney Houston	2012
8	Baby One More Time	Britney Spears	Baby One More Time	1999
9	Vogue	Madonna	I'm Breathless	1990
10	Rolling in the Deep	Adele	21	2011
11	1234	Feist	The Reminder	2007
12	Elastic Heart	Sia	The Hunger Games: Catching Fire Soundtrack	2015
13	Oops! I Did It Again	Britney Spears	Oops! I Did It Again	2000
14	Bad Romance	Lady Gaga	The Fame Monster	2009
15	Lose Control	Missy Elliot	The Cookbook	2005
16	U Can't Touch This	MC Hammer	Please Hammer, Don't Hurt 'Em	1990
17	Thriller	Michael Jackson	Thriller	1982
18	Single Ladies	Beyonce	I am... Sasha Fierce	2008
19	Rhythm Nation	Janet Jackson	Janet Jackson's Rhythm Nation 1814	1989

# Notes:

The artist, album, and releaseYear fields should be an embedded document named details.
Be sure that the songId and releaseYear fields have a type of number.
Next, your company has run into some things they would like to be changed within the database:

The title field needs to be renamed to songTitle, so it is clearer to the developers working with the data.
They would like to have the artist field to be outside the details document but the album and releaseYear should stay within that document.
