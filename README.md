# Korean FastSpeech 2 - Pytorch Implementation

# Install Dependencies
1.
python=3.7, [pytorch](https://pytorch.org/)=1.6, [ffmpeg](https://ffmpeg.org/)와 [g2pk](https://github.com/Kyubyong/g2pK)를 설치합니다.
```
# ffmpeg install
sudo apt-get install ffmpeg
pip install g2pk
```
2.
```
pip install -r requirements.txt
```

3.
```
# Preprocessing

**(1) kss dataset download**
* [Korean-Single-Speech dataset](https://www.kaggle.com/bryanpark/korean-single-speaker-speech-dataset): Download and unzip. change params in hparams.py

**(2) phoneme-utterance sequence간 alignment 정보 download**

* KSS ver.1.3. ([download](https://drive.google.com/file/d/1bq4DzgzuxY2uo6D_Ri_hd53KLnmU-mdI/view?usp=sharing))
* KSS ver.1.4. ([download](https://drive.google.com/file/d/1LgZPfWAvPcdOpGBSncvMgv54rGIf1y-H/view?usp=sharing))

Down KSS datasets and down Montreal Forced Aligner under links To train fastspeech2

**(3) **
```
python preprocess.py
```
```
4. 
# Synthesis
inference Sysnthesis 
```
python synthesis.py --step 500000
```
