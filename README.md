# COVID Audio Model
### 1. Data Preprocessing 
a) Remove bad data

If the audio file is empty, or other sound is recorded, remove it.

b) Data partitioning

Due to lack of data files, separate cough data once or twice and add them to data.

c) Data augmentation

Add white noise, data shift, speeded up the data, slowed down the data and add them to data.

d) Wav file to image file

Convert audio files to mel-spectrogram images using librosa library and save it. 

### 2. Audio model
a) Extract the features from the images using Densnet201.

b) Train classifier.

### 3. Prediction 

----------

### 1. 데이터 전처리 
a) 필요없는 데이터를 제거한다.

오디오 파일이 비어있거나, 기침소리 외에 다른소리가 녹음되어 있는 경우 파일을 제거한다. 

b) 데이터를 나눈다.

데이터 부족을 보완하기 위하여, 기침소리를 한번 혹은 두번으로 분할한다. 

c) 데이터 augmentation을 진행한다. 

백색소음, 오디오 이동, 속도를 빠르기를 조절하여 augmentation을 진행한다. 

d) WAV 파일 변환 후 저장

WAV 파일을 librosa 라이브러리를 활용하여 mel-spectrogram으로 변환 후 image 파일로 저장한다. 

### 2. 모델 구축
a) Densent 201을 활용하여 features을 추출한 후 저장한다. 
b) COVID 와 NON-COVID 로 binary classifier을 진행한다. 

### 3. 예측 
a) WAV 파일을 image 파일로 저장하여 예측하는 code를 구현한다. 

--------------

Things to do
- 데이터를 기침 한개단위로 자르기
- CNN 변경
  
