**MVP:**

My goal is to use topic modeling of Twitter data to identify sub-topics within the COVID-19 anti-vaccine movement. So far, I have hydrated a dataset of Twitter IDs into full Tweets, cleaned the data, and created a baseline model. This baseline model involved some basic pre-processing (removing links, user mentions, punctuation, numbers, generic stop-words) followed by topic modeling with NMF (10 topics). Here are the results, along with my best approximations so far (obviously these need more optimization):

Topic  0: possibly school-related
unvaccinated, risk, children, kids, going, person, population, vaccination, teachers, new

Topic  1: possibly pro-vaccine (getting/got fully vaxxed/vax)
vaxxed, fully, getting, got, vax, ll, going, ve, time, mask

Topic  2: Bill Gates conspiracy theories (plan for global/world control and depopulation, etc) 
depopulation, agenda, gates, world, vaccines, plan, control, global, new, population

Topic  3: CDC masks indoors
people, virus, masks, think, risk, like, cdc, need, getting, indoors

Topic  4: possibly work-from-home
amp, kids, virus, work, vax, home, ppl, ll, spread, symptoms

Topic  5: vaccine passports, but also ‘vaccines are experimental’ 
vaccine, virus, passports, getting, doesn, does, ll, pfizer, experimental, rate

Topic  6: another cdc masks/mask
vaccinated, fully, person, risk, virus, cdc, masks, spread, mask, unvaccinated

Topic  7: doctor, but also deaths
covid, vaccines, spread, got, dr, deaths, kids, months, risk, tested

Topic  8: don’t need OR need vaccines and/or masks at work
don, want, know, think, need, vaccines, care, work, mask, wear

Topic  9: ?
just, like, got, think, going, say, ve, time, right, make


My next steps will be to improve upon this baseline model by altering the number of topics, removing less-helpful words (covid, vaccine(s), virus, etc), adding stemming, and adding spell-check. I may also try bigrams, named entity recognition and/or compound term extraction, and converting emojis to words. 

