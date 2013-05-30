Nei.ghbor.Net Keystone
======================

Keystone is one of the primary development focus' of the Nei.ghbor.Net team. The idea is to allow new nodes to peer to each other and set up location-based routing of content with a minimum of hassle. We've seeded this repo with nodeatlas (the hyperboria federated node-map) and a java geo-coordinate transformer from the NASA world-winds project. Until such time as the process is appropriately scriptified, this document shall serve as an explanation of the Keystone Geo-Routing Convention to be used by the Lightning API and Nei.ghbor.Net enabled apps.

Keystone Geo-Routing Convention
===============================

Nei.ghbor.Net prioritises locality as a primary-key for data transfer. By using MGRS (military grid reference system)  as prefixes to register CCN faces between Ground nodes, we can ensure that data requests for a specific area are routed to machines in that area.

For example:

Alice and Bob are early pioneers in the Nei.ghbor.Net project. They live far away from each other, but none the less they are closer to each other than any other nodes. 

Alices MGRS coordinates are AABB12345678

Bobs MGRS coordinates are AABB99995555

We convert these coordinates into A CCNX compatible prefix

Alice - /Nei.ghbor.Net/AA/BB/15/26/37/48

Bob - /Nei.ghbor.Net/AA/BB/95/95/95/95

We then find the smallest shared grid between these two coordinates, in this case: AA/BB/

So Alice and Bob register faces to each other at /Nei.ghbor.Net/AA/BB/

The shorter the prefix, the more of a 'backbone' the connection is serving as... in this case, alice and bob are the primary means that users are getting content within the /AA/BB scope.

These are very preliminary specifications of the Keystone convention. Any and all comments and questioned are welcome and solicited: email ryan@nei.ghbor.net with any input you have.




