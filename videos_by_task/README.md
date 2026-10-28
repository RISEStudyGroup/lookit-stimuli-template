# RISE Videos by Task

This folder contains experimental video stimuli for the **Remote Infant Studies of Early Learning (RISE)** battery, organized by developmental task and then by the study version.

There have been 3 three study versions:

- **Aim1:** Original RISE pilot study stimuli (see Tenenbaum et al., 2025).
- **Aim2:** Stimuli used in the expanded RISE battery, including modifications to selected tasks.
- **LRISE:** Stimuli developed or retained for the following LRISE, including 1 additional task.

Some stimuli are shared between Aim 2 and LRISE and are stored in combined folders named `Aim2_and_LRISE` under the task.

**Current CHS stimuli** identifies the files used in the LRISE implementation on CHS as of **10/16/2026**


## Repo structure

```text
videos_by_task/
├── AVSynchrony/
│   ├── Aim1/
│   ├── Aim2/
│   └── LRISE/
├── Helpers/
│   ├── Aim1/
│   ├── Aim2/
│   └── LRISE/
├── Numeracy/
│   ├── Aim1/
│   ├── Aim2/
│   └── LRISE/
├── Prediction/
│   ├── Aim1/
│   └── Aim2_and_LRISE/
├── SocialPreference/
│   ├── Aim1/
│   └── Aim2_and_LRISE/
├── SpeechDiscrimination-LRISE/
│   ├── LRISE_v1/
│   └── LRISE_v2/
├── VPC/
│   ├── Aim1/
│   └── Aim2_and_LRISE/
├── word_recognition/
│   ├── Aim1/
│   ├── Aim2/
│   └── LRISE/
└── README.md
```

## Experimental tasks and stimuli

### 1. Geo-Social Attention (`SocialPreference/`)

Assesses infants' preference for social versus nonsocial stimuli by comparing looking time to videos of dancing children and moving geometric shapes.

**Based on:** Pierce et al. (2016); Chawarska et al. (2016).

```text
SocialPreference/
├── Aim1/
│   └── GeoSocial_Aim1.mp4
└── Aim2_and_LRISE/
    └── GeoSocial_Aim2.mp4
```

The Aim 2 version includes modifications to the social and geometric stimuli, including closer views of children's faces and reduced color saturation of geometric shapes.

**Current CHS stimulus:** `GeoSocial_Aim2.mp4`

### 2. Visual Paired Comparison (`VPC/`)

Assesses visual recognition memory through infants' preference for novel versus familiar social (Faces) and nonsocial objects (Fribbles).

**Based on:** Manns et al. (2000); Barry et al. (2014).

```text
VPC/
├── Aim1/
│   └── VPCV1_Aim1.mp4 through VPCV8_Aim1.mp4
└── Aim2_and_LRISE/
    └── VPCV1_Aim2.mp4 through VPCV8_Aim2.mp4
```

The task includes multiple stimulus versions used to counterbalance experimental presentations.

**Current CHS stimuli:** `VPCV1_Aim2.mp4` through `VPCV8_Aim2.mp4`

### 3. Prediction (`Prediction/`)

Examines infants' ability to learn visual patterns, anticipate the location of upcoming stimuli, and update predictions when the location changes.

**Based on:** Reuter et al. (2018).

```text
Prediction/
├── Aim1/
│   ├── PredictionTarget_LthenR_Aim1.mp4
│   └── PredictionTarget_RthenL_Aim1.mp4
└── Aim2_and_LRISE/
    ├── PredictionTargetLthenR_Aim2.mp4
    └── PredictionTargetRthenL_Aim2.mp4
```

The two conditions counterbalance the starting location of the visual target before it switches to the opposite side of the screen.

**Current CHS stimuli:** Both videos in `Aim2_and_LRISE/`.

### 4. Audiovisual Synchrony (`AVSynchrony/`)

Assesses infants' sensitivity to audiovisual alignment by comparing looking time to synchronous and asynchronous speech videos.

**Based on:** Righi et al. (2018); Tenenbaum et al. (2015).

```text
AVSynchrony/
├── Aim1/
│   └── AudioVisual_Aim1.mp4
├── Aim2/
│   ├── AudioVisual_1000_Aim2.mp4
│   └── AVSynch_1000_Aim2.mp4
└── LRISE/
    ├── AudioVisual_Multi_0_66-LRISE.mp4
    └── AudioVisual_Multi_66_0-LRISE.mp4
```

