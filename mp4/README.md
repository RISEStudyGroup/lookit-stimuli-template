# RISE Video Stimuli (MP4)

This folder contains MP4 video stimuli used in the current version of the **Remote Infant Studies of Early Learning (RISE)** battery called LRISE. 

Even though in the folder, the files are vaguely organized, the videos are organized below by experimental task. The folder also has other task supporting videos.

## CHS implementation - LRISE

The current CHS implementation contains eight experimental tasks presented in randomized order. For each task, one video is randomly selected from the available stimulus conditions, which vary by task.

The experimental videos are specified in the `available_videos` object of the CHS study code, with files loaded from the repository's `mp4/` or `webm/` directories.

## Video stimuli by task

### 1. Geo-Social Attention (`SocialPreference`)

Assessing infants' preference for social versus nonsocial stimuli by comparing looking time to videos of dancing children and moving geometric shapes.

**Used currently in LRISE:**

```text
GeoSocial_Aim2.mp4
```

### 2. Visual Paired Comparison (`VPC`)

Assessing visual recognition memory through infants' preference for novel versus familiar social (Faces) and nonsocial objects (Fribbles).

**Used currently in LRISE:**

```text
VPCV1_Aim2.mp4
VPCV2_Aim2.mp4
VPCV3_Aim2.mp4
VPCV4_Aim2.mp4
VPCV5_Aim2.mp4
VPCV6_Aim2.mp4
VPCV7_Aim2.mp4
VPCV8_Aim2.mp4
```

### 3. Prediction (`Prediction`)

Examining infants' ability to learn visual patterns, anticipate the location of upcoming stimuli, and update predictions when the location changes.

**Used currently in LRISE:**

```text
PredictionTargetLthenR_Aim2.mp4
PredictionTargetRthenL_Aim2.mp4
```

These two conditions counterbalance the initial target location and subsequent location change.


### 4. Audiovisual Synchrony (`AVSynchrony`)

Assessing infants' sensitivity to audiovisual alignment by comparing looking time to synchronous and asynchronous speech videos.

**Used currently in LRISE:**

```text
LRISE_AVSynch_Short_AthenS.mp4
LRISE_AVSynch_Short_SthenA.mp4
```

These videos counterbalance the order of asynchronous and synchronous stimulus presentations.

### 5. Word Comprehension (`word-recognition`)

Assessing infants' real-time comprehension of familiar words using a looking-while-listening task with named target and distractor images.

**Used currently in LRISE:**

```text
2026_10_05_word_recognition_LRISE.mp4
```

### 6. Social Evaluation (`helpers`)

Examining infants' preference for prosocial versus antisocial agents after observing animated helping and hindering events.

**Used currently in LRISE:**

```text
2026_10_05_Condition1_LRISE.mp4
2026_10_05_Condition2_LRISE.mp4
2026_10_05_Condition3_LRISE.mp4
2026_10_05_Condition4_LRISE.mp4
```

### 7. Numeracy (`numeracy`)

Assessing infants' sensitivity to changes in nonsymbolic numerical quantities by comparing looking time to constant versus alternating streams of dots.

**Used currently in LRISE:**

```text
Numeracy5cl1.mp4
Numeracy5cr1.mp4
Numeracy20cl1.mp4
Numeracy20cr1.mp4
```

The conditions vary the constant numerical quantity (5 or 20 dots) and the side on which the constant stream appears.


### 8. Speech Discrimination (`SpeechDiscrimination`)

Assessing infants' sensitivity to differences between speech sounds, including phonetic contrasts relevant to their language experience.

**Used currently in LRISE:**

```text
speechdisc_lrise_condition_1.mp4
speechdisc_lrise_condition_2.mp4
speechdisc_lrise_condition_3.mp4
speechdisc_lrise_condition_4.mp4
speechdisc_lrise_condition_5.mp4
speechdisc_lrise_condition_6.mp4
speechdisc_lrise_condition_7.mp4
speechdisc_lrise_condition_8.mp4
speechdisc_lrise_condition_9.mp4
speechdisc_lrise_condition_10.mp4
speechdisc_lrise_condition_11.mp4
speechdisc_lrise_condition_12.mp4
```

The CHS implementation randomly selects one of these twelve experimental conditions.


## Supporting videos

In addition to the experimental task videos, this folder contains supporting media for the study setup, calibration, and presentation.

```text
intro_vid.mp4
Calibration_Movie.mp4
sample_video.mp4
a_size.mp4 through p_size.mp4
```

- `intro_vid.mp4`: Introduction video presented before the experimental tasks.
- `Calibration_Movie.mp4`: Calibration video used before task presentation.
- `sample_video.mp4`: Sample video file from CHS.
- `a_size.mp4` through `p_size.mp4`: Additional files for sizing.


### CHS video configuration

Experimental videos are loaded using the following configuration:

```javascript
{
    "kind": "exp-lookit-video",
    "video": {
        "position": "fill",
        "source": pop_random(available_videos[trial_name])
    },
    "backgroundColor": "white",
    "autoProceed": true,
    "doRecording": true,
    "frameOffsetAfterPause": 1,
    "baseDir": "https://raw.githubusercontent.com/RISEStudyGroup/lookit-stimuli-template/master/",
    "videoTypes": ["webm", "mp4"]
}
```

The base directory points to the RISE stimulus repository.
