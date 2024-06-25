# The Perceived Intensity of Facial Expressions Dataset

This repository contains the human annotation data for the PIFE dataset.

## Contents

* human_annotation_videos_with_AUs.csv

  The human annotation data for the videos in the dataset, along with the AU values detected by OpenFace.

* human_annotation_images_with_AUs.csv

  The human annotation data for the images in the dataset, along with the AU values detected by OpenFace.

## Data format

### human_annotation_images_with_AUs.csv

| Field            | Explanation                                                                              |
| ---------------- | ---------------------------------------------------------------------------------------- |
| frame            | The number of the frame extracted from the movie                                         |
| movie            | The name of the movie followed by AM or HM for artistic or hollywood movies respectively |
| face_id          | The Face ID assigned by OpenFace                                                         |
| AU*##*_r         | The value of each action unit as detected by OpenFace                                    |
| sum              | The sum of the AU values                                                                 |
| exp_sum          | The exponent of the sum?                                                                 |
| image            | The image of the extracted frame                                                         |
| intensity*n*     | The intensity assigned by annotator *n*                                                  |
| intensity_mean   | The mean of intensities assigned by the annotators                                       |
| intensity_sd     | The standard deviation of the intensities assigned by the annotators                     |
| annot_group      | The group the annotators were assigned to                                                                                                                     |
| movie_type       | *A* for artistic movies, or *H* for Hollywood movies                                     |

### human_annotation_videos_with_AUs.csv

| Field            | Explanation                                                                              |
| ---------------- | ---------------------------------------------------------------------------------------- |
| movie            | The name of the movie                                                                    |
| frame_start      | The first frame of the segment extracted from the movie                                  |
| face_id          | The Face ID assigned by OpenFace                                                         |
| timestamp        | The start time of the segment in seconds                                                 |
| AU##_r           | The value of each action unit as detected by OpenFace                                    |
| exp_sum          | The exponent of the sum?                                                                 |
| sum              | The sum of the AU values                                                                 |
| annot_group      | The group the annotators were assigned to                                                |
| frame_start      | The first frame of the segment                                                           |
| intensity*n*     | The intensity assigned by annotator *n*                                                  |
| intensity_mean   | The mean of intensities assigned by the annotators                                       |
| intensity_sd     | The standard deviation of the intensities assigned by the annotators                     |
| variability*n*   | The variability assigned by annotator *n*                                                |
| variability_mean | The mean of the variabilities assigned by the annotator                                  |
| variability_sd   | The standard deviation of the variabilties asssigned by the annotators                   |
| frame_end        | The number of the last frame in the extracted segment                                    |
