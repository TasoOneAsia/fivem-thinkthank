# Player Manager

General player instantiation and management will occur here. Experimenting with APIs capable of returning
several different data structures depending on the needs of the caller could be pretty cool here.

Also as this will be inherently state oriented (therefore DB oriented), having them in the same resource
would reduce the downsides of serialization and general event overhead.