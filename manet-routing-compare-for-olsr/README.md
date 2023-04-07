
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
<li>Protocol: OLSR protocol</li>
</ul>

<hr/>


## What to do?
#### After running a file .cc above, you will get next files: 

OLSR.csv

OlSR.flowmon

OLSR.mob

![image](https://user-images.githubusercontent.com/122405130/230540258-1d032177-a344-4d22-9e6f-f405d91fc67f.png)


For saving outputs from terminal you can use the next command:
```cpp
./ns3 run scratch/manet-routing-compare &> temp.data
```

![image](https://user-images.githubusercontent.com/122405130/224842757-d8f93835-8ecc-4a03-8d43-3af358d23b9c.png)

![image](https://user-images.githubusercontent.com/122405130/224843120-88d5ddb6-ef6a-46df-8742-d003ebfdc989.png)


## For output statistics use flow.py script in this repository and output characteristics:

### use the command: 
```python
python flow.py OLSR.flowmon
 ```
![image](https://user-images.githubusercontent.com/122405130/230541112-5d39df08-e7a4-41c8-9212-60ebe9a6aa23.png)



## Now we have to output graph that retrieves from AODV.csv file Receive Rate & Packets Received statistics

Fristly we remove commas from out OLSR.csv file for using it with gnuplot

![image](https://user-images.githubusercontent.com/122405130/224854479-bbd8cde3-f7e0-4b00-98b2-770e6ce9ecc6.png)
![image](https://user-images.githubusercontent.com/122405130/224855248-c6c75f16-8d5d-4383-94c9-8590de1e0009.png)
#### we plot graph with gnuplot by running the command:
```gnu
gnuplot gnuplot.code
```
![image](https://user-images.githubusercontent.com/122405130/224854580-827fe19f-8c8d-4ee6-9e19-e6625dec2b2e.png)

Gnuplot scripts are also available in this repo

### Now we got this beautiful graph(simulation starts after 100'th second)
![image](https://user-images.githubusercontent.com/122405130/224858052-3afde8fc-27e5-4e62-b0fc-f7f4ec6c2905.png)
<!--
[Duck Duck Go](https://duckduckgo.com "The best search engine for privacy")

<https://www.markdownguide.org>
<fake@example.com>


I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#code).



-->

