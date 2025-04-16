<h1 align="center">🚗 Driver Drowsiness Detection System 😴</h1>
<p align="center"><strong>Real-time alert system using facial landmark detection & audio warning</strong></p>
<hr>

<h2>📌 Overview</h2>
<p>This project aims to <strong>detect driver drowsiness in real-time</strong> using webcam input, facial landmark detection, and EAR (Eye Aspect Ratio) logic. When drowsiness is detected, an <strong>alarm sound</strong> is triggered to alert the driver.</p>
<hr>


<h2>🚀 How to Run</h2>
<ol>
  <li>Clone the repo</li>
  <li>Install dependencies:
    <pre><code>pip install -r requirements.txt</code></pre>
  </li>
  <li>Run the detection system:
    <pre><code>python app/run_realtime.py</code></pre>
  </li>
</ol>
<hr>

<h2>📊 EAR Logic</h2>
<p>The <strong>Eye Aspect Ratio (EAR)</strong> is calculated using dlib's 68 facial landmarks. If EAR drops below a threshold (e.g. 0.25) for consecutive frames, it’s considered drowsiness.</p>

<hr>

<h2>🎯 Features</h2>
<ul>
  <li>Facial landmark detection using dlib</li>
  <li>Real-time video stream analysis</li>
  <li>Alarm audio to prevent microsleep events</li>
  <li>Optional model training for behavior detection</li>
</ul>

<hr>

<h2>🧠 Future Enhancements</h2>
<ul>
  <li>Night vision support with IR camera</li>
  <li>Integration with vehicle telemetry</li>
  <li>Voice-based warning or mobile alert</li>
</ul>

<hr>



<hr>

<h2>📜 License</h2>
<p>This project is licensed under the MIT License - see the <code>LICENSE</code> file for details.</p>
