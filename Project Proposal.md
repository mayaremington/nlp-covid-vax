Question/need:
- What is the framing question of your analysis, or the purpose of the model/system you plan to build?
	- As of early September 2021, COVID-19 cases are again on the rise in the United States, fueled by the highly contagious delta variant and primarily affecting the unvaccinated. As a result, encouraging the 25% of unvaccinated adults to take the vaccine is of primary importance. It is well established that social media platforms have been used to spread anti-vaccine misinformation - and that such messaging can fuel vaccine hesitancy. Understanding this messaging is the first step towards addressing it. The goal of this project is to use natural language processing - specifically topic modeling - of Twitter data to identify sub-topics within the anti-vaccine movement.
- Who benefits from exploring this question or building this model/system?
	- Understanding anti-vaccine messaging is crucial for government and public health officials at all levels (local, state, federal) as well as anyone in the position to counsel unvaccinated individuals (doctors, clergy, community members, etc.)

Data Description:
- What dataset(s) do you plan to use, and how will you obtain the data?
	- I plan to obtain tweets from the Twitter API using the anti-vaccine keywords identified in this paper: https://arxiv.org/pdf/2105.05134.pdf. I will start with the most recent month’s data, and ideally by the end I will have data from approximately October 2020 to the present. If the dataset grows close to 1 GB in size, I will work with a sample of the data..
- What is an individual sample/unit of analysis in this project? What characteristics/features do you expect to work with?
	- An individual unit of analysis will be a single tweet within a term-document matrix. I will perform topic modeling using LDA 
- If modeling, what will you predict as your target? 
	- As of right now, the plan is for a completely unsupervised project - so no target

Tools:
- How do you intend to meet the tools requirement of the project?
	- My primary data will be written text documents in the form of tweets
- Are you planning in advance to need or use additional tools beyond those required? 
	- I’m considering using Tableau to create visualizations

MVP Goal:
- What would a minimum viable product (MVP) look like for this project?
	- A baseline model using LDA and 30-40 topics
