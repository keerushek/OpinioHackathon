# OpinioHackathon
This is the repo of the submission for the hackathon conducted by opinio
Problem statement selected is "Logistics in India"

The challenges that will be solved using our solution will be:
1.locating customer addresses
2.routing and sequencing
3.capacity utilization

Nobody knows the neighbourhood better than you. Why not help the person delivering your package much quicker.

The customer once is done with checkout of the products brought on the application. A Popup is shown with "Know a Shortcut SHARE IT".

This will allow the user to add nodes from the source to destination on a map shown on the application. These nodes can be used to reach the destination from the source, this path can be different from the one suggested by googlemaps or can be the same. 

If in case this path provides a faster and shorter path to the destination then the customer will be given an incentive for helping the app. Eg: 5% off on the next 5 deliveries. The delivery person can also upvote this path to give more weightage for the shortcut provided.

These orders which have nodes provided will be stored in the backend. When the next source-destination is provided from the application from a different user, algorithms will be used to check if source-destination combo are closer to any of previous orders. 

If yes, using the nodes provided by the previous user the path is generated to check if it is better than the path provided by google maps for source-destination. Dijkstra's Algorithm can be used to optimise this.

If No, then all the nodes available close to the source are taken and then checked if the destination is closer from the immediate next node. Using DFS or BFS this can be solved.

