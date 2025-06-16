# AR Tattoo App: Proof of Concept (POC)

## 🎯 Project Vision (Overall App Concept)
The long-term vision for this application is to create a platform where tattoo artists can upload their flash designs (tattoo artwork), and potential clients can then use Augmented Reality (AR) to visualize these designs directly on their own bodies via their mobile camera, or on uploaded photos. Beyond the core AR functionality, future iterations aim to include artist portfolios, client search/filter capabilities, and potentially an on-platform messaging and commission system.

## ✨ Proof of Concept (POC) Objective
The primary objective of this Proof of Concept is to validate the core technical feasibility of the application's most critical and challenging features. By the end of this POC phase (targeting end of summer), we aim to demonstrate:

1. Successful, markerless AR overlay of 2D images onto a live camera feed/photo of a human body.

2. A viable method for automatically removing backgrounds from hand-drawn tattoo flash designs.

**Focus Area 1: React Native AR Deep Dive**
- **Goal:** To successfully implement and test a 2D image overlay within the React Native camera feed, specifically demonstrating "markerless" placement on a human body.

- **Key Focus Areas:**

  - Identifying and integrating the most suitable React Native AR library (e.g., react-native-arkit) that can leverage underlying ARKit/ARCore capabilities for body detection or people occlusion.

  - Setting up the foundational React Native project and version control.

- **Initial Test:** Can a static, transparent 2D image be accurately placed and displayed at a fixed point within the live AR camera view?

- **Crucial Test:** Can the chosen AR library detect a human body in the camera feed and project a pre-processed tattoo image onto it? This projection doesn't need to conform perfectly to body curves in the POC, but it must convincingly appear on the person's body without requiring manual markers.

- **Acceptance Criteria:** The POC should be able to display a pre-loaded, background-removed tattoo design on a person visible in the camera feed, allowing for basic user-controlled scaling and positioning of the design.

**Focus Area 2: Background Removal Methods**
- **Goal:** To identify and test a reliable method for automatically removing backgrounds from uploaded photos of tattoo designs (especially hand-drawn "flash" on paper), ensuring the tattoo outline is cleanly isolated for AR overlay.

- **Key Focus Areas:**

  - **API Service Integration (Fastest Approach for POC):** Research and test cloud-based API services (e.g., remove.bg, Google Cloud Vision API, AWS Rekognition) for automated background removal. This method is prioritized for its speed and typically high quality for the POC, acknowledging potential future costs.

  - **Local Library Research:** Exploring existing React Native libraries that offer image editing capabilities, with a primary focus on automated background removal. Secondary consideration will be given to other basic image adjustment features (e.g., lighting, contrast) that might improve flash sheet quality if they are not already digitized.

## 🗺️ Beyond the POC (Future Scope)
This POC focuses solely on proving the core AR and image processing capabilities. Future development will involve:

- Comprehensive user authentication and role management (artists vs. clients).

- Robust file upload system for tattoo designs.

- Advanced image editing and background removal integration.

- Artist profile management (collections, tagging, social links).

- Client search, filtering, favoriting, and collection features.

- Potential on-platform messaging and commission tools.