# twitch-graph

## Overview

This project is the italian version of [Visualizing Twitch Communities](https://github.com/KiranGershenfeld/VisualizingTwitchCommunities) by [KiranGershenfeld](https://github.com/KiranGershenfeld).

The project's aim is to map communities of streamers on Twitch.tv based on shared viewership. The data is collected from the Twitch API and visualized in Gephi. The complete graph can be viewed at [https://cinci-git.github.io/twitch-graph/](https://cinci-git.github.io/twitch-graph/).

## Data

The data_collection folder has a script called main that can be ran to collect (at least) the top 100 streams in italian language and all their viewers and save the data in a json file. To collect the data I ran the script every 15 minutes from 17/07/2022 to 15/08/2022. 

## Graph

The graph is made using Gephi and the website using [gexf-js](https://github.com/raphv/gexf-js).

The nodes of the graph are streamers and their size is the amount of unique viewers that visited that channel. The edges represent the shared viewers of two channels. To make the graph I considered only the users that watched a channel  for at least 2 hours. I removed the users detected for more than 350 hours, since they are probably bots (however they were only the 0.6% of the total).

## License
[MIT](https://choosealicense.com/licenses/mit/)

