# Visual Field Restriction Data Collection Software

## Experiment Description

This software was designed to collect data for the experiment described in:

**Title:** Exploring the Visual Field Restriction in the Recognition of Basic Facial Expressions: A Combined Eye Tracking and Gaze Contingency Study

**Authors:** M. B. Urtado, R. D. Rodrigues, S. S. Fukusima

**Publication Status:** To be published

In this experiment, participants were presented with 30 facial image stimuli under three visual field restriction conditions: NVR (No Visual Restriction), PFFV (Parafoveal and Foveal Vision), and FV (Foveal Vision).<br>
In the NVR condition, stimuli were presented without any restriction, while in the PFFV and FV conditions, the visual field was limited to 5° and 2° of the visual angle, respectively.<br>
The visual restriction was implemented using the moving window technique, directly controlled by the eye tracker in response to the viewer’s eye gaze (this is controlled by the eye tracker driver, not the experiment software).<br>
For all conditions, the eye movements were constantly recorded (again directly by the eye tracker driver).<br>
The goal was to investigate the impact of visual field restriction on the recognition of basic facial expressions.<br>
<br>
Note: This README.md section provides a brief overview of the experiment conducted using the data collected with this software. For more detailed information, please refer to the publication once it is available.

## Requirements

1. Install PsychoPy (we used the 2022.2.3 version).
   - https://www.psychopy.org/download.html
   - Peirce J, Gray JR, Simpson S, MacAskill M, Höchenberger R, Sogo H, Kastman E, Lindeløv JK. (2019). PsychoPy2: Experiments in behavior made easy Behav Res 51: 195. https://doi.org/10.3758/s13428-018-01193-y
2. Check requeriments.txt for extra installation requirements.
3. Download the required facial images directly from [The Karolinska Directed Emotional Faces (KDEF)](https://kdef.se/).
   - Replace the 30 dummy images located in the "/Images/Faces" directory of this repository with the newly downloaded images according to the respective IDs indicated by file names (also see "Image IDs" on "Project Organization").
   - These 30 images need to be converted to grayscale in order to replicate our exact experiment.
4. Experiment conditions are determined based on the experimental parameters listed below.
5. The experiment was designed to be operated with an Eye Tracker as the moving window controller; however, it relies on the functionality of an Eye Tracker driver.
   - Otherwise, the moving window would be controlled by the computer mouse (which was not the method employed for our research data acquisition).

## Experimental Parameters

- **Eye Tracker Model:** The Eye Tribe’s ET1000.
- **Monitor:** LG Flatron 23MP65HA (1920 x 1080 pixels resolution, 23-inch screen).
- **Participant Distance:** 57 cm with chin rest usage.

## Project Organization

- Each ".psyexp" file corresponds to a distinct experiment. The file names correspond to the experimental conditions (NVR, PFFV, FV).
- "/data/" is the folder where the experiments record the data, each experiment generates three files, where the ".csv" file contains the recorded data.
- "/Images/Faces" contains all emotional facial images used by the experiment. All images were sourced from The Karolinska Directed Emotional Faces - KDEF image database.
  - **Note on Image Usage:** The original experiment utilized images from The Karolinska Directed Emotional Faces (KDEF) image database. However, **due to licensing restrictions, these images cannot be included in this repository**. As an alternative, we replaced the KDEF images with dummy synthetic facial images obtained from [ThisPersonDoesNotExist.com](https://thispersondoesnotexist.com/) converted to grayscale (**these were not used in the research experiment**). The file names were maintaned to keep compatibility with the original experiment source-code. These synthetic images have no research value and are not paired with the expected emotional expressions; they were included only to demonstrate the software functionality, allowing you to run it. Please, refer to "Requirements" in order to change these files to the correct ones from KDEF.
  - Goeleven, E.; Raedt, R.D.; Leyman, L.; Verschuere, B. The Karolinska Directed Emotional Faces: A validation study. Cognition and Emotion 2008, 22, 1094–1118. https://doi.org/10.1080/02699930701626582.
  - Lundqvist, D.; Flykt, A.; Öhman, A. The Karolinska Directed Emotional Faces - KDEF - CD ROM from Department of Clinical Neuroscience, 1998.
  - https://kdef.se/
  - Image IDs: AF01HAS, AM02HAS, AF02HAS, AM04HAS, AF06HAS, AM31HAS, AF03SAS, AM16SAS, AF07SAS, AM25SAS, AF17SAS, AM32SAS, AF04NES, AM05NES, AF08NES, AM07NES, AF16NES, AM13NES, AF13AFS, AM08AFS, AF14AFS, AM14AFS, AF21AFS, AM23AFS, AF05ANS, AM10ANS, AF09ANS, AM17ANS, AF20ANS, AM29ANS.

## License

This software is released under the BSD 3-Clause License.

## Research Ethics Committee

The study was approved by the Research Ethics Committee (CEP) of the University of São Paulo (protocol code 41844720.5.0000.5407). 