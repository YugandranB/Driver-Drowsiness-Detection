<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Driver Drowsiness Detection - README</title>
</head>
<body style="font-family: Arial, sans-serif; line-height: 1.6; padding: 2rem;">

 <h1 align="center">🚗 Driver Drowsiness Detection System 😴</h1>
<p align="center"><strong>Real-time alert system using facial landmark detection & audio warning</strong></p>
<hr>
  <hr/>

  <h2>📌 Overview</h2>
  <p>This project aims to <strong>detect driver drowsiness in real-time</strong> using webcam input, facial landmark detection, and EAR (Eye Aspect Ratio) logic. When drowsiness is detected, an <strong>alarm sound</strong> is triggered to alert the driver.</p>

  <hr/>



  <hr/>

  <h2>⚙️ How It Works</h2>
  <ul>
    <li>Uses <strong>dlib's 68 facial landmarks</strong> to calculate EAR.</li>
    <li>EAR below a threshold for several frames → Drowsiness detected.</li>
    <li><strong>Plays alarm</strong> using <code>alarm.wav</code> to alert the driver.</li>
  </ul>

  <hr/>

  <h2>🚀 Getting Started</h2>
  <h3>🔧 Install Dependencies</h3>
  <pre><code>pip install -r requirements.txt</code></pre>


  <h3>▶️ Run Real-Time Detection</h3>
  <pre><code>python app/run_realtime.py</code></pre>

  <h3>📹 Test on Video</h3>
  <pre><code>python experiments/test_on_video.py --video path/to/video.mp4</code></pre>

  <hr/>

  <h2>🔊 Customizing the Alarm</h2>
  <p>Replace <code>assets/alarm.wav</code> with your preferred sound clip (WAV format).</p>

  <hr/>


  <hr/>

  <h2>👤 Author</h2>
  <p>
    <strong>Yugandran B</strong><br/>
    Connect on <a href="https://www.linkedin.com/in/yugandran-b/" target="_blank">LinkedIn</a><br/>
    GitHub: <a href="https://github.com/yugandranb" target="_blank">@yugandranb</a>
  </p>

  <hr/>

  <h2>📄 License</h2>
  <p>This project is under the <a href="LICENSE">MIT License</a>.</p>

</body>
</html>
