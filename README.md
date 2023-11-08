# Analysis of Perspective API on Offensive Content 

## What I am testing 
Based on information from this study: https://www.adl.org/resources/report/very-fine-people , I chose to test whether the Perspective API can detect white supremacist language if the comments are made without profanity. 

The original datasets I pulled from are found at this site: 
https://www.openicpsr.org/openicpsr/project/156161/version/V2/view;jsessionid=4ABC483849F98BEA7F9A5EF1112A9E24 

The dataset files are too large to be uploaded to this repository, so only the cleaned and sampled data files are available in this repository. The original files can be found at the site link. 

I used two datasets: 
- Reddit: comments made by regular Internet users, representing a baseline 
- Stormfront: comments made by people on forums on a white nationalist website

I examined these attributes from the Perspective API:
- TOXICITY: "A rude, disrespectful, or unreasonable comment that is likely to make people leave a discussion."
- IDENTITY_ATTACK: "Negative or hateful comments targeting someone because of their identity."
- INSULT: "Insulting, inflammatory, or negative comment towards a person or a group of people."
- THREAT: "Describes an intention to inflict pain, injury, or violence against an individual or group."

## Hypotheses 
I hypothesized that the Perspective API is unable to identify white supremacist speech, especially if that speech is made in a manner without the use of profanity.

## Results
The flagging of comments with high identity attack scores was much more prevalent in the Stormfront data. Additionally, the rate at which these types of comments appear in the Stormfront data is much higher. The Perspective API was able to detect a difference between the Stormfront data and the Reddit data, despite the use of language not including profanity, disproving my hypothesis. 





