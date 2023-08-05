# Age_and_Gender_Detection

<h2>Objective :</h2>
<p>To build a gender and age detector that can approximately predicts the gender and age of the person on scanning the face from a picture or from the live video though camera(webcam).</p>


<h2>About the Project :</h2>
<p>In this Python Project, I had used Machine Learning to accurately identify the gender and age of a person from a single image of a face. I used the models trained by <a href="https://talhassner.github.io/home/projects/Adience/Adience-data.html">Tal Hassner and Gil Levi</a>. The predicted gender may be one of ‘Male’ and ‘Female’, and the predicted age may be one of the following ranges- (0-5), (6-12), (13-18), (19-25), (28-34), (35,42), (43,50), (52,59), (60-100). It is very difficult to accurately guess an exact age from a single image because of factors like makeup, lighting, obstructions, and facial expressions</p>


<h2>The contents of this Project :</h2>
<ul>
  <li>opencv_face_detector.pbtxt</li>
  <li>opencv_face_detector_uint8.pb</li>
  <li>age_deploy.prototxt</li>
  <li>age_net.caffemodel</li>
  <li>gender_deploy.prototxt</li>
  <li>gender_net.caffemodel</li>
  <li>a few pictures to try the project on</li>
  <li>detect.py</li>
 </ul>
 <p>For face detection, we have a .pb file- this is a protobuf file (protocol buffer); it holds the graph definition and the trained weights of the model. We can use this to run the trained model. And while a .pb file holds the protobuf in binary format, one with the .pbtxt extension holds it in text format. These are TensorFlow files. For age and gender, the .prototxt files describe the network configuration and the .caffemodel file defines the internal states of the parameters of the layers.</p>


 <h2>How to use : </h2>
 <ul>
  <li>Download my Repository</li>
  <li>Open your windows powershell or command prompt or Terminal and change directory to the folder where all the files of repository are present.</li>
  <li><b>For detecting age and gender from the image : </li>
  
      python test.py --image image_name
</ul>
  <p><b>Note: </b>The Image should be present in same folder where all the files are present</p> 
<ul>
  <li><b>For detectig age and gender in the live video through webcam :</li>
  
      python test.py
</ul>
<ul>
  <li>Press <b>Ctrl + C or q</b> to stop the program execution.</li>
</ul>
