# Interoperability Exercise
In order to demonstrate the ability for different solution providers to communicate using a common traceability standard (GDST 1.0), a exercise style exercise has been proposed where participants from varying backgrounds and parts of the supply chain will come together and demonstrate interoperability. Through doing this, GDST will enable several solution providers to state their ability to use the standard to achieve end-to-end traceability for seafood companies. A traditional exercise has groups compete for prizes, but this event will focus on existing products and development environments being used collaboratively to achieve joint outcomes. We are simulating real life situations (integrations) in an environment with GDST expertise and dummy data to enable interoperability.

## Participants and Groups
The exercise will be composed of participants from different roles of the supply chain that are grouped together to demonstrate they can implement an interoperable solution.

Each participant could have potentially 1 or 2 members. Participants would be grouped into groups of 3 or more. The goal should be to keep the groups big enough to model a complex supply chain, but small enough to be productive. To make it easy for the groupings, participants would sign up ahead of time and the groupings would be made ahead of time to ensure that group members shared similar working hours.

### Identified Groups

**Group 1:** WholeChain and TraceRegister

**Group 2:** Plumensoft, OpenSC, GoChain

Each group would be assigned a supply chain scenario to model where each participant in the group would represent a trading party in the example supply chain. They would be tasked with simulating the example supply chain.

## Advisors
GDST secretariat staff and other traceability experts knowledgeable about seafood supply chains will participate in the event in an advisory role. Advisors will help advise event organizers on the supply chains that will be assigned to each group as well as answer questions during the exercise. Suggested staffing below:

-	Thomas Burke – co-host
-	Philip Heggelund – co-host
-	Frank Terzoli – WWF-US – US point of contact, upstream supply chain expertise
-	Carli Lloyd – Coordinator

## Schedule
The event will follow a 4-day schedule with a total combined time of 14 hours.

### Day 1 
*1 hour commitment.*
- 15 minutes of introductions
- 40 minute presentation discussing the GDST 1.0 standards, tools, and the supply chain scenarios.
-	15 minutes introducing the standards and event 
-	5-10 minutes for questions

Instructions for groups:
1.	Familiarize with the tools, sample data, scenarios, and communication streams
2.	Early Day 1 have joint meeting: contact info between groups, scenario planning
3.	Work from day 1-2 on scenario
4.	Produce conclusion presentations
5.	Show solution, discuss takeaways at the end

### Day 2 – 3
*12 hour commitment.*

These would be the core working days. Participants would commit 2 full working days for each of their participating members. For each day, two zoom meetings will be scheduled for each group, and each zoom meeting would be 3 hours long. This means that each group would be working together for a minimum of 12 hours through-out the exercise. Groups are welcome to commit as many hours as they want during these 2 days.

Prior to the exercise, Zoom meetings would have been scheduled for each group that best fits their working hours. This is to accommodate time zones and personal commitments.

During each 3 hour zoom meeting, event organizers and advisors will be available on Slack to answer any questions that a group might have. They could also arbitrarily join different Zoom meetings for groups to check in on their progress and provide feedback.

At the end of the 3rd day, each group would submit a presentation to the event organizers. Their presentation should answer the following questions:
1.	To what degree and how were you able to simulate the example supply chain?
2.	What are some key challenges encountered during the exercise?
3.	How did the group overcome these challenges?
4.	What are some improvements that could be made to the GDST standard and tools to help other businesses and solution providers in the future?

### Day 4
*2 hour commitment.*

This would be the final day in which each group would be given 15 minutes to present. They would have 5 minutes to present, and 10 minutes for questions. Depending on the number of groups, the meeting would last up to 2 hours. 

**Prentiation Element**
-	Define the technical workflow
    -	Utilize the XML files as examples
    -	Communication and standard protocols proposed
        -	Digital Link
        -	ASN
        -	EPCIS 2.0 REST
        -	OpenAPI
    -	Roadmap to implementation
    -	How would you use the GDST tools?
-	Scenario
-	Difficulties
-	Share with the XML that they were sharing (put in the dropbox)
-	Screenshots/demo 

## Communication Channels
We have gone ahead and setup both a Discord and a Slack channel available to be used by the groups. However, it is up to each team to determine which communication channels will work best for them.

### Discord
https://discord.gg/QaWFMEa6

