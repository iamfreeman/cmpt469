Overview
The Composite tile format enables concatenating tiles of different formats into one tile.

3D Tiles and the Composite tile allow flexibility for streaming heterogeneous datasets. For example, buildings and trees could be stored either in two separate Batched 3D Model and Instanced 3D Model tiles or, using a Composite tile, the tiles can be combined.

Supporting heterogeneous datasets with both inter-tile (separate tiles of different formats that are in the same tileset) and intra-tile (different tile formats that are in the same Composite tile) options allows conversion tools to make trade-offs between number of requests, optimal type-specific subdivision, and how visible/hidden layers are streamed.

A Composite is a binary blob in little endian accessed in JavaScript as an ArrayBuffer.
