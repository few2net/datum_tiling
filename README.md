# datum_tiling
This repository resolves the MultiPolygon issue that occurred during segmentation when the intersection between the ROI and the annotation resulted in a MultiPolygon.

Original source: [link](https://open-edge-platform.github.io/datumaro/stable/_modules/datumaro/plugins/tiling/tile.html#Tile)

Tutorial: [link](https://open-edge-platform.github.io/datumaro/stable/docs/jupyter_notebook_examples/notebooks/06_tiling.html)



## Usage

```python
from tile import Tile

tiled_dataset = dataset.transform(
    Tile, grid_size=(2, 2), overlap=(0.1, 0.1), threshold_drop_ann=0.3
)
```
