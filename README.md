<h1 align="center">Eduardo Larsen Güths</h1>

<p align="center">
  <b>Master's Student in Neuroscience (PPGNeuro · UFSC)</b> — Brain-Computer Interfaces<br>
  Decoding movement from EEG · 3D Modeling · Low-Cost Prototyping<br><br>
  From CAD to neural networks: end-to-end engineering applied to <b>prosthetic hands</b> and medical devices.
</p>

---

## 🧠 In focus: BCI for a Bionic Hand (Master's Project)

**Decoding 3D hand trajectories from EEG** to control a prosthesis — Master's in Neuroscience (PPGNeuro · UFSC), with the data collection protocol **approved by the UFSC Research Ethics Committee (CEP)**.

➡️ **[Mestrado-Kinect-EEG-Trajectory](https://github.com/educapeta/Mestrado-Kinect-EEG-Trajectory)**

What's in the repository:

- **Offline EEG acquisition** — g.Nautilus (32 channels, 500 Hz), ME/MI protocol with 6 conditions, markers with the exact EEG sample index and EEG↔motion synchronization via a shared monotonic clock
- **Multimodal hand ground truth** — Kinect v2 (RGB + depth), stereo-calibrated auxiliary webcams (reprojection error < 1.5 px), and **two inertial gloves** (ESP32 + MPU6050) with versioned firmware
- **SAND neural network** — sparse attention + convolutions: 2 s EEG window → 3D trajectory (30 × 3), with position/velocity targets and an anatomical regularizer
- **Online system** — asynchronous inference with the predicted trajectory overlaid on video, plus a Kalman filter fusing decoded velocity with IMU acceleration
- **~27 test suites** runnable without hardware, including end-to-end synthetic sessions

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097D7?style=flat&logo=google&logoColor=white)
![Kinect v2](https://img.shields.io/badge/Kinect_v2-7B83EB?style=flat&logo=microsoft&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat&logo=espressif&logoColor=white)
![g.tec](https://img.shields.io/badge/g.tec_g.Nautilus-00A3E0?style=flat)

---

## 🫁 InjeVent — Patented Emergency Ventilator

**Arduino-based emergency mechanical ventilator** developed during the COVID-19 pandemic, validated in animal model testing at Hospital das Clínicas (Porto Alegre) — protected by **patent application BR102020015383-8** (UFSC / IFSC).

➡️ **[injevent](https://github.com/educapeta/injevent)**

<table>
<tr>
<td width="280" align="center">
  <a href="https://github.com/educapeta/injevent">
    <img src="https://raw.githubusercontent.com/educapeta/injevent/main/docs/photos/injvent_prototype.jpg" alt="InjeVent prototype" width="240">
  </a>
</td>
<td>

- **Patent application BR102020015383-8** filed with INPI — inventors: Saulo Güths, **Eduardo Larsen Güths** & Marcelo Vandrese
- **25 firmware versions** (V4 → V41_PCV): dual PID control, PCV/VCV/A/C/PSV modes, dual ADS1115 16-bit pressure sensing, clinical alarms
- **17 3D-printed pneumatic parts** — collectors, solenoid couplings, relief valves, fittings
- **Clinical validation** on animal model alongside commercial ventilators (TAKAOKA), with medical & veterinary teams

</td>
</tr>
</table>

![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=arduino&logoColor=white)
![PID](https://img.shields.io/badge/Control-PID-brightgreen?style=flat)
![3D Printing](https://img.shields.io/badge/3D_Printing-STL-orange?style=flat)
![Patent](https://img.shields.io/badge/Patent-BR102020015383--8-blue?style=flat)

---

## 🔬 EEG Artifact Detection with CNN (Course Project)

**Automatic detection of EEG artifacts (blinks, muscle, motion) using a 1D convolutional neural network** — final project for *Modern Computational Tools* (Neuroscience graduate program, UFSC).

➡️ **[eeg-artifact-detection](https://github.com/educapeta/eeg-artifact-detection)**

An end-to-end pipeline covering the full EEG data lifecycle:

- **EDF/GDF I/O & cleaning** — interactive viewer, BAD-segment removal, metadata sanitization, clean export
- **Quantitative QEEG metrics** — band power (Delta→Gamma), inter-channel Z-scores, Welch PSD, topographic maps
- **CNN artifact classifier** (TensorFlow/Keras) — 0.5 s epochs, data augmentation, class-weighted training, probability-thresholded predictions exported back as MNE annotations
- **Data exploration tools** — NPY diagnostics, histogram, signal segment visualization

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![MNE](https://img.shields.io/badge/MNE_Python-2E8B57?style=flat)
![scikit--learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CA1AF?style=flat&logo=scipy&logoColor=white)

---

## 🦾 Low-Cost Anthropomorphic Arm (Undergraduate Thesis)

**"Prototipagem e análise estática de um braço antropomórfico de 4 GDL"** — Undergraduate thesis (TCC) in Mechanical Engineering, UFSC (2024), supervised by Prof. Rodrigo de Souza Vieira (co-supervision: Esdras S. da Silva).

Development of a **4-degree-of-freedom anthropomorphic arm** to simulate human arm motion: kinematic modeling, simulation, structural optimization of components, and a prototype built via **3D printing** — aiming to replicate common object-grasping movements, applying human tactile sensing technologies to upper-limb prostheses.

In collaboration with the **Robotics Lab (LAR)**, the **Biomedical Engineering Institute (IEB)**, and the **Integrated Circuits Lab (LCI)** at UFSC.

<div align="center">
<img src="assets/tcc/tcc_arm_isometric.png" alt="Isometric view of the 4-DOF anthropomorphic arm" width="49%">
<img src="assets/tcc/tcc_arm_side.png" alt="Side view of the arm" width="49%"><br>
<img src="assets/tcc/tcc_kinematic_4r.png" alt="4R kinematic model diagram" width="40%">
<img src="assets/tcc/tcc_fea_vonmises.png" alt="FEA von Mises stress of the optimized link" width="49%">
</div>

### 🔗 Resources

- **Thingiverse (3D-printable files):** [Antrophomorfic Arm 4DOF](https://www.thingiverse.com/thing:6723166) · [All designs](https://www.thingiverse.com/Educapeta/designs)
- **Full thesis (PDF, 146 pages):** [assets/tcc/tcc_thesis_eduardo_larsen_guths_2024.pdf](assets/tcc/tcc_thesis_eduardo_larsen_guths_2024.pdf)

---

## 🧩 3D Modeling Portfolio

<table>
<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/projetos-para-casa">
    <img src="https://raw.githubusercontent.com/educapeta/projetos-para-casa/main/01-rack-capo/preview.png" width="210">
  </a>
</td>
<td>
  <h3>🏠 <a href="https://github.com/educapeta/projetos-para-casa">Home Projects</a></h3>
  <b>20 designs</b>, each in its own folder with <b>README and preview image</b>: guitar
  capotraste with rack-and-pinion, monotub, cheese press and Camembert mold, volleyball
  net tensioner, water pump, phone clips and tripods, organizers, filament holders,
  bruxism plate, insulated reservoir, tolerance tester, and more.
  <br><br>
  <b>181 files</b> · <code>.SLDPRT</code> <code>.SLDASM</code> <code>.STL</code> <code>.ipt</code> <code>.gx</code> <code>.fpp</code>
</td>
</tr>

<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/projetos-para-cervejaria">
    <img src="https://raw.githubusercontent.com/educapeta/projetos-para-cervejaria/main/Cerveja_Facil_AgroKeg/Desenhos/Carbonator_AgK_Tampa.JPG" width="210">
  </a>
</td>
<td>
  <h3>🍺 <a href="https://github.com/educapeta/projetos-para-cervejaria">Brewery Projects</a></h3>
  <b>Carbonator</b> system for the Cerveja Fácil / AgroKeg project (cap, gas base,
  O-ring pins, nuts and spring), flexible version with tap, O-ring molds, adapters,
  sparge, thermometer holder, and fermenter tap guide.
  <br><br>
  <b>107 files</b> · <code>.SLDPRT</code> <code>.SLDASM</code> <code>.SLDDRW</code> <code>.STL</code> <code>.gx</code> <code>.fpp</code>
</td>
</tr>

<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/equipamentos-saulo">
    <img src="https://raw.githubusercontent.com/educapeta/equipamentos-saulo/main/Air_Safe/Midias/render.JPG" width="210">
  </a>
</td>
<td>
  <h3>🔧 <a href="https://github.com/educapeta/equipamentos-saulo">Equipment</a></h3>
  <b>Sheet-metal enclosures</b> with flat patterns for laser cutting (Air Safe Model 1
  and 2, with technical drawings and assembly videos), 3D-printed boxes (DUPLAC V1/V2),
  CO₂ meter enclosure, motorcycle case, buckles, lamp holder, and finishing parts.
  <br><br>
  <b>133 files</b> · <code>.SLDPRT</code> <code>.DXF</code> <code>.PDF</code> <code>.IGS</code> <code>.stp</code>
</td>
</tr>

<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/trabalho-final-metodologia">
    <img src="https://raw.githubusercontent.com/educapeta/trabalho-final-metodologia/main/Desenhos/Braco_Superior.JPG" width="210">
  </a>
</td>
<td>
  <h3>🦾 <a href="https://github.com/educapeta/trabalho-final-metodologia">Mechanical Actuator (Course Project)</a></h3>
  Mechanical system of links and levers inspired by an accelerator handle, with gripper
  and tweezers. Includes final assembly, technical drawings of the parts, and the
  project specification report.
  <br><br>
  <b>21 files</b> · <code>.SLDPRT</code> <code>.SLDASM</code> <code>.SLDDRW</code> <code>.docx</code>
</td>
</tr>

<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/motorhome">
    <div style="font-size:64px">🚐</div>
  </a>
</td>
<td>
  <h3>🚐 <a href="https://github.com/educapeta/motorhome">Motorhome</a></h3>
  Sink designed to maximize the limited counter space of a vehicle — parametric model
  with STL ready for 3D printing.
  <br><br>
  <b>6 files</b> · <code>.SLDPRT</code> <code>.STL</code>
</td>
</tr>

<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/confortimetro">
    <div style="font-size:64px">🌡️</div>
  </a>
</td>
<td>
  <h3>🌡️ <a href="https://github.com/educapeta/confortimetro">Confortímetro</a></h3>
  3D modeling of the comfort meter development project.
  <br><br>
  <b>5 files</b> · <code>.SLDPRT</code>
</td>
</tr>
</table>

💡 Opening any `.stl` file in a GitHub repository renders the part in 3D. 🖨️

---

## 🛠️ Tools & Formats

`SolidWorks 2017` · `FlashPrint` · `Fusion 360` · `AutoCAD/DXF` · `Inventor` ·
`Python` (NumPy · PyTorch · OpenCV · MediaPipe) · `PlatformIO/ESP32` · `Kinect SDK 2.0` ·
`STL` (3D printing) · `DXF` (sheet metal) · `STEP / IGES / x_t` (CAD interchange) · `Git LFS`

## 📄 License

3D models are my own work, released under **CC BY-NC-SA 4.0** — use, print, and adapt
with attribution, non-commercial only. For commercial use, contact me.

---

<p align="center"><i>Opening an <code>.stl</code> file in any repository lets GitHub display the part in 3D. 🖨️</i></p>
