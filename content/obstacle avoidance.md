aUToronto onboarding activity:
write an obstacle avoidance algorithm
```
#include <cstdint>
#include <iostream>
#include <vector>
#include <tuple>
#include <cassert>
#include <list>
#include <algorithm>
using namespace std;

/*
Assume our self-driving car is travelling with some constant velocity in the X-Y plane (so the car's Z/altitude is not changing) and assume that have a prediction algorithm that 
produces several predicted bounding boxes for each static obstacle in our way.
Assume that we know the ground truth position of static obstacles and that the predictions are provided to you. Also assume that bounding boxes for all obstacles and predictions are X,Y,Z axes aligned.

REQUIREMENTS:
- We want to be able to identify the best bounding box prediction for each obstacle object using IoU as the metric of good-ness. 
Intersection over Union (IoU) = Area of Overlap / Area of Union

- Additionally, we want to evaluate the performance of our predictor using the F1-score. 
F1 = (2*Precision*Recall) / (Precision + Recall)
(Hint: our predictor is not perfect, it is possible for some predictions to be produced for obstacles that dont actually exist, and some obstacles that exist may not have any predictions made for them.
Use the IoU threshold to determine prediction associations with ground truth labels.)

Complete the functions below the achieve the above requirements, you may use as many additional helper functions as you like.
Feel free to generate some actual ground truth labels + predictions in main() to test your code to ensure it achieves the requirements.
State any assumptions you've made if you are unclear about anything and to explain your rationale.
*/

struct Center{
  double x;
  double y;
  double z; 
};

struct Dimensions{
  double w;
  double l;
  double h;
};

struct Velocity{
  double vx;
  double vy;
};

struct BoundingBox{
  Center center;
  Dimensions dimensions;
};

struct Label{
  BoundingBox bounding_box;
  uint64_t id;
};

struct Labels{
  vector<Label> labels;
  uint64_t timestamp;
};

struct Prediction{
  BoundingBox bounding_box;
  Velocity velocity;
  uint64_t timestamp;
  double confidence;
};

class Predictions {
  public:
    Predictions(const vector<Prediction>& predictions) : predictions_{predictions} {}

    vector<Prediction> predictions_;

    void ExtrapolatePredictions(uint64_t timestamp){
      // Write code here to extrapolate the predictions to the given timestamp since our car is moving while making predictions.

    }
};

double compute_overlap_area(const BoundingBox& box_one, const BoundingBox& box_two)
{
  // Compute overlap area between two boxes given as bounding boxes
  
}

double compute_union_area(BoundingBox& box_one, BoundingBox& box_two, double overlap_area)
{
  // Compute the union area for IoU criteria using calculated overlap area from before

}

std::tuple<double, double> ComputePrecisionRecall(const Labels& labels, const Predictions& predictions, double threshold = 0.5){
  // Return the computed precision-recall values here.
  // Feel free to make as many helper functions as you need.


}

int main() {


}

```


# Task breakdown
assumptions
- constant velocity in a plane
- assume there is already a prediction algorithm that produces bounding boxes for every static obstacle in the cars path
- assume you know the coordinates of the static obstacles
- and that you already have the predictions

### requirements
- identify the best bounding box prediction of each obstacle
- use [[IoU (intersection over union)]]
- 