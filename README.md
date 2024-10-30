Dataset Description:
The dataset provides instances for solving the Periodic Capacitated Arc Routing Problem with Irregular Service (PCARP-IS) schedules. Each instance follows a specific format, described in detail below:

horizon: Defines the planning horizon in terms of the total number of periods.
nsubperiods: Specifies the number of subset of periods.

Each subset of periods is indexed (starting from 0) and lists the periods it contains.

nvertices: total number of vertices in the network.
nreq_links: number of required links, meaning links that must be served.
nnot_req_links: number of non-required links, meaning links that are optional for the routing.

Each link (i, j) is described by the following attributes:
Link type (edge or arc)
serv_cost (the service cost for visiting this link)
trav_cost (the travel cost for traversing this link)
demand
freq: A list specifying the required frequency of visits for some of the subbsets of periods.

For example:
(6,7) arc serv_cost 2 trav_cost 2 demand 65 freq: 0 1 3 2
This arc from vertex 6 to vertex 7 has a service cost of 2, a travel cost of 2, and a demand of 65. In subperiod 0, it requires 1 visit; in subperiod 3, it requires and 2 visits.

Non-required links (edges and arcs) are listed without service cost, demand, or frequency requirements.
