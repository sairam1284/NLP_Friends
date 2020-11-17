# Project 4

## Background
---  
The 90's had some of my favorite sitcoms by far.  For this project, I wanted to look at every script from the tv Show Friends and see what types of observations I could make by just looking at the dialogue.  I want to see if I can use Natural Language Processing (NLP) to provide some insight into the characters and themes discussed in the show.    

## Data
---
- Scraped from the following site: https://fangj.github.io/friends/
- Obtained 30,000+ lines of dialogue between the primary characters

## Methodologies

---
- BeautifulSoup for web scraping
- CountVectorizer and TfidfVectorizer pre-processing techniques for tokenization
- Corex and NMF for topic modeling


## Findings
---


#### 1. Themes Discussed in the show
The 1st part of my project utilized Corex to extract the different themes discussed throughout the show. Looking at how the themes changed as the characters got older was very interesting.  Specifically, I noticed that As characters grew older, the topics regarding family seemed to decrease which makes sense as one gets older they tend to spread apart from the family.  In addition I noticed that themes regarding marriage and children were slow in the mid 20-'s but really picked up once characters started reaching 30 years of age.  

- **Final Remarks -** I found this so interesting because I think one of the reasons this show was so popular was that it really depicted the lives people transitioning from their mid-20's to mid-30's; going from dating around to discussing marriage and kids. 
![Friends Themes](/Images/Themes.png)
--- 
#### 2. Character Analysis
I wanted to see if Corex was able to distinguish the different characters of the show.  Looking at some of the associated words, it is clear that Corex did quite a good job at this. 

![Friends characters](/Images/Joey-words.png)
--- 
#### 3. Character Word Usage
For this part, I really wanted to dive into the commonly overlooked words and see if I could glean any sort of useful information about the characters.  
1. **Discourse Words** - These are words which are used commonly but don't really add value to a sentence.  Examples include (uh, um, like, y'know).  I found that roughly 4% of the total words used consisted of these words with Rachel and Phoebe consisting the highest percentage. 
2. **I Words** - These words may indicate someone who talks about themselves a lot. (I, me, my, myself). Approximately 7% of the dialogue consists of these words.  Rachel had the highest at 7.5% which is not surprising giving the stereotype her character had as the spoiled one
3. **You Words**-  These words may indicate someone who is bossy.  (you, your, you've).  Approximately 5% of the dialogue and Monica had the highest at 5.2%.  
- **Final Remarks-** It was really interesting to see that just by looking at certain types of words, one could really ascertain a lot of information about one's speech patterns.  
![Friends word types](/Images/Word_Types.png)
