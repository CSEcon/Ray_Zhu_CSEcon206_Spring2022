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

### 1. Background and Motivation

Elections are frequently held over longer and set time intervals, ranging from months to years. This limits governance because it is difficult to remove elected people or policies before the next election, even if they are harmful to most participants. Participants may opt (via public deliberation) to change their vote if new information becomes available, but they will not be able to do so before the next elections (Blum and Zuber 2015). Another concern is the peak-end effect, in which voters make decisions based on how they felt just before the elections rather than the entire period of rule. Finally, there are some concerns about centralized e-voting, such as censorship and results and/or data manipulation (Blum and Zuber 2015).

### 2. Research Question

Can we overcome the problems of traditional voting, including the peak-end effect, censorship, data manipulation, and behavioral anomalies, by adopting the design of a repetitive blockchain-based voting mechanism？

>The peak-end effect: The peak-end effect is the phenomenon that people vote according to their impression of the candidates a short time before voting instead of carefully measuring the overall performance of the candidates over the long term (Venugopalan and Homoliak 2021). People may regret their votes due to the peak-end effect but have no way to change the vote until the next election in the traditional voting framework.

>Censorship/centralization/data manipulation: For voting that a centralized institution organizes, it might engage censorship and even render manipulation. We cannot ensure everyone's vote is properly shown in the result.

>Behavioral anomalies: When people make decisions, their rationality could be limited due to different factors or environments; in other words, people are not and cannot be completely rational all the time. This is called "bounded rationality"(Sent 2018). In voting, similarly, we cannot assume people are always making rational decisions. Substantial rationality is defined as "a form of rationality that considers the value of an action"(Jeanes 2019). According to Jeanes (2019), "Something can be considered substantively rational if the consequences of the actions are considered desirable by the social actor and actions are selected, measured, and judged by these values". However, opposite to substantial rationality, another concept, procedural rationality, refers to the "rationality of the processes used in arriving at a decision, as opposed to the rationality of the decision itself"(N. 2013). We should be cautious about different types of rationality as they are sophisticated and sensitive. Maybe a blockchain-based voting design like such could help us navigate through.

### 3. Methods

Venugopalan and Homoliak (2021) propose Always on Voting (AoV), a blockchain-based voting framework that allows participants to vote and alter elected politicians or policies on a continual basis without having to wait for the next election. Participants can modify their votes privately at any time, and the consequence of their changes is visible at the conclusion of each epoch, which is shorter than the interval between two major elections. Furthermore, the end of epoch times has been rendered unexpected.

According to Venugopalan and Homoliak (2021), AoV has three main characteristics: (1) it works in repetitive epochs, (2) voters can change their votes at any time before the end of each epoch (when the tally is performed), and (3) epoch ends are randomized and unpredictable. Only the supermajority of votes may change the prior winning vote decision at the end of each epoch.

### 4. Intellectual Merits

This paper contributes to mainly two strands of literature, blockchain application and public voting in economics and political economy. This paper investigated the political science research and economics research that led to an engineering solution for the peak-end effect problem, voter manipulation, and other problems (Venugopalan and Homoliak 2021). They demonstrated that existing voting methods provide little to no remedy for replacing elected candidates – even after they have fallen out of favor with a majority of voters (for years until the next general election). To defeat a mining adversary, the AoV architecture employs a variety of cryptographic and information security methods, including verified delay functions and Bitcoin block headers as a source of randomization (Venugopalan and Homoliak, 2021). This research provides a template for people to apply blockchain technology to the political economy.

### 5. Practical Impacts

To ensure security and cut costs, AoW makes use of a public-permissioned blockchain. It does not only provide a potentially workable solution to public voting but also expands the scope and imagination of blockchain applications, encouraging more people to make use of the advantages brought by blockchain networks to alleviate sunk costs caused by various behavioral anomalies and provide transparency and efficiency to public decision-making procedures. Participants' wallet privacy was achieved by syncing their wallet addresses with the Election Authority so that no third-party observer could map a future participant's wallet address to a previous or present one (Venugopalan and Homoliak 2021). Finally, they proposed a supermajority need to elicit a modification that reflects the present election outcome, which helps to keep the existing system stable.

