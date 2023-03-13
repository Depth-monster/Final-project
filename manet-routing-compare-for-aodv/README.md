# Scenario parameters:

<ul>
  <li>Number of nodes: 50</li>
<li>Number of sinks: 10</li>
<li>Mobility Model: RandomWaypointMobilityModel** </li>
<li>Propagation Model: ConstantSpeedPropagationDelay</li>
<li>Propagation Loss Model: Friis</li>
<li>Mac: AdhocWifiMac</li>
<li>Mac Standard: 802.11b</li>
<li>Bps: 2Kbps</li>
<li>Total Simualtion Time: 200 seconds</li>
<li>Node speed: 20 m/s</li>
<li>Node pause time: 0</li>
<li>Protocol: Ad-hoc On-demand Distance Vector protocol</li>
</ul>

<hr/>


## What to do?
#### After running a file .cc above, you will get next files: 

AODV.csv

AODV.flowmon

AODV.mob

![image](https://user-images.githubusercontent.com/122405130/224842451-d7704a45-ad88-4ca0-a4dd-c635571c26e7.png)

For saving outputs from terminal you can use the next command:

./ns3 run scratch/manet-routing-compare &> temp.data

![image](https://user-images.githubusercontent.com/122405130/224842757-d8f93835-8ecc-4a03-8d43-3af358d23b9c.png)

![image](https://user-images.githubusercontent.com/122405130/224843120-88d5ddb6-ef6a-46df-8742-d003ebfdc989.png)


## For output statistics use flow.py script in this repository and output characteristics:
### use the command: ![image](https://user-images.githubusercontent.com/122405130/224851787-b6941a0b-7a45-4fe7-8ec5-5be7c6097943.png)

![image](https://user-images.githubusercontent.com/122405130/224851600-721ed9f0-d491-453c-adfb-dd8f17c91228.png)


## Now we have to output graph that retrieves from AODV.csv file Receive Rate & Packets Received statistics
Fristly we remove commas from out AODV.csv file for using it with gnuplot
![image](https://user-images.githubusercontent.com/122405130/224854479-bbd8cde3-f7e0-4b00-98b2-770e6ce9ecc6.png)
![image](https://user-images.githubusercontent.com/122405130/224854540-ed45522d-7473-41a9-9a89-d4e8e46afb43.png)
#### we plot graph with gnuplot by running the command:
![image](https://user-images.githubusercontent.com/122405130/224854580-827fe19f-8c8d-4ee6-9e19-e6625dec2b2e.png)

Gnuplot scripts are also available in this repo

### Now we got this beautiful graph(simulation starts after 100'th second)
![image](https://user-images.githubusercontent.com/122405130/224854767-7ec59281-f5de-453c-9b7e-3f167e005d2e.png)

<!--
[Duck Duck Go](https://duckduckgo.com "The best search engine for privacy")

<https://www.markdownguide.org>
<fake@example.com>


I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).



-->

