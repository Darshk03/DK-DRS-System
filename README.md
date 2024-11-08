# DK-DRS-System

This project is a Decision Review System (DRS) simulation built using Python and the Tkinter GUI library. It mimics a cricket DRS system, allowing users to play a video clip and review "out" or "not out" decisions with a simulated interface. The project also utilizes OpenCV, PIL, threading, and imutils for video processing and image handling.

Features
Play video forwards and backwards at different speeds.
Simulate a decision review with "Out" or "Not Out" images displayed after a short delay.
Interactive GUI with buttons for playback control and decision review options.
Prerequisites
Make sure you have Python 3 and the following libraries installed:

tkinter (usually included with Python)
opencv-python
Pillow
imutils
You can install the required libraries using:

bash
Copy code
pip install opencv-python pillow imutils
Project Structure
clip.mp4 - Video file to simulate the match or incident.
Welcome.jpg - Welcome screen image.
Decision Pending.jpg - Displayed when a decision is pending.
sponsor.jpg - Sponsor image displayed briefly before the final decision.
OUT.jpg and NOT OUT.png - Final decision images for "out" and "not out."
How to Run the Project
1Clone the repository or download the project files.

2)Ensure the required images and video file (clip.mp4) are in the project directory.

3)Run the drs_system.py (or your main Python file name) using:

Usage
Once the application is running:

Use the buttons to navigate through the video:
<< Previous (fast): Rewind the video quickly.
<< Previous (slow): Rewind the video slowly.
Next (slow) >>: Fast forward the video slowly.
Next (fast) >>: Fast forward the video quickly.
Give Out: Start the "Out" decision review sequence.
Give Not Out: Start the "Not Out" decision review sequence.
The sequence includes:

A "Decision Pending" image.
A sponsor image.
The final decision as either "OUT" or "NOT OUT".
Code Overview
The main functions in this code:

play(speed): Controls video playback speed and direction.
pending(decision): Simulates the review process and displays the appropriate images for each stage.
out() and not_out(): Launch threads to handle "Out" and "Not Out" decisions.
Contributing
Feel free to open issues or submit pull requests for improvements or additional features!

License
This project is open-source and available under the MIT License.

