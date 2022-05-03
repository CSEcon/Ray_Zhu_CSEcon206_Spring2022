# The Future of Computional Microeconomics: Comments for "[Always on Voting: A Framework for Repetitive Voting on the Blockchain](https://arxiv.org/abs/2107.10571)"

> *Disclaimer: Submissions to the Final Project for [COMPSCI/ECON 206 Computational Microeconomics](https://ce.pubpub.org/), 2022 Spring Term (Seven Week - Second) instructed by [Prof. Luyao Zhang](http://scholars.duke.edu/person/luyao.zhang) at Duke Kunshan University.*

## Citation of the Article 

Venugopalan, Sarad, and Ivan Homoliak. 2021. “Always on Voting: A Framework for Repetitive Voting on the Blockchain.” ArXiv:2107.10571 [Cs], July. https://arxiv.org/abs/2107.10571.

in BibTex
```
@article{venugopalan_2021_always,
  author = {Venugopalan, Sarad and Homoliak, Ivan},
  month = {07},
  title = {Always on Voting: A Framework for Repetitive Voting on the Blockchain},
  url = {https://arxiv.org/abs/2107.10571},
  year = {2021},
```

## 

## Part I: Summary
[Mindmap Created by Whimisical]

### 1. Background and Motivation

Elections are commonly repeated over longer and fixed intervals of time, ranging from months to years. This results in limitations on governance since elected candidates or policies are difficult to remove before the next election even though they might be deemed detrimental to the majority of participants. When new information is available, participants may decide (through a public deliberation) to make amendments to their choice but have no opportunity to change their vote before the next elections. Another issue is the peak-end effect where voters’ judgment is based on how they felt a short time before the elections, instead of judging the whole period of the governance. Finally, there exist a few issues related to centralized e-voting, such as censorship and tampering with the results and data. 

### 2. Research Question

Can we overcome the problems of traditional voting by adopting the deisgn of a repetitive blockchain-based voting mechanism？

### 3. Methods

We propose Always on Voting (AoV) — a repetitive blockchain-based voting framework that allows participants to continuously vote and change elected candidates or policies without having to wait for the next election. Participants are permitted to privately change their vote at any point in time, while the effect of their change is manifested at the end of each epoch whose duration is shorter than the time between two main elections. Further, the times of epoch ends were made unpredictable.

AoV has three key features: (1) it works in repetitive epochs, (2) voters are allowed to change their vote anytime before the end of each epoch (when the tally is performed), and (3) ends of epochs are randomized and unpredictable. At the end of each epoch, only the superma- jority of votes can change the previous winning vote choice

### 4. Intellectual Merits

We reviewed the works in political science that motivated an engineering solution to the peak-end effect problem in voting and voter manipulation. We showed that existing voting systems provide little to no recourse for changing the elected candidates (for years until the next main election) – even when they had fallen out of favor to a majority of voters. The AoV framework uses various tools in cryptography and information security such as verifiable delay functions to thwart a mining adversary and Bitcoin block headers as the source of randomness.

### 5. Practical Impacts

AoW utilizes a public permissioned blockchain to ensure the security properties and to save costs. Wallet privacy of participants was achieved by synchronizing participant wallet addresses with the EA in such a way that no third- party observer can map any future participant’s wallet address to the current or previous one. Finally, we proposed a supermajority requirement to elicit a change reflecting the current result of the election, which helps to maintain the stability of the existing system.


## Part II: Critics 
[Mindmap Created by Whimisical]

### 1. Economics for Computer Science: Incentives in Computer Science

Type here

### 2. Computer Science for Economics: Practicality in Economics

Type here


## Part III: Inspirations
[Mindmap Created by Whimisical]

### 1. Interdisciplinary Research
Type here
### 2. Research for Real-world Practices

Type here
### 3. Future Professional Growth
Type here

### References
Type here

### References in BibTex
```









```


