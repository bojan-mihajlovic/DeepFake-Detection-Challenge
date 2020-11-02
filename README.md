# DeepFake-Detection-Challenge
Kaggle - DeepFake Detection Challenge - Bronze Medal Solution

This competition is closed for submissions. Participants' selected code submissions were re-run by the host on a privately-held test set and the private leaderboard results have been finalized. Late submissions will not be opened, due to an inability to replicate the unique design of this competition.

Deepfake techniques, which present realistic AI-generated videos of people doing and saying fictional things, have the potential to have a significant impact on how people determine the legitimacy of information presented online. These content generation and modification technologies may affect the quality of public discourse and the safeguarding of human rights—especially given that deepfakes may be used maliciously as a source of misinformation, manipulation, harassment, and persuasion. Identifying manipulated media is a technically demanding and rapidly evolving challenge that requires collaborations across the entire tech industry and beyond.

AWS, Facebook, Microsoft, the Partnership on AI’s Media Integrity Steering Committee, and academics have come together to build the Deepfake Detection Challenge (DFDC). The goal of the challenge is to spur researchers around the world to build innovative new technologies that can help detect deepfakes and manipulated media.

Challenge participants must submit their code into a black box environment for testing. Participants will have the option to make their submission open or closed when accepting the prize. Open proposals will be eligible for challenge prizes as long as they abide by the open source licensing terms. Closed proposals will be proprietary and not be eligible to accept the prizes. Regardless of which track is chosen, all submissions will be evaluated in the same way. Results will be shown on the leaderboard.

The PAI Steering Committee has emphasized the need to ensure that all technical efforts incorporate attention to how the resulting code and products based on it can be made as accessible and useful as possible to key frontline defenders of information quality such as journalists and civic leaders around the world. The DFDC results will be a contribution to this effort and building a robust response to the emergent threat deepfakes pose globally.

## Data

**Training Set**

This code competition's training set is not available directly on Kaggle, as its size is prohibitively large to train in Kaggle. Instead, it's strongly recommended that you train offline and load the externally trained model as an external dataset into Kaggle Notebooks to perform inference on the Test Set. Review Getting Started for more detailed information.

The full training set is just over 470 GB. We've made it available as one giant file, as well as 50 smaller files, each ~10 GB in size. You must accept the competition's rules to gain access to any of the links below.

A small sample training set has been made available below.

You'll also need the sample_submission.csv, as it indicates the IDs you'll be making predictions for.

What should I expect the data format to be?

The data is comprised of **.mp4** files, split into compressed sets of ~10GB apiece. A **metadata.json** accompanies each set of **.mp4** files, and contains filename, label (REAL/FAKE), original and split columns, listed below under Columns.

What am I predicting?

You will be predicting whether or not a particular video is a deepfake. A deepfake could be either a face or voice swap (or both). In the training data, this is denoted by the string "REAL" or "FAKE" in the label column. In your submission, you will predict the probability that the video is a fake.

## Files

**train_sample_videos.zip** - a ZIP file containing a sample set of training videos and a metadata.json with labels. the full set of training videos is available through the links provided above.
**sample_submission.csv** - a sample submission file in the correct format.
**test_videos.zip** - a zip file containing a small set of videos to be used as a public validation set.
To understand the datasets available for this competition, review the Getting Started information.

## Columns

filename - the filename of the video
label - whether the video is REAL or FAKE
original - in the case that a train set video is FAKE, the original video is listed here
split - this is always equal to "train".
