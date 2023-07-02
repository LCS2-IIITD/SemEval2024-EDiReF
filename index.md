---
title: "SemEval 2024 Task: Emotion Discovery and Reasoning its Flip in Conversation (EDiReF)"
---

The __EDiReF__ shared task at [SemEval 2024](https://semeval.github.io/SemEval2024/) is an amalgamation of three subtasks tasks- (i) Emotion Recognition in Conversation __(ERC)__ in Hindi-English code-mixed conversations, (ii) Emotion Flip Reasoning __(EFR)__ in Hindi-English code-mixed conversations, and (iii) __EFR__ in English conversations. The definition for the tasks of ERC and EFR are as illustrated below:

* __ERC__:  Given a dialogue, ERC aims to assign an emotion to each utterance from a predefined set of possible emotions.
* __EFR__: Given a dialogue, EFR aims to identify the trigger utterance(s) and instigators for an emotion-flip in a multi-party conversation dialogue.

For example, given a sample dialogue below:

|     Speaker    |                Utterance            |
|----------------|-------------------------------------|
| Sp<sub>1</sub> | I had an awful day today!           |
| Sp<sub>2</sub> | Oh no! What happened?               |
| Sp<sub>1</sub> | Somebody ate my sandwich!           |
| Sp<sub>2</sub> | I can make you a new one right now! |
| Sp<sub>1</sub> | That would be great! Thanks!        |

ERC aims to assign emotions to each utterance

|     Speaker    |                Utterance            | Emotion |
|----------------|-------------------------------------|---------|
| Sp<sub>1</sub> | I had an awful day today!           | Sad     |
| Sp<sub>2</sub> | Oh no! What happened?               | Sad     |
| Sp<sub>1</sub> | Somebody ate my sandwich!           | Sad     |
| Sp<sub>2</sub> | I can make you a new one right now! | Joy     |
| Sp<sub>1</sub> | That would be great! Thanks!        | Joy     |

The example dialogue has two emotion flips. Sp<sub>1</sub>'s emotion changed from Sad to Joy while Sp<sub>2</sub>'s emotion also shifted from Sad to joy. EFR aims to justify such emotion flips using triggers and instigators.

|     Speaker    |                Utterance            | Emotion | Trigger | Instigators |
|----------------|-------------------------------------|---------|---------|-------------|
| Sp<sub>1</sub> | I had an awful day today!           | Sad     |    0    |      -      |
| Sp<sub>2</sub> | Oh no! What happened?               | Sad     |    0    |      -      |
| Sp<sub>1</sub> | Somebody ate my sandwich!           | Sad     |    0    |      -      |
| Sp<sub>2</sub> | I can make you a new one right now! | Joy     |    1    |   Excited   |
| Sp<sub>1</sub> | That would be great! Thanks!        | Joy     |    0    |      -      |

## Organization

<!-- Please subscribe to https://groups.google.com/group/dimsum16 for announcements about the task.

See the [schedule](http://alt.qcri.org/semeval2016/task10/index.php?id=important-dates) for planned data releases and deadlines. -->

The organizers are:

* [Shivani Kumar](https://sites.google.com/iiitd.ac.in/shivani-kumar/home),  IIIT Delhi
* [Md Shad Akhtar](https://faculty.iiitd.ac.in/~shad.akhtar/),  IIIT Delhi
* [Tanmoy Chakraborty](https://www.tanmoychak.com/),  IIT Delhi
* [Eric Cambria](https://dr.ntu.edu.sg/cris/rp/rp00927), NTU, Singapore
