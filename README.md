<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Driver Drowsiness Detection System</title>
</head>
<body style="font-family: Arial, sans-serif; margin: 20px; line-height: 1.6;">

  <h1 align="center" style="font-size: 2.5em;">🚗 Driver Drowsiness Detection System 😴</h1>
  <p align="center" style="font-size: 1.2em;">
    <i>A real-time alerting system that detects driver drowsiness using facial landmark detection and EAR logic, with an integrated alarm mechanism.</i>
  </p>
  <hr>

  <h2>📌 Project Overview</h2>
  <p>
    Fatigue while driving is a major cause of road accidents. This project addresses that problem by implementing a real-time <strong>driver drowsiness detection system</strong>. It uses a webcam to monitor the driver’s face, detects eye blinks and closure patterns using facial landmarks, and calculates the Eye Aspect Ratio (EAR). If drowsiness is detected based on sustained low EAR values, an <strong>alarm is triggered</strong> to alert the driver instantly.
  </p>
  <hr>

  <h2>⚙️ Features</h2>
  <ul>
    <li>🎯 <strong>Real-Time Drowsiness Detection:</strong> Detects eye closure over time to infer fatigue.</li>
    <li>📍 <strong>EAR-Based Logic:</strong> Utilizes the Eye Aspect Ratio algorithm to determine the eye state.</li>
    <li>🔊 <strong>Instant Alarm System:</strong> Audible alerts triggered when drowsiness is detected.</li>
    <li>🧠 <strong>Custom Model Training (Optional):</strong> Expandable with deep learning for better accuracy.</li>
    <li>💻 <strong>Cross-Platform & Lightweight:</strong> Compatible with basic webcams and laptops.</li>
  </ul>
  <hr>

  <h2>🚀 Getting Started</h2>

  <h3>1. Clone the Repository</h3>
  <pre><code>git clone https://github.com/yourusername/driver-drowsiness-detection.git</code></pre>

  <h3>2. Install Dependencies</h3>
  <pre><code>pip install -r requirements.txt</code></pre>

  <h3>3. Run Real-Time Detection</h3>
  <pre><code>python app/run_realtime.py</code></pre>

  <h3>4. (Optional) Test on a Video</h3>
  <pre><code>python experiments/test_on_video.py --input path_to_video.mp4</code></pre>

  <hr>

  <h2>📊 How It Works - EAR (Eye Aspect Ratio)</h2>
  <p>
    The system uses dlib's 68-point facial landmark detector. The Eye Aspect Ratio (EAR) is computed as a ratio of distances between vertical eye landmarks and horizontal eye landmarks. A sustained low EAR indicates that the eyes are closed, thus suggesting drowsiness.
  </p>
  <pre><code>
EAR = (||p2 - p6|| + ||p3 - p5||) / (2 * ||p1 - p4||)
  </code></pre>
  <p>
    If EAR falls below a certain threshold (commonly <code>0.25</code>) for a number of consecutive frames, an alarm is triggered.
  </p>

  <p align="center">
    <img src="https://learnopencv.com/wp-content/uploads/2022/09/03-driver-drowsiness-detection-EAR-points.png" 
         alt="EAR Landmark Points" 
         width="600" 
         style="display: block; margin: auto;" />
    <br>
    <em>Figure: Eye landmarks used for EAR calculation</em>
  </p>

  <p align="center">
    <img src="https://www.mdpi.com/applsci/applsci-11-08441/article_deploy/html/images/applsci-11-08441-g001.png" 
         alt="System Architecture Diagram" 
         width="600" 
         style="display: block; margin: auto;" />
    <br>
    <em>Figure: System architecture for driver drowsiness detection</em>
  </p>

  <hr>

  <h2>🛠️ Dependencies</h2>
  <ul>
    <li><code>OpenCV</code> – For video capture and drawing landmarks</li>
    <li><code>dlib</code> – Facial landmark detection</li>
    <li><code>imutils</code> – For image processing utilities</li>
    <li><code>scipy</code>, <code>numpy</code> – For EAR calculation and matrix operations</li>
    <li><code>pygame</code> – To play alert sounds</li>
  </ul>
  <hr>

  <h2>📈 Future Improvements</h2>
  <ul>
    <li>🔬 Integrate infrared (IR) camera support for nighttime monitoring</li>
    <li>📱 Send alerts to connected mobile apps via Bluetooth or Wi-Fi</li>
    <li>🧠 Replace EAR logic with CNN/LSTM-based deep learning model</li>
    <li>🚘 Integrate with automotive systems for active braking or steering correction</li>
  </ul>

  <hr>

  <h2>🧾 License</h2>
  <p>This project is licensed under the <strong>MIT License</strong>. See the <code>LICENSE</code> file for more details.</p>

</body>
</html>