## Part II: Critics 
![Support process example](https://user-images.githubusercontent.com/73629458/166884896-4de39cfb-9081-4207-9764-169b28f9b23d.png)

Figure 1. Critics from two perspectives

### 1. Economics for Computer Science: Incentives in Computer Science

I think the blockchain network and its implementation bring all benefits of this AoV system through computer science. In addition to immutability, anonymity, anti-censorship, and all other advantages a blockchain-based application may possess, I see the biggest advantage is the design of a blinding key, which makes sure that every single voting activity is run with basic functions in real life but with a more secure way. But I also regard its restriction in winner number as the main limitation in the hope that it could be overcome in the future.

A new blinding key must be used to blind a participant's vote whenever she alters her vote choice. It's possible that reusing blinding keys will betray the participant's vote. A blinded vote protects anonymity, and proof of set membership with zero knowledge ensures the vote is correct (without revealing any information about the vote choice). Even if the vote choice is kept private, a network attacker can see the voting events on the smart contract. A person may vote once in one period and then vote again in another. Due to the vote being blindfolded with a different blinding key, a network adversary is unable to tell if the participant voted for the same candidate or voted for a new candidate. However, both votes may be linked to the same participant blockchain wallet address, allowing identifying the number of times a member voted and drawing other statistical conclusions.

One major limitation that Always on Voting (AoV) has is that it is only suitable for voting with 1-out-of-k choices as a result. In other words, it does not support voting in which multiple winners would be generated. In the future, maybe the authors or other scholars or developers could improve on the algorithms and engineering design to make multiple winners plausible in this system. 

### 2. Computer Science for Economics: Practicality in Economics

This intellectual combination of blockchain, information collection, public voting, and other sophisticated designs embedded greatly improves traditional voting a lot in several aspects. To make it clearer, the implementation of the AoV framework could potentially address both problems with efficiency and fairness. 

First, efficiency could be raised as people are more likely to find the right person as a winner; even for the cases where the selected winner performs not as expected, they can immediately vote again, rebalance, find a better alternative, and cut loss in time. This is because a participant can vote at any point during an interval when they are updated with new information that was not available before she voted before. A participant may opt to amend her vote choice based on newly available facts and/or through public discussions. Participants can modify their votes at any moment in the AoV framework, and the consequence of the change is visible when the tally is computed at the conclusion of the epoch. Previously limitations in voting intervals and other inconveniences stemmed from technological restrictions. People have long been aware of the cost and opportunity cost brought by being committed to a voting winner, say, a president, but when we find it is not the right person, it takes much more time to change. And before we can finally make the change, the "wrongly" selected president may generate more significant negative impacts. Especially when he or she is trying to preserve the rights, we have no idea what cost we might have to pay. However, with AoV, we can cut loss in time. Moreover, when people have the right to change votes and even the president at any time, the power relations are redistributed. Those in power would be more careful about policies and regulations and better serve people's needs.

Second, fairness is shown by that a participant is fully de-identified, and their voting willingness could be fully shown in the AoV framework. As a result, ideally, everyone has an equally weighted vote in the public voting. Although traditional onsite voting is claimed to be fair, nobody can ensure that someone in charge or some interest groups may be engaged and manipulate the voting result. Even for the existing online voting system, as most of them are centralized and structured, we have no idea whether the results are manipulated or not, and the administrators might also reveal the voters' identities. Anonymization in voting aims to protect participants from being hurt and influenced. Suppose a participant can make sure they are completely safe and de-identified. In that case, he or she will make a decision that truly represents his real thoughts or preferences, as political economics suggests. On the other side, anti-manipulation could ensure the fairness and justice of the voting and show the willingness of everyone in the community in one and reveal the collective decision.

The first major limitation comes from the computer science implementation. Because the engineering design does not support multiple winners, many voting designs could not be performed through this AoV system. Voting with multiple winners is quite common in daily life, even more often to see than one-winner voting. For instance, DKU was voting for its Academic Principles Awards last month. These awards are to be given to 7 students. AoV is not suitable for that case.

The second limitation is that the capacity of AoV is limited given the complexity of structure and low speed in processing and maintaining the blockchain. Therefore, the application scale is quite limited. But with the newest generation of blockchain applications, I believe AoV could be expanded to a wider range and even work as, or provide inspiration at least, to the national election.

## Part III: Inspirations

### 1. Interdisciplinary Research
I think we can test the usefulness, efficiency, and reliability of the AoV framework's application in voting from different perspectives using interdisciplinary approaches. First, we can try it from a computational microeconomics perspective. We can program all voting environments and agents and simulates a scenario (and maybe reinforcement learning) to test whether it is workable, how it works, and where it could be improved. Second, from the perspective of data science, we can look for possible data sources online or collect them manually or crawl them automatically, depending on the data types and sources. Then, we can do statistical testing, data analysis, visualization with the data we have, and draw observations about voting. Last but not least, we can design lab experiments as economists would do. This methodology can form comparisons and show us the pros and cons of AoV voting with more nuances available.

### 2. Research for Real-world Practices
>RESEARCH QUESTION: Can the Always on Voting (AoV) framework help us find the right person for mayor? A comparison study between City A and City B.

In the future, we can find two political units in adjacent, say, two cities next to each other with similar economics, population, and cultural factors. With one piloting using the AoV framework, the other city uses the traditional voting scheme to vote for a mayor. We may regard this as a natural experiment and collect relevant data based on this. By comparing these two cities' voting and its outcomes (which could be reflected in the mayor's performance, the city's economics and employment indexes, and the frequency of vote change), we may conclude more about the advantages and disadvantages of the AoV framework.

### 3. Future Professional Growth
We have seen many examples of interactions between economics and computer science, and I am so convinced by its tremendous potential. On the one hand, computer science facilitates computing, setting up structures, connecting people from different locations, transforming great ideas into realities, and providing tools and platforms for economists to implement sophisticated economic and mechanism design. On the other hand, economics brings values, meanings, and application scenarios to computer science and makes the system more vivid and have commercial values. Looking into the future, I believe people like us, with visions in both economics and computer science, will lead in innovation by adopting the merits of both disciplines.

## Glossary Table
| Item        | Timeline    |  Description| 
| ----------- | ----------- | ----------- | 
|Consensus Algorithm|Consensus Algorithm is a fault-tolerant mechanism that is used in computer and blockchain systems to achieve the necessary agreement on a single data value or a single state of the network among distributed processes or multi-agent systems|(Frankenfield 2019)|
|Proof of Work (PoW)| Proof of Work (PoW) as an original consensus algorithm that requires effort solving mathematical puzzles is used to operate at the cost of additional CPU consumption, higher time cost, and lower system throughput, which cannot cope with the quality of service requirements of some scenarios|(Frankenfield 2019)
|Tally|A tally (also see tally sticks) is an unofficial private observation of an election count carried out under Proportional Representation using the Single Transferable Vote. Tallymen, appointed by political candidates and parties, observe the opening of ballot boxes and watch as the individual ballot papers are counted|(“Tally (Voting)” 2022)|
|Peak–end Effect (Rule)|The peak–end rule is a psychological heuristic in which people judge an experience largely based on how they felt at its peak (i.e., its most intense point) and at its end, rather than based on the total sum or average of every moment of the experience. The effect occurs regardless of whether the experience is pleasant or unpleasant|(Kahneman et al. 1993)|
|Substantive Rationality|An action may be regarded as rational because of the way it was chosen (procedural rationality), or because of its outcomes (substantive rationality)|("ScienceDirect Topics” n.d.)|
|Procedural Rationality|The rationality of the processes used in arriving at a decision, as opposed to the rationality of the decision itself.|("ScienceDirect Topics” n.d.)|

## References
Blum, Christian, and Christina Isabel Zuber. 2015. “Liquid Democracy: Potentials, Problems, and Perspectives.” Journal of Political Philosophy 24 (2): 162–82. https://doi.org/10.1111/jopp.12065.Frankenfield.

Jake. 2019. “Consensus Mechanism (Cryptocurrency).” Investopedia. 2019. https://www.investopedia.com/terms/c/consensus-mechanism-cryptocurrency.asp.

Jeanes. 2019. A Dictionary of Organizational Behaviour. Oxford University Press.

Kahneman, Daniel, Barbara L. Fredrickson, Charles A. Schreiber, and Donald A. Redelmeier. 1993. “When More Pain Is Preferred to Less: Adding a Better End.” Psychological Science 4 (6): 401–5. https://doi.org/10.1111/j.1467-9280.1993.tb00589.x.N.

Sam M. S. 2013. “What Is PROCEDURAL RATIONALITY? Definition of PROCEDURAL RATIONALITY (Psychology Dictionary).” April 28, 2013. https://psychologydictionary.org/procedural-rationality/.

“Procedural Rationality - an Overview | ScienceDirect Topics.” n.d. Www.sciencedirect.com. Accessed May 7, 2022. https://www.sciencedirect.com/topics/psychology/procedural-rationality#:~:text=Rationality%20in%20Society&text=An%20action%20may%20be%20regarded.Sent.

Esther-Mirjam. 2018. “Rationality and Bounded Rationality: You Can’t Have One without the Other.” The European Journal of the History of Economic Thought 25 (6): 1–17. https://doi.org/10.1080/09672567.2018.1523206.

“Tally (Voting).” 2022. Wikipedia. April 11, 2022. https://en.wikipedia.org/wiki/Tally_(voting)#:~:text=A%20tally%20(also%20see%20tally.

Venugopalan, Sarad, and Ivan Homoliak. 2021. “Always on Voting: A Framework for Repetitive Voting on the Blockchain.” ArXiv:2107.10571 [Cs], July. https://arxiv.org/abs/2107.10571.

### References in BibTex
```
@article{venugopalan_2021_always,
  author = {Venugopalan, Sarad and Homoliak, Ivan},
  month = {07},
  title = {Always on Voting: A Framework for Repetitive Voting on the Blockchain},
  url = {https://arxiv.org/abs/2107.10571},
  year = {2021},
  journal = {arXiv:2107.10571 [cs]}
}

@article{blum_2015_liquid,
  author = {Blum, Christian and Zuber, Christina Isabel},
  month = {07},
  pages = {162-182},
  title = {Liquid Democracy: Potentials, Problems, and Perspectives},
  doi = {10.1111/jopp.12065},
  url = {https://kops.uni-konstanz.de/bitstream/handle/123456789/31936/Blum_2-124tcdzkw7jqj0.pdf?sequence=1&isAllowed=y},
  urldate = {2020-04-22},
  volume = {24},
  year = {2015},
  journal = {Journal of Political Philosophy}
}

@misc{frankenfield_2019_consensus,
  author = {Frankenfield, Jake},
  title = {Consensus Mechanism (Cryptocurrency)},
  url = {https://www.investopedia.com/terms/c/consensus-mechanism-cryptocurrency.asp},
  year = {2019},
  organization = {Investopedia}
}

@misc{a2022_tally,
  month = {04},
  title = {Tally (voting)},
  url = {https://en.wikipedia.org/wiki/Tally_(voting)#:~:text=A%20tally%20(also%20see%20tally},
  urldate = {2022-05-05},
  year = {2022},
  organization = {Wikipedia}
}

@article{kahneman_1993_when,
  author = {Kahneman, Daniel and Fredrickson, Barbara L. and Schreiber, Charles A. and Redelmeier, Donald A.},
  month = {11},
  pages = {401-405},
  title = {When More Pain Is Preferred to Less: Adding a Better End},
  doi = {10.1111/j.1467-9280.1993.tb00589.x},
  urldate = {2020-02-29},
  volume = {4},
  year = {1993},
  journal = {Psychological Science}
}

@article{sent_2018_rationality,
  author = {Sent, Esther-Mirjam},
  month = {10},
  pages = {1-17},
  title = {Rationality and bounded rationality: you can’t have one without the other},
  doi = {10.1080/09672567.2018.1523206},
  volume = {25},
  year = {2018},
  journal = {The European Journal of the History of Economic Thought}
}

@book{jeanes_2019_a,
  author = {Jeanes},
  publisher = {Oxford University Press},
  title = {A Dictionary of Organizational Behaviour},
  year = {2019}
}

@misc{n_2013_what,
  author = {N. , Sam M. S.},
  month = {04},
  title = {What is PROCEDURAL RATIONALITY? definition of PROCEDURAL RATIONALITY (Psychology Dictionary)},
  url = {https://psychologydictionary.org/procedural-rationality/},
  urldate = {2022-05-07},
  year = {2013}
}

@misc{procedural,
  title = {Procedural Rationality - an overview | ScienceDirect Topics},
  url = {https://www.sciencedirect.com/topics/psychology/procedural-rationality#:~:text=Rationality%20in%20Society&text=An%20action%20may%20be%20regarded},
  urldate = {2022-05-07},
  organization = {www.sciencedirect.com}
}
```


## APPENDIX: Peer Comment & Feedback
### 1. Peer Comment
>I thoroughly enjoyed Ray’s Final Project draft. I would like to provide him with comments on the parts that I found inspiring and the parts that I think he could still improve.

>Good
Ray takes his time to slowly develop the ideas found in the research paper. The writing is clear and concise. The ideas are well-formulated without irrelevant parts. For example, the Methods section succinctly describes Always On Voting and its three key features.

>Areas for improvement
Some parts of the first draft are taken from the research paper. Ray could either paraphrase those sections or cite them. I would advise that he paraphrases as that will demonstrate his mastery of the material. Some terms, such as peak-end effect in Intellectual Merits and the EA in Practical Impacts, are new but undefined. Ray could refer to other sources that define these terms and use those definitions for better clarity. Of course, the sources should be cited as well. Unfortunately, I do not see Parts II and III in the GitHub repository, which makes my feedback limited because there is not enough information to work with. I hope that Ray finds the time to finish all of the Parts on time. I am happy to help him further outside of the school deadlines if he wishes.

>All in all, I am glad that I got to review Ray’s work. And since this is the last assignment, I must say that I am glad to have met him through CS/ECON 206 too! Perhaps Professor is most to thank for that.

### 2. Feedback
Thank you, Habib, for your thoughtful and helpful comments, and they help a lot. I benefit from this interation and have improved my assignment accordingly. In respond to your comments,

1. I already cited or quoted everything from the references, with a mixture with my own understanding and contributions. When you did the review, I am still working on my final project and had not committed the changes.
2. I explain all the terms carefully and even make a glossary table in the end. Hope this helps you understand my work.
3. Now I have all parts ready. Thanks for your reminder!

I also would like to say I am more than thrilled to study with you in my last college class. I wish you all the best in the future!
