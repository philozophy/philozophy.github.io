Technical tidbits useful for the site.

## Feedburner
http://feeds.feedburner.com/Philozophy

## Fonts
https://www.onlinewebfonts.com/search?q=Caslon

- public health and liberty:
  - specific examples: church closures, lockdowns for covid 19
  - show why we won't find rational grounds to decide that question:
    - probabilities, future, subjective risk affinity
- fallacies
- stories

## Transcribing podcasts to text
It does not work, the result requires too much editing.

The software you can use is Vosk-api, a modern speech recognition toolkit based on neural networks. It supports 7+ languages and works on variety of platforms including RPi and mobile.

First you convert the file to the required format and then you recognize it:

ffmpeg -i file.mp3 -ar 16000 -ac 1 file.wav
Then install vosk-api with pip:

pip3 install vosk
Then use these steps:

git clone https://github.com/alphacep/vosk-api
cd vosk-api/python/example
wget https://github.com/alphacep/kaldi-android-demo/releases/download/2020-01/alphacep-model-android-en-us-0.3.tar.gz
tar xf alphacep-model-android-en-us-0.3.tar.gz 
mv alphacep-model-android-en-us-0.3 model-en
python3 ./test_simple.py file.wav > file.json

## CSS snippet for handling fonts
<style> 
    /* @font-face {
      font-family: "Caslon"; 
      font-variant-ligatures: common-ligatures discretionary-ligatures historical-ligatures contextual;
      src: url("//db.onlinewebfonts.com/t/22bd8660c8d0b70ac3e9d024f7f2c31d.eot"); 
      src: url("//db.onlinewebfonts.com/t/22bd8660c8d0b70ac3e9d024f7f2c31d.eot?#iefix") format("embedded-opentype"), 
      url("//db.onlinewebfonts.com/t/22bd8660c8d0b70ac3e9d024f7f2c31d.woff2") format("woff2"), 
      url("//db.onlinewebfonts.com/t/22bd8660c8d0b70ac3e9d024f7f2c31d.woff") format("woff"), 
      url("//db.onlinewebfonts.com/t/22bd8660c8d0b70ac3e9d024f7f2c31d.ttf") format("truetype"), 
      url("//db.onlinewebfonts.com/t/22bd8660c8d0b70ac3e9d024f7f2c31d.svg#Caslon") format("svg"); 
    }
      
    @font-face {
      font-family: "My Hoefler Text";
      font-variant-ligatures: common-ligatures discretionary-ligatures historical-ligatures contextual;
      text-rendering: optimizeLegibility;
      src: url("/assets/fonts/Hoefler-Text_Regular.woff2") format("woff2");
    }
    
    @font-face {
      font-family: "Clicker Script"; 
      src: url("//db.onlinewebfonts.com/t/b5cae760e3ebeb67aed58508b5ae4269.eot"); 
      src: url("//db.onlinewebfonts.com/t/b5cae760e3ebeb67aed58508b5ae4269.eot?#iefix") format("embedded-opentype"), 
      url("//db.onlinewebfonts.com/t/b5cae760e3ebeb67aed58508b5ae4269.woff2") format("woff2"), 
      url("//db.onlinewebfonts.com/t/b5cae760e3ebeb67aed58508b5ae4269.woff") format("woff"), 
      url("//db.onlinewebfonts.com/t/b5cae760e3ebeb67aed58508b5ae4269.ttf") format("truetype"), 
      url("//db.onlinewebfonts.com/t/b5cae760e3ebeb67aed58508b5ae4269.svg#Clicker Script") format("svg"); } */
    
    /* p:first-child::first-letter {
      display: inline-block;
      float:left;
      font-size: 350%;
      margin-top: -14px; 
      margin-bottom: -14px;
      margin-right: 5px;
      color:#8C8273;
    } */
  </style>
