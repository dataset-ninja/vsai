The authors of the **VSAI** dataset highlight the significance of arbitrary-oriented vehicle detection using aerial imagery in remote sensing and computer vision applications, such as traffic management, disaster monitoring, and smart cities. While object detection in natural imagery has advanced considerably in the past decade, the progress has been slower for airborne imagery due to factors like variations, appearances, and limited availability of high-quality aerial datasets that reflect real-world complexities. To address these challenges and enhance object detection research in remote sensing, the authors curated a multi-view dataset for **vehicle** detection in complex **scenarios** using **aerial images** (VSAI). This dataset encompasses arbitrary-oriented views in aerial imagery, covering diverse real-world scenes captured using different drone platforms.

The VSAI dataset comprises 49,712 annotated vehicle instances, including oriented bounding boxes and arbitrary quadrilateral bounding boxes. This encompasses 47,519 small vehicles and 2,193 large vehicles. In addition to the object annotations, the occlusion rate of objects was annotated to improve the generalization capabilities of object detection networks.

The authors compare conventional datasets with those collected by camera-equipped drones, highlighting the broad applications of the latter in fields like agriculture, disaster monitoring, traffic management, and military reconnaissance. Unlike natural datasets where objects are usually oriented upward due to gravity, aerial images under oblique views exhibit instances with arbitrary directions, influenced by the drone's view and scale transformation.

They outline the unique challenges of object detection in aerial imagery, including large size variations of instances, degraded images due to flight limitations and weather variations, presence of many small instances, unbalanced object density, and arbitrary orientations. The authors also acknowledge dataset bias and the need for a dataset that reflects real-world complexity to enhance the generalization ability of object detection networks.

Furthermore, the authors emphasize the significance of identifying objects using multi-view (off-nadir) imagery from drones, particularly in applications like disaster monitoring, emergency rescue, and environmental reconnaissance.

|    Version    |    CMOS    | Field Angle |  Resolution  |
| :-----------: | :--------: | :---------: | :----------: |
|   Mavic air   | 1/2.3 inch |    85°    | 4056 × 3040 |
|  Mavic 2 pro  |   1 inch   |    77°    | 5472 × 3648 |
| Phantom 3 Pro | 1/2.3 inch |    94°    | 4000 × 3000 |
|   Phantom 4   | 1/2.3 inch |    94°    | 4000 × 3000 |
| Phantom 4 RTK |   1 inch   |    84°    | 5472 × 3648 |

The VSAI dataset comprises 444 static images collected from various drone platforms, including DJI Mavic Air, DJI Mavic 2 Pro, Phantom 3 Pro, Phantom 4, and 4 RTK. The dataset covers a wide range of technical parameters and was collected from various Chinese cities to ensure geographic diversity. Images were captured throughout the year, under various weather and lighting conditions, focusing on small vehicles (e.g., cars, minibuses, pickups) and large vehicles (e.g., buses, large trucks). The dataset aims to address the uneven distribution of vehicles in real-world scenarios.

In the VSAI dataset, the instances with line of sight (LOS) angles of (−30°, −25°) were the largest. Overall, the LOS angle distribution of the number of instances was not balanced, mainly concentrating on small observation angles in the range of (−45°, −15°).

<img src="https://github.com/supervisely/supervisely/assets/78355358/cdef1a6a-fdc1-4abf-b2f6-32c096d3bd32" alt="image" width="200">


VSAI covers six complicated scenes throughout China, including the desert, city, mountain, suburb, riverside, and seaside. The six scenarios also contain many subsets, such as cities, including the overhead bridge, crossroad, stadium, riverside embracing dam, bridge, etc. 

<img src="https://github.com/supervisely/supervisely/assets/78355358/b05bab64-bfd1-4951-8b57-0d71b36d9d07" alt="image" width="400">

The authors also collected statistical information about the vehicles, including the vehicle’s orientation angles, instance length, and vehicle aspect ratio. Thus, the lengths of the vehicles were concentrated in the range of 0 to 75 pixels, signifying that there were numerous small instances in the VSAI dataset. At the same time, there was a considerable scale change in VSAI. In addition, distinct perspectives also resulted in a wider range of the vehicle aspect ratio rather than the aspect ratio of 2 or so in traditional down-view aerial images.

<img src="https://github.com/supervisely/supervisely/assets/78355358/5eb53703-ceaa-490f-990b-749ebc8cd1d8" alt="image" width="1200">


Additionally, VSAI provides useful annotations with respect to the occlusion ratio. In this case, the proportion of vehicles being blocked to represent the occlusion ratio and define four levels of occlusions: no occlusion **N** (occlusion ratio 0%), small occlusion **S** (occlusion ratio < 30%), moderate occlusion **M** (occlusion ratio 30~70%), and large occlusion **L** (occlusion ratio > 70%), mainly for better reflecting the instance density of the instance location.

<img src="https://github.com/supervisely/supervisely/assets/78355358/346818b4-511c-4573-afba-9232ba2ed48d" alt="image" width="400">