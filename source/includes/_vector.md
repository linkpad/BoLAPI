# Vector Functions

## VectorType

* Return if as vector

`VectorType(v)`

## VectorIntersection

* Return the Intersection of 2 lines

`VectorIntersection(a1,b1,a2,b2)`

## IsLineSegmentIntersection

* Return if 2 linesegments intersect

`IsLineSegmentIntersection(A,B,C,D)`

## LineSegmentIntersection

* Return the Intersection of 2 linesegments

`LineSegmentIntersection(A,B,C,D)`

## VectorDirection

`VectorDirection(v1,v2,v)`

## VectorPointProjectionOnLine

* Return a vector on line v1-v2 closest to v

`VectorPointProjectionOnLine(v1, v2, v)`

## Vector

* Return a vector from x,y,z pos or from another vector

`Vector(a,b,c)`


# Vector Methods

## vector:clone

* Return a new Vector from vector

`vector:clone()`

## vector:unpack

`vector:unpack()`

## vector:len2

* Return vector^2

`vector:len2()`

* Return vector^v

`vector:len2(v)`

## vector:len

* Return vector length

`vector:len()`

## vector:dist

* distance between 2 vectors (v and vector)

`vector:dist(v)`

## vector:normalize

* Normalize vector

`vector:normalize()`

## vector:normalized

* return a new Vector normalize from vector

`vector:normalized()`

## vector:rotate

* Rotate the vector by phi angle

`vector:rotate(phiX, phiY, phiZ)`

## vector:rotated

* Return a new Vector rotate from vector by phi angle

`vector:rotated(phiX, phiY, phiZ)`

## vector:projectOn

* Return a new Vector from vector projected on v

`vector:projectOn(v)`

## vector:mirrorOn

* Return a new Vector from vector mirrored on v

`vector:mirrorOn(v)`

## vector:center

* Return center between vector and v

`vector:center(v)`

## vector:crossP

* Return cross product of vector

`vector:crossP()`

## vector:dotP

* Return dot product of vector

`vector:dotP()`

## vector:polar

* Return the angle from axe

`vector:polar()`

## vector:angleBetween

* Return the angle formed from vector to v1,v2

`vector:angleBetween(v1, v2)`

## vector:compare

* Compare vector and v

`vector:compare(v)`

## vector:perpendicular

* Return new Vector rotated 90° right

`vector:perpendicular()`

## vector:perpendicular2

* Return new Vector rotated 90° left

`vector:perpendicular2()`