*Discord is great since it has built-in voice channels.*

### Slack
**Group 1:** https://gdst-workspace.slack.com/archives/C01NSKVA230

**Group 2:** https://gdst-workspace.slack.com/archives/C01NSKW29AS

## Resources
- [Core Normative Standard](http://traceability-dialogue.org/wp-content/uploads/2020/03/2020.03.11_GDST1.0CoreNormativeStandardsfinalMAR13.pdf)
    - This is the standard documentation for the GDST standard. 
- [Technical Implementation Guide](http://traceability-dialogue.org/wp-content/uploads/2020/03/2020.03.11_GDST1.0TechnicalImplementationGuidancefinalMAR13.pdf)
    - This is a document that talks about more technical guidance around the GDST standard.
- [Developer Documentation](https://developer.traceability-dialogue.org/)
    - This is some additional documentation put together by the technical team to help developers adopt the GDST Standard.
- [Developer GitHub](https://github.com/ift-gftc/doc.gdst)
    - This is the GitHub that hosts the developer documentation.
- [Trawler Rest API GitHub](https://github.com/DuckScapePhilip/TrawlerAPI)
    - This is a GitHub that talks about how to access a temporary REST API to use the Trawler API that converts CSV data into EPCIS XML.
- [Trawler Source Code](https://github.com/ift-gftc/gftcms/tree/master/packages/trawler)
    - This is the source code to the Trawler Library that converts CSV into EPCIS XML. It is a Node Module.
- [IT Co-Mapping Tool](https://ift-gftc.github.io/IT-Conversion-Mapping-Tool/)
    - This is a micro-web application that allows you to use a diagram tool for laying out events and exporting them to EPCIS XML.
        
## Scenarios

### Group 1 - Farmed Shrimp
*WholeChain and Trace Register*

This is scenario that will follow shrimp being harvested from a farm in Ecuador. Then that shrimp will be sold to a processing plant in Ecuador, and finally the processed Shrimp will be sold to an Italian Importer. 

![Scenario 1 Image](https://i.ibb.co/VM0kzn5/Screenshot-2021-02-22-213255.png)

*(The arrows represent the flow of traceability data between the trading parties in the scenario.)*

This scenario involves a Farm, Processor, and Importer in the supply chain. The Event order will go as such:
1.	Farm Harvest – Shrimp is harvested at the Shrimp Farm
2.	Receive – Shrimp is sold from the farmer to the processing plant and received at the processing plant.
3.	Commingling – Shrimp is commingled with other received Shrimp from other Shrimp Farms.
4.	Processing – The shrimp is then peeled, put into cases, and frozen.
5.	Ship – The shrimp is sold to an Italian importer and shipped to them.
6.	Receive – The Italian Importer receives the shrimp.

#### Example XML
There is example XML for this scenario in the Group 1 folder of this GitHub. This XML can be uploaded to the IT-Co Mapping tool to visualize the event data.

### Group 2 - Wild Caught Tuna
*OpenSC, GoChain, and Plumensoft*

This scenario will follow Tuna being caught off the coast of California by several fisherman. That tuna is then sold to a Tuna Company in San Diego. That Tuna Company then will ship the tuna to a processor in Thailand for the Tuna to be processed into cans. The processed cans of tuna will then be shipped back to and imported by the Tuna Company in San Diego to be sold to retailers in the United States.

![Scenario 2 Image](https://i.ibb.co/vL1k5V3/Screenshot-2021-02-22-213642.png)

*(The arrows represent the flow of traceability data between the trading parties in the scenario.)*

This scenario involves a Vessel, Tuna Distributor, and Processor. The event order will go as such:
1.	Fishing Event – Tuna is fished up by the vessel off the coast of California.
2.	Offload – The tuna is sold to the Tuna Distributor at the port of San Diego
3.	Ship – The tuna is sold to the Processor in Thailand and shipped from San Diego to there.
4.	Receive – The tuna is received in Thailand.
5.	Processing – The tuna is processed by the processor in Thailand into cans of tuna.
6.	Ship – The tuna is sold back to the Tuna Distributor and shipped to them.
7.	Receive – The tuna is received by the Tuna Distributor.

#### Example XML
There is example XML for this scenario in the Group 2 folder of this GitHub. This XML can be uploaded to the IT-Co Mapping tool to visualize the event data.
