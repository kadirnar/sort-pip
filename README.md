<div align="center">
<h2>
  Sort-Pip: Packaged version of the Sort repository  
</h2>
<h4>
    <img width="500" alt="teaser" src="https://github.com/kadirnar/sort-pip/blob/05b7b968926a40324c7162041d875d6b53a02651/doc/sort_video.gif">
</h4>
<div>
    <a href="https://pepy.tech/project/sort-track"><img src="https://pepy.tech/badge/sort-track" alt="downloads"></a>
    <a href="https://badge.fury.io/py/sort-track"><img src="https://badge.fury.io/py/sort-track.svg" alt="pypi version"></a>
</div>
</div>

## <div align="center">Overview</div>

This repo is a packaged version of the [Sort](https://github.com/abewley/sort) algorithm.
### Installation
```
pip install sort-track
```

### Detection Model + Sort 
```python
from sort.tracker import SortTracker

tracker = SortTracker(args)
for image in images:
   dets = detector(image)
   online_targets = tracker.update(dets)
```

### Citation
```bibtex
@inproceedings{Bewley2016_sort,
  author={Bewley, Alex and Ge, Zongyuan and Ott, Lionel and Ramos, Fabio and Upcroft, Ben},
  booktitle={2016 IEEE International Conference on Image Processing (ICIP)},
  title={Simple online and realtime tracking},
  year={2016},
  pages={3464-3468},
  keywords={Benchmark testing;Complexity theory;Detectors;Kalman filters;Target tracking;Visualization;Computer Vision;Data Association;Detection;Multiple Object Tracking},
  doi={10.1109/ICIP.2016.7533003}
}
```
