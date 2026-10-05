# Lab 18 — Submission

Notebook source: https://github.com/vuog23/Track04-Day18-2D-perception-detection-segmentation-keypoints/blob/main/lab_2d_perception_student.ipynb

## Run summary

- Device: CUDA; YOLO26n-pose training: 40 epochs at 640 px.
- Pose mAP50: 0.9950; pose mAP50-95: 0.4357; training time: 3.8 minutes.
- Q11 was completed from the six worst validation examples: paw keypoints, especially front paws, have the largest errors; overlapping or occluded legs make left/right localization harder. Suggested fixes are more diverse crossed-leg examples, checked left/right labels, and high-resolution paw crops.
- Bonus 4C results and interpretation: `bonus_4c.md`.

## Files

- `ket_qua.json`: run metrics, progress checks, and Q1–Q12 answers.
- `autolabel/bus.txt`: SAM-generated YOLO-seg labels.
- `bonus_4c.md`: original and mirrored validation comparison.
- `evidence/`: the six worst validation examples and per-keypoint error chart used for Q11.
