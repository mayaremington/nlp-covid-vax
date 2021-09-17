Abstract
As of early September 2021, the COVID-19 delta variant continues to surge in the US. This wave is primarily affecting the unvaccinated, yet 25% of adults decline to get the shot. It is well established that social media platforms have been used to spread anti-vaccine misinformation - and that such messaging can fuel vaccine hesitancy. Using a database of anti-vaccine Tweets, I  performed NMF-based topic modeling with the goal of identifying topics within the anti-vaccine movement. I ended-up with 9 topics. Based on my review of the Tweet text, I broke down the topic into 3 groups: strongly anti-vaccine, pro-vaccine (mostly), and a mix of both. I plotted each of the topics over time to view trends. One important take-away is that specific COVID anti-vaccine messaging has been around since at least November - well before most individuals in the US were eligible for the vaccine. When it comes to handling the next pandemic, public health officials may want to consider addressing anti-vaccine messaging earlier (i.e. well before the vaccine is ready for distribution).

Design
The most recent COVID wave is primarily affecting the unvaccinated, yet 25% of adults decline to get the shot. It is well established that social media platforms have been used to spread anti-vaccine misinformation - and that such messaging can fuel vaccine hesitancy. Understanding this messaging is crucial for ending this pandemic and preparing for the next one. The goal of this project is to use natural language processing - specifically topic modeling - of Twitter data to identify sub-topics within the anti-vaccine movement.

Data
I obtained a database of 1.8 million TwitterIDs from the paper referenced below. The study authors collected the data by querying the Twitter API with 59 anti-vaccine keywords. This was performed in real-time between November 2020 - April 2021. I hydrated the TwitterIDs using the Hydrator app (https://github.com/DocNow/hydrator), which returned the reconstituted Tweet text in addition to metadata (date/time, username, etc). I received 1.1 million Tweets from Hydrator, indicating that 700K Tweets have likely been deleted by Twitter (given that Twitter reports having removed large numbers of users because they spread vaccine misinformation). After removing duplicates, the total number of tweets was 367K.

*Muric G, Wu Y, Ferrara E. COVID-19 Vaccine Hesitancy on Social Media: Building a Public Twitter Dataset of Anti-vaccine Content, Vaccine Misinformation and Conspiracies, arXiv:2105.05134 [cs.SI] 2021

Algorithms
I performed pre-processing on my text data using sklearn and regex. I removed links and ‘@mentions’ but kept hashtag text (just removed the ‘#’). Then I performed topic modeling using NMF. I ended-up with 9 topics. Based on my review of the Tweet text, I broke down the topic into 3 groups: strongly anti-vaccine, pro-vaccine (mostly), and a mix of both. I plotted each of the topics over time to view trends. One important take-away is that COVID anti-vaccine messaging has been around since at least November - well before most individuals in the US were eligible for the vaccine.  

Tools
I used python text processing libraries for my analysis - primarily scikit learn.

Communication
Looking forward to the presentation!
