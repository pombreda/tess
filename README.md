====
Tess

A Go port of [libtess.js](https://github.com/brendankenny/libtess.js).

===============
Developer Notes

- GluMesh.checkMesh -> GluMesh.Check
- Do not create types yourself! Use for example:
  - NewGluFace
  - NewGluVertex
  - NewGluHalfEdge
  - NewDictNode
- DictNode
  - getKey is just n.Key
  - getSuccessor is just n.Next
  - getPredecessor is just n.Prev

Left to port:

- `src/`
  - `normal.js`
  - `libtess.js`
  - `sweep.js`
  - `geom.js`
  - `tessmono.js`
  - `render.js`
  - `mesh.js`
  - `priorityq/`
    - `PQHandleElem.js`
    - `PriorityQ.js`
    - `PriorityQHeap.js`
    - `PQNode.js`
  - `mesh/`
    - `GluVertex.js`
    - `GluFace.js`
    - `GluHalfEdge.js`
    - `GluMesh.js`
  - `dict/`
    - `DictNode.js`
    - `Dict.js`
  - `libtess/`
    - `GluTesselator.js`
    - `CachedVertex.js`
  - `sweep/`
    - `ActiveRegion.js`
