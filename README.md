# Vitoria-SMARTEES-Survey

## USE OF SURVEY DATA FOR MODELS

A survey was carried out in Vitoria in November 2020 as part of the SMARTEES project. Data from this survey was employed in the models for two purposes:

1) To fill in the characteristics of the agents and their social networks 2) To generate the population of agents so that it is compatible with the sociodemographic characteristics of the surveys as well as those of the real population of the city.

## Data for agents and social networks

The main entity of the model is the citizens that are characterized following the HUMAT model. For the Vitoria model, after analysing the data survey it was determined that each citizen will have six categories of needs (dimensions), instead of the original three of the HUMAT model: (1) wellness needs, which, among others, refer to health and security, (2) environmental quality needs, referring to air and noise pollutions, (3) comfort, which, among others, refer to house price and parking, (4) city prestige, (5) participation needs, referring to possibility to participate in city decisions and (6) social needs, referring to belongingness, relatedness, social safety, social status, etc. Each of these needs is conditioned by the importance that each citizen gives to it. How much a citizen accepts or rejects the Social Innovation project (SI) is calculated by an additive function that takes 1) how much each alternative satisfies her in each group of needs and 2) the importance that the agent gives to each of these groups. After initializing the satisfaction and importance of these needs using this survey and following the HUMAT model, the citizen agents form an initial opinion about the SI that will evolve over time due to the modification of their needs and the influence of their social networks.

The direct relationship between the questions in the survey and the dimensions considered in HUMAT are shown in the following table.

Dimensions Survey question code

|Dimensions| |Survey question code|
|:----|:----|:----|
|Wellness|Importance|P16_1, P16_3, P16_6, P17_7|
| |Satisfaction|P20_2, P20_5, P20_8, P22_2, P22_4, P22_5|
|Environmental Quality|Importance|P16_2, P16_4, P17_3, P17_8, P17_9|
| |Satisfaction|P20_1, P20_4, P20_10, P20_11|
|Comfort|Importance|P16_5, P17_1, P17_5, P17_6|
| |Satisfaction|P20_3, P20_7|
|Prestige|Importance|P18_3|
| |Satisfaction|P20_6|
|Participation|Importance|P18_5, P18_6, P18_7|
| |Satisfaction|P23, P24|

The survey can be checked (note that it is written in Spanish)

In addition to citizens, the model incorporates critical nodes, i.e., important entities, specifically in Vitoria the following were included: city council, merchants associations, other associations and local media.

There are different social networks (friends, neighbours...) between citizens. The dimension of these networks for each citizen was also taken from the survey, i.e., the number of links to create. Each pair of citizens in the same network are connected through a pair of weighted links, the weight representing the trust one agent has on the other (notice that trust does not have to be reciprocal). Similarly, critical nodes are connected to citizens through weighted unidirectional links coming from the critical node, the weight represents the trust the citizen has on the critical node. In this case, the number of links to generate was determined using secondary data sources (for example, Twitter followers). All trust parameters were taken from the survey.
