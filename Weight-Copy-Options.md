When you **copy bone weights** in Outfit Studio, an options dialog pops up. It looks like the following.

![Weight Copy Options](http://i.imgur.com/bMV8lXi.png)

As the description in the dialog mentions, every single vertex of the source will **spread its bone weights to the maximum amount of vertices** in the target that you set it to, provided they are within the search radius.

In this amazingly painted example, the green circle is the source vertex, the red circles are all of the target vertices and the radius is shown in blue.

![Search Radius](http://i.imgur.com/q2yXsIk.png)

There are **5 vertices within the search radius**, but with a maximum of 4 vertex targets, **only 4 of them will receive weights** from that one source. Of course, they can and will still receive weights from other sources.

All of the weights received will be averaged out with a maximum of 4 different bones that can affect a single vertex.