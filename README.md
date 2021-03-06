# music_emotion_recognition
## Part 1. Feature Extraction
### Feature 1. Melody & Harmony
<font size = 5><font family = 'san-serif'>Salient Pitch(M & V), Chromagram Centroid(M & V), Key Clarity(Int), Mode(M & V), Harmonic Change(M & V)</font></font>

ref_paper: <a href = 'https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=876309'>Salient Pitch</a> <a href = 'http://mac.citi.sinica.edu.tw/~yang/pub/yang11taslp_dist.pdf'>CC, KY and Mode</a> <a href = 'http://delivery.acm.org/10.1145/1180000/1178727/p21-harte.pdf?ip=128.59.176.103&id=1178727&acc=ACTIVE%20SERVICE&key=7777116298C9657D%2ECCAFA7F43E96773E%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1574347291_3745098f57a0683d85b13b813d3202a3'>Harmonic Change</a>

Notice

The Salient Pitch for High-Frequency Part (> 1kHz) contain a Half-Wave-Rectification <a href = 'https://www.youtube.com/watch?v=Ll0IOk_Ltfc'>see it here</a>, it is not necessarily crucial to do this, hence, we just calculate the Second Peak for ACF(Autocorrelation Function) and it turns out to have the salient pitch within 70 ~ 10000 Hz


## Part 1.1 Emotion Annotation (Kernel Density Estimation)
### Time_average.csv (KDE for averaging time)
