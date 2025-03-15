## [Prototype] (https://www.figma.com/proto/Zf6ucyS94JkTrmuoybwpVR/Samsung-Camera-App-Feature?node-id=303-184&p=f&t=qK3nlvRvsDHn1D89-1&scaling=scale-down&content-scaling=fixed&page-id=0%3A1)

## Feature Introduction: Case-based Camera Pro Settings

### Problem Statement
Modern smartphones have powerful manual camera capabilities, but most users find manual settings (ISO, aperture, shutter speed, exposure, focus, white balance, etc.) confusing or overwhelming. There's currently no intuitive solution enabling average users to access professional-level photographic adjustments without extensive knowledge or trial-and-error.

### Introducing: Case-based Camera Pro Settings

**Concept Overview:**  
The Case-based Camera Pro Settings feature enables users to intuitively achieve optimal photographic results simply by expressing natural-language intentions or preferences. Users don't need detailed technical understanding; they describe their desired photographic outcomes verbally, and the camera software dynamically interprets these requests into optimal manual settings.

**Example Scenario:**  
A user preparing to photograph a sunset scene could simply say:
- *"Make the stars pop out more,"*
- *"Focus more on the background,"*
- *"Capture the sun's bright light without distorting nearby objects,"*
- *"Focus on the left corner where the person is standing."*  
The phone instantly translates these natural language descriptions into precise adjustments of ISO, white balance, shutter speed, aperture, exposure, and focus depth.

### Problem Statement Being Solved:

- Users struggle with complex manual camera controls.
- There's a gap between novice photography enthusiasts and professional camera settings.
- Existing auto modes lack nuanced, context-aware fine-tuning based on user intent.

### Use Cases:

1. **Casual Users:** Quick optimization for everyday photography situations (portraits, landscapes, low-light).
2. **Content Creators:** Efficiently translate creative visions into professional photos without manual fine-tuning.
3. **Professional Photographers:** Faster workflow by initial automated setting adjustments, with manual tweaks thereafter.

### Functional Description:

- Users activate the feature via voice command or simple UI prompt.
- Natural language input is processed by an on-device AI model.
- The AI translates descriptive inputs into precise camera parameter adjustments in real-time.
- A live preview instantly shows the applied adjustments, allowing users to iteratively refine commands.

### Underlying Technologies:

- **On-Device Natural Language Processing (NLP):**
  - Google's Gemini AI or Samsung's in-house NLP model interpreting context and photographic intent from spoken or typed language.

- **AI-driven Computational Photography Algorithms:**
  - Leveraging Samsung's advanced computational photography (ISP integration, Exynos or Snapdragon NPUs) for real-time, AI-based adjustments.

- **Scene Understanding via Computer Vision:**
  - Object detection and semantic segmentation to interpret spatial commands ("left corner," "background").
  - HDR and multi-frame image fusion for handling dynamic lighting instructions ("sun's bright light").

- **Adaptive Image Processing Pipeline:**
  - Dynamically adjusts ISO, exposure, white balance, depth-of-field, and focus based on AI-determined optimal parameters.

- **Integration with Samsung's Exynos/Snapdragon Chips:**
  - Exploiting the latest NPUs and ISPs for efficient on-device computation and minimal latency.

### Research Leveraged:

- Samsung’s AI photography features (Nightography, Object Eraser).
- Google's generative AI camera editing (Magic Editor, Best Take).
- Semantic segmentation and computational photography research from industry leaders like Google Research.

### Implementation Steps:

1. **Research and Prototyping:**
   - Build a prototype NLP model trained on a dataset of photographic commands and desired outcomes.

2. **Integration with Camera OS Pipeline:**
   - Modify camera OS-level software to process NLP outputs directly into manual setting adjustments.

2. **User Testing and Refinement:**
   - Iterate prototypes through UX testing with diverse user feedback.

3. **Deployment:**
   - Integrate into Samsung’s camera OS (One UI Camera) across Galaxy smartphones, watches (basic settings via voice commands), and future XR devices for immersive photographic control.

This feature empowers Samsung device users—regardless of expertise level—to effortlessly achieve professional-quality photography through intuitive interactions.


[View Design](./Design_Final.pdf)




Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