The Aim 2 version increased the audiovisual delay from 666 ms to 1000 ms to increase the perceptual distinction between synchronous and asynchronous stimuli.

**Current CHS stimuli:** `LRISE_AVSynch_Short_AthenS.mp4` and `LRISE_AVSynch_Short_SthenA.mp4`, located in the main `mp4/` folder. These filenames differ from those in `AVSynchrony/LRISE/` but are the same files.

### 5. Word Comprehension (`word_recognition/`)

Assesses infants' real-time comprehension of familiar words using a looking-while-listening task with named target and distractor images.

**Based on:** Bergelson and Swingley (2012); Fernald and Marchman (2012).

```text
word_recognition/
├── Aim1/
│   └── word-recognition_Aim1.mp4
├── Aim2/
│   └── wordrecognition_Aim2.mp4
└── LRISE/
    ├── 2026_10_05_word_recognition_LRISE.mp4
    └── word_recognition_lrise_v2.mp4
```

The Aim 2 version incorporated additional attention getters and previously tested image pairs.

The LRISE version updated the stimuli, updated the counterbalancing, and controlled for consistent timing between the word onset and end of trial. 

**Current CHS stimulus:** `2026_10_05_word_recognition_LRISE.mp4`

### 6. Social Evaluation (`Helpers/`)

Examines infants' preference for prosocial versus antisocial agents after observing animated helping and hindering events.

**Based on:** Hamlin et al. (2007); Margoni and Surian (2018).

```text
Helpers/
├── Aim1/
│   └── condition-1_Aim1.mp4 through condition-8_Aim1.mp4
├── Aim2/
│   └── condition1_Aim2.mp4 through condition8_Aim2.mp4
└── LRISE/
    └── Condition1_LRISE.mp4 through Condition4_LRISE.mp4
```

The task presents animated agents helping or hindering another agent's progress up a hill. 

The LRISE version updated to just four condition videos of side by side helping or hindering.

**Current CHS stimuli:** `2026_10_05_Condition1_LRISE.mp4` through `2026_10_05_Condition4_LRISE.mp4` in the main `mp4/` folder. These filenames differ from those in `Helpers/LRISE/` but are the same files.

### 7. Numeracy (`Numeracy/`)

Assesses infants' sensitivity to changes in nonsymbolic numerical quantities by comparing looking time to constant versus alternating streams of dots.

**Based on:** Libertus and Brannon (2010); Starr et al. (2013).

```text
Numeracy/
├── Aim1/
│   ├── Numeracy5cl_Aim1.mp4
│   ├── Numeracy5cr_Aim1.mp4
│   ├── Numeracy20cl_Aim1.mp4
│   └── Numeracy20cr_Aim1.mp4
├── Aim2/
│   ├── Numeracy5cl_Aim2.mp4
│   ├── Numeracy5cr_Aim2.mp4
│   ├── Numeracy20cl_Aim2.mp4
│   └── Numeracy20cr_Aim2.mp4
└── LRISE/
    ├── Numeracy5cl1_LRISE.mp4
    ├── Numeracy5cr1_LRISE.mp4
    ├── Numeracy20cl1_LRISE.mp4
    └── Numeracy20cr1_LRISE.mp4
```

The conditions vary the constant numerical quantity (5 or 20 dots) and its position on the screen (left or right).


**Current CHS stimuli:** `Numeracy5cl1.mp4`, `Numeracy5cr1.mp4`, `Numeracy20cl1.mp4`, and `Numeracy20cr1.mp4` in the main `mp4/` folder. The corresponding task-organized LRISE files have `_LRISE` suffixes.

### 8. Speech Discrimination (`SpeechDiscrimination-LRISE/`)

Assesses infants' sensitivity to differences between speech sounds, including phonetic contrasts relevant to their language experience.

**Based on:** Werker & Hensch, (2015)

```text
SpeechDiscrimination-LRISE/
├── LRISE_v1/
│   └── conditionvideo_1.mp4 through conditionvideo_12.mp4
└── LRISE_v2/
    └── speechdisc_lrise_condition_1.mp4
        through speechdisc_lrise_condition_12.mp4
```

The folder contains two stimulus versions, each with twelve conditions.

The LRISE_v1 contains the videos played back to back. 

The LRISE_v2 versions include attention getters between the conditions. 

**Current CHS stimuli:** The twelve videos in `LRISE_v2/`.
