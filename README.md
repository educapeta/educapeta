<h1 align="center">Eduardo Larsen Güths</h1>

<p align="center">
  <b>Mestrando em Neurociências (PPGNeuro/UFSC)</b> — Interfaces Cérebro-Máquina<br>
  Decodificação de movimento a partir de EEG · Modelagem 3D · Prototipagem de baixo custo<br><br>
  Do desenho CAD à rede neural: engenharia de ponta a ponta aplicada a <b>próteses de mão</b>.
</p>

---

## 🧠 Em foco: BCI de mão biônica (projeto de mestrado)

**Decodificação de trajetória 3D da mão a partir de EEG** para controle de prótese — mestrado em
Neurociências (PPGNeuro/UFSC), com protocolo de aquisição **aprovado pelo CEP/UFSC**.

➡️ **[Mestrado-Kinect-EEG-Trajectory](https://github.com/educapeta/Mestrado-Kinect-EEG-Trajectory)**

- **Aquisição offline de EEG** — g.Nautilus (32 canais, 500 Hz), protocolo ME/MI com 6 condições,
  marcadores com a amostra exata do EEG e sincronização com o movimento por relógio monotônico comum
- **Ground truth multimodal da mão** — Kinect v2 (RGB + profundidade), webcams auxiliares calibradas
  em estéreo (erro de reprojeção < 1,5 px) e **duas luvas inerciais** (ESP32 + MPU6050) com
  firmware versionado
- **Rede SAND** — atenção esparsa + convoluções: janela de EEG de 2 s → trajetória 3D (30 × 3),
  com alvos de posição e velocidade e regularizador anatômico
- **Sistema online** — inferência assíncrona com a trajetória prevista sobreposta ao vídeo e
  filtro de Kalman fundindo velocidade decodificada com a aceleração do IMU
- **~27 suítes de teste** executáveis sem hardware, com sessões sintéticas ponta a ponta

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![MediaPipe](https://img.shields.io/badge/MediaPipe-0097D7?style=flat&logo=google&logoColor=white)
![Kinect v2](https://img.shields.io/badge/Kinect_v2-7B83EB?style=flat&logo=microsoft&logoColor=white)
![ESP32](https://img.shields.io/badge/ESP32-E7352C?style=flat&logo=espressif&logoColor=white)
![g.tec](https://img.shields.io/badge/g.tec_g.Nautilus-00A3E0?style=flat)

---

## 🦾 Braço antropomórfico de baixo custo (TCC)

Desenvolvimento de um **braço antropomórfico de 4 graus de liberdade** para simular o movimento do
braço humano: modelo cinemático, simulação, otimização estrutural dos componentes e protótipo
construído por **impressão 3D** — com o objetivo de replicar movimentos de preensão de objetos,
aplicando tecnologias de sensação táctil humana a próteses de membros superiores.

Em colaboração com o **Laboratório de Robótica (LAR)**, o **Instituto de Engenharia Biomédica (IEB)**
e o **Laboratório de Circuitos Integrados (LCI)** da UFSC.

🔗 **[Antrophomorfic Arm 4DOF no Thingiverse](https://www.thingiverse.com/thing:6723166)**
· [todos os designs](https://www.thingiverse.com/Educapeta/designs)

---

## 🧩 Repositórios de modelagem 3D

<table>
<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/projetos-para-casa">
    <img src="https://raw.githubusercontent.com/educapeta/projetos-para-casa/main/01-rack-capo/preview.png" width="210">
  </a>
</td>
<td>
  <h3>🏠 <a href="https://github.com/educapeta/projetos-para-casa">Projetos para Casa</a></h3>
  <b>20 modelagens</b>, cada uma em sua própria pasta com <b>README e imagem</b>: capotraste de
  violão com cremalheira, monotub, prensa e molde de queijo Camembert, catraca de rede de vôlei,
  bomba de água, prendedor e tripé de celular, organizadores, suporte de filamento, placa de
  bruxismo, reservatório isotérmico, testador de tolerância e mais.
  <br><br>
  <b>181 arquivos</b> · <code>.SLDPRT</code> <code>.SLDASM</code> <code>.STL</code> <code>.ipt</code> <code>.gx</code> <code>.fpp</code>
</td>
</tr>

<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/projetos-para-cervejaria">
    <img src="https://raw.githubusercontent.com/educapeta/projetos-para-cervejaria/main/Cerveja_Facil_AgroKeg/Desenhos/Carbonator_AgK_Tampa.JPG" width="210">
  </a>
</td>
<td>
  <h3>🍺 <a href="https://github.com/educapeta/projetos-para-cervejaria">Projetos para Cervejaria</a></h3>
  Sistema <b>Carbonator</b> do projeto Cerveja Fácil / AgroKeg (tampa, base de gás, pinos com
  o-ring, porcas e mola), versão flexível com espigão, moldes de o-ring, adaptadores, sparge,
  suporte de termômetro e direcionador de torneira do fermentador.
  <br><br>
  <b>107 arquivos</b> · <code>.SLDPRT</code> <code>.SLDASM</code> <code>.SLDDRW</code> <code>.STL</code> <code>.gx</code> <code>.fpp</code>
</td>
</tr>

<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/equipamentos-saulo">
    <img src="https://raw.githubusercontent.com/educapeta/equipamentos-saulo/main/Air_Safe/Midias/render.JPG" width="210">
  </a>
</td>
<td>
  <h3>🔧 <a href="https://github.com/educapeta/equipamentos-saulo">Equipamentos</a></h3>
  Gabinetes em <b>chapa dobrada</b> com padrão plano para corte (Air Safe Modelo 1 e 2, com
  desenhos técnicos e vídeos de montagem), caixas impressas em 3D (DUPLAC V1/V2), gabinete do
  medidor de CO₂, caixa para moto, fivelas, suporte de lâmpada e peças de acabamento.
  <br><br>
  <b>133 arquivos</b> · <code>.SLDPRT</code> <code>.DXF</code> <code>.PDF</code> <code>.IGS</code> <code>.stp</code>
</td>
</tr>

<tr>
<td width="230" align="center">
  <a href="https://github.com/educapeta/trabalho-final-metodologia">
    <img src="https://raw.githubusercontent.com/educapeta/trabalho-final-metodologia/main/Desenhos/Braco_Superior.JPG" width="210">
  </a>
</td>
<td>
  <h3>🦾 <a href="https://github.com/educapeta/trabalho-final-metodologia">Atuador Mecânico (Trabalho final)</a></h3>
  Sistema mecânico de braços e alavancas inspirado em uma manopla aceleradora, com garra e pinça.
  Inclui montagem final, desenhos técnicos das peças e o memorial descritivo do projeto.
  <br><br>
  <b>21 arquivos</b> · <code>.SLDPRT</code> <code>.SLDASM</code> <code>.SLDDRW</code> <code>.docx</code>
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
  Pia desenhada para aproveitar o espaço reduzido da bancada de um veículo — modelo paramétrico
  e STL pronto para impressão.
  <br><br>
  <b>6 arquivos</b> · <code>.SLDPRT</code> <code>.STL</code>
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
  Modelagem 3D do desenvolvimento do projeto do confortímetro.
  <br><br>
  <b>5 arquivos</b> · <code>.SLDPRT</code>
</td>
</tr>
</table>

---

### 🛠️ Ferramentas e formatos que uso

`SolidWorks 2017` · `FlashPrint` · `Fusion 360` · `AutoCAD/DXF` · `Inventor` ·
`Python` (NumPy · PyTorch · OpenCV · MediaPipe) · `PlatformIO/ESP32` · `Kinect SDK 2.0` ·
`STL` (impressão 3D) · `DXF` (corte de chapa) · `STEP / IGES / x_t` (intercâmbio) · `Git LFS`

### 📄 Licença

Os modelos são de minha autoria e estão sob **CC BY-NC-SA 4.0** — use, imprima e adapte com
atribuição, sem fins comerciais. Para uso comercial, entre em contato.

---

<p align="center"><i>Abrindo um arquivo <code>.stl</code> em qualquer repositório, o GitHub mostra a peça em 3D. 🖨️</i></p>
