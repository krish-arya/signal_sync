SignalSync is an AI-based traffic management system that analyzes video footage to detect vehicles and identify emergency sirens. The system processes traffic videos to highlight traffic density and emergency events, providing real-time situational awareness.

Features: 
1. Vehicle detection using YOLOv5 models
2. Siren detection through audio signal analysis
3. Video processing with annotated bounding boxes and emergency event highlights
5. Real-time progress monitoring during video processing
6. Saves the processed video with detected vehicles and siren events

Tech Stack: 
1. Computer Vision: YOLOv5 (PyTorch), OpenCV
2. Audio Analysis: Librosa
3. Video Processing: MoviePy, ffmpeg-python
4. Environment: Google Colab or any compatible Python environment

Setup Instructions: 
1. Install the required dependencies:
2. pip install torch torchvision torchaudio opencv-python numpy librosa soundfile ffmpeg-python moviepy
3. Mount your Google Drive if using Google Colab.
4. Set the video_path, audio_path, and output_path variables according to your files.
5. Run the process_video function to process the video and save the output.

How it Works: 
1. Detects vehicles frame-by-frame using YOLOv5.
2. Extracts audio from the video for siren detection.
3. Identifies siren events based on spectral analysis.
4. Highlights frames with detected sirens and displays vehicle counts with timestamps.

Output: 
1. Bounding boxes for detected vehicles (cars, buses, trucks)
2. Red overlay and warning text during detected siren events
3. Frame-wise car count and time display

Future Scope: 
1. Upgrade to YOLOv8 for improved detection accuracy
2. Incorporate traffic flow prediction models
3. Enable real-time deployment using cloud APIs

