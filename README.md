# :dog: DogCam: Smart Camera for Tracking Your Dog's Movements
## 𝔼𝕧𝕖𝕟 𝕨𝕙𝕖𝕟 𝕀 𝕒𝕞 𝕒𝕨𝕒𝕪, 𝕀 𝕤𝕥𝕒𝕪 𝕚𝕟 𝕥𝕙𝕖𝕚𝕣 𝕨𝕠𝕣𝕝𝕕.

DogCam is a heart-driven side project that combines my love for **dogs** and my passion for **computer vision**. It’s built to help pet parents better understand and care for their furry companions by gently tracking their `daily behaviors`, offering `timely alerts`, and `capturing the little moments` that matter.

Unlike many commercial solutions that bundle expensive hardware and software, DogCam is an `open-source` project that works with any `RTSP-supported camera` making it more accessible for those who simply want to stay closer to their dogs, even from afar.

---

## :rocket: Motivation

After spending a year in Canada learning English, experiencing new cultures, building friendships with people from around the world, I returned home feeling recharged, and ready to reconnect with my technical roots in computer vision.

As a lifelong **dog lover** and someone who has volunteered to foster and train stray dogs, I wanted to build something meaningful at the intersection of **pet care** and **tech**.

This side project helps me sharpen my skills in `real-time video processing`, `object tracking`, `behavior recognition`, and `system integration` while also keeping an eye on my adopted aging Shiba Inu 🐕.

---

## :pushpin: Features

- :movie_camera: **Real-time RTSP Stream Capture** 
  Connects to any RTSP-supported camera via RTSP to record continuous video streams for behavior analysis.

- :on: **Object Tracking with Camera Adjustment** 
  Tracks pet movement within the frame.
  Supports automatic PTZ (Pan-Tilt-Zoom) control based on dog position to keep the dog centered on screen.

- :dog2: **Dog Behavior Detection (Under Development)** 
    - **General Behavior Detection:**
Uses pre-trained object detection models (e.g., YOLO) to detect common behaviors such as:
       - Sleeping / Lying down
       - Walking / Moving
       - Chewing toys

    - **Health-Sensitive Behavior Monitoring:**
  Customized detection for dogs, including:
      - Excessive foot licking (possible dermatitis indicator)
      - Repeated jumping on/off sofas (mobility risk for elderly dogs)

- :bell: **Real-time Notifications** 
  LINE or Slack alerts based on detected behaviors. In the future versions, Users will be able to configure which events trigger alerts.

- :bar_chart: **Daily Summary Report**
  Auto-generated report summarizing key activities, with short video highlights (e.g., “10 seconds of cute moments from today”).

### Dog Object Tracking:
![dogcam_demo_cropped](https://github.com/user-attachments/assets/35061d8a-acf5-4dfa-a1a9-e55354cb93a7)


---

## Roadmap

- [x] RTSP camera integration & video recording
- [x] Frame extraction & data labeling
- [ ] PTZ（Pan-Tilt-Zoom) integration for camera control (**working on**)
- [ ] Object tracking (OpenCV, DeepSORT)
- [ ] Object detection（YOLO） & activity segmentation
- [ ] Dog behavior detection model training
- [ ] Build interactive dashboard with Flask
- [ ] Integrate LINE/Slack notification bot

---

## Tech Stack

- Python + OpenCV
- FFmpeg (for stream handling & re-encoding)
- (Upcoming) DeepSORT supports multi-dog tracking with persistent identity assignment, even when dogs frequently enter, exit, or are briefly occluded in the video
- (Upcoming) Yolov for object detection
- (Planned) Flask for web interface
- (Planned) SQLite or MongoDB for storing activity metadata

---
## Contributing / Feedback

This project is still in early stages. If you have suggestions, feel free to open issues or fork the repo!

---

## About Me

Hi! I’m Ann, an Senior ML engineer/Data Scientist with a passion for dogs and tech. You can read more about my work at [LinkedIn](https://www.linkedin.com/in/ya-chu-chang-56aa15131).

