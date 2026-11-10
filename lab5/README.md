# Lab 5 – Shape from BufferGeometry

For this lab, I created a 3D crystal using Three.js BufferGeometry.

The crystal has **6 vertices and 8 triangular faces**. I used an indexed geometry, where the vertices are defined in a Float32Array and the faces are created using indices.

I used `computeVertexNormals()` to calculate smooth vertex normals. I also created a non-indexed version of the geometry to compare the shading. By pressing **F**, I can switch between the two versions.

The crystal rotates automatically, and OrbitControls allows me to view it from different angles.

The order of the indices is important because it determines the direction of each face. If the order is incorrect, some faces may point inward and become invisible when back-face culling is enabled.