# Detector_de_Fadiga
O programa desenvolvido é capaz de identificar sinais de fadiga em tempo real, como o fechamento prolongado dos olhos, a partir de um fluxo de vídeo gravado ou em tempo real.
<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">

</head>
<body>
  <h1>Detecção de Fadiga</h1>
  <p>Este é um projeto de detecção de fadiga que utiliza a relação de aspecto dos olhos (EAR) para identificar sinais de sonolência em pessoas. O código é capaz de capturar o vídeo de uma webcam, detectar os rostos presentes no vídeo e calcular o EAR para cada olho. Se o EAR estiver abaixo de um determinado limiar por um número consecutivo de quadros, um alarme será acionado indicando a sonolência.</p>
  <h2>Aplicações</h2>
  <p>Este projeto pode ser útil em situações em que a sonolência do operador ou condutor é uma preocupação, como em sistemas de monitoramento de motoristas, sistemas de segurança em ambientes de trabalho, entre outros.</p>
  <h2>Estrutura do Projeto</h2>
  <p>O projeto consiste em:</p>
  <ul>
    <li><code>detecao_fadiga.py</code>: contém o código para detectar a fadiga utilizando a relação de aspecto dos olhos (EAR).</li>
    <li><code>alarm.wav</code>: contém o arquivo de audio para o aviso sonoro de sonolência.</li>
    <li><code>shape_predictor_68_face_landmarks.dat</code>: contém o modelo treinado para a detecção de pontos da face.</li>                                                                 
  </ul>
  <h2>Pré-requisitos</h2>
  <p>Antes de executar o projeto, é necessário ter as seguintes dependências instaladas:</p>
  <ul>
    <li>scipy</li>
    <li>imutils</li>
    <li>numpy</li>
    <li>playsound</li>
    <li>argparse</li>
    <li>dlib</li>
    <li>opencv-python</li>
    <li>matplotlib</li>
  <p>Ou execute apenas um <code>pip install requirements.txt</code></p></p>
  </ul>
  <h2>Executando o Projeto</h2>
  <p>Para executar o projeto, siga as instruções abaixo:</p>
  <ol>
    <li>Instale as dependências listadas acima, caso ainda não estejam instaladas.</li>
    <li>Clone o repositório ou baixe o arquivo <code>detecao_fadiga.py</code>.</li>
    <li>Abra um terminal e navegue até o diretório onde o arquivo <code>detecao_fadiga.py</code> está localizado.</li>
    <li>Execute o seguinte comando no terminal para iniciar o projeto:</li>
  </ol>
  <pre><code>python detecao_fadiga.py</code></pre>
  <h2>Técnicas Utilizadas</h2>
  <p>O projeto utiliza as seguintes técnicas:</p>
  <ul>
    <li>Detecção de rosto com o detector frontal de rostos do dlib.</li>
    <li>Predição dos marcos faciais utilizando o preditor de marcos faciais do dlib.</li>
    <li>Cálculo da relação de aspecto dos olhos (EAR) para identificar o piscar de olhos.</li>
    <li>Desenho dos contornos do olho utilizando o casco convexo.</li>
    <li>Utilização da biblioteca <code>playsound</code> para reproduzir o alarme sonoro.</li>
    <li>Visualização da relação de aspecto dos olhos (EAR) ao longo do tempo utilizando a biblioteca <code>matplotlib</code>.</li>
  </ul>
  <p align="center"><em>Este projeto é fornecido como está, sem garantias ou responsabilidades. Use por sua própria conta e risco.</em></p>
</body>
</html>
