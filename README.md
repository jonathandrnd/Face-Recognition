# Face-Recognition
Implementation of face Recognition, Notebook was inspired by FaceNet paper (https://arxiv.org/abs/1503.03832) and assignment of deep learning specialization in coursera (https://www.coursera.org/learn/convolutional-neural-networks/home/week/4).

Face recognition problems commonly fall into two categories:

- Face Verification - "is this the claimed person?". For example, at some airports, you can pass through customs by letting a system scan your passport and then verifying that you (the person carrying the passport) are the correct person. A mobile phone that unlocks using your face is also using face verification. This is a 1:1 matching problem.
- Face Recognition - "who is this person?". For example, the video lecture showed a face recognition video (https://www.youtube.com/watch?v=wr4rx0Spihs) of Baidu employees entering the office without needing to otherwise identify themselves. This is a 1:K matching problem.

# Goal
- Face Recognition in real time.
- Use MTCNN algorithm to detect faces 
- Use a pretrained model to map face images into 128-dimensional encodings.
- Use these encodings to perform face recognition.

# Files Description

- **FaceRecognition.ipynb :** Contains the source code, Given a video and a database (People images folder) perform face recognition. Aditionally save the video with people's tags.
- **/database:**  Contains one image per person in the video. (You can add your own images , change video, or use Webcam).
- **facenet_keras_160x160.h5 :** Model Weights in Keras (FaceNet).
- **haarcascade_frontalface_default.xml** It was used for comparison purposes with MTCNN.
- **friends_output.mp4:** Result of run the algorithm.

![Alt text](https://github.com/jonathandrnd/Face-Recognition/blob/master/_img/sample.png?raw=true "Title")

# References

- Florian Schroff, Dmitry Kalenichenko, James Philbin (2015). [FaceNet: A Unified Embedding for Face Recognition and Clustering](https://arxiv.org/pdf/1503.03832.pdf)
- Yaniv Taigman, Ming Yang, Marc'Aurelio Ranzato, Lior Wolf (2014). [DeepFace: Closing the gap to human-level performance in face verification](https://research.fb.com/wp-content/uploads/2016/11/deepface-closing-the-gap-to-human-level-performance-in-face-verification.pdf) 
- MTCNN face detection implementation for TensorFlow https://github.com/ipazc/mtcnn
- OpenFace https://github.com/iwantooxxoox/Keras-OpenFace.
- FaceNet github repository: https://github.com/davidsandberg/facenet 
- deeplearning.ai ‘s assignments https://www.coursera.org/learn/convolutional-neural-networks/home/week/4
