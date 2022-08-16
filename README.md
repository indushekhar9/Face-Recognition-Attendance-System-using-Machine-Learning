
## Face Recognition Attendance System using Machine Learning

In this project, I have developed an attendance system through which real time attendance of students, employees can be marked on real time basis just by showing their face or their ID card in which photo is available, to the camera of the device on which project is running.

Basically there are four steps & algorithms are used-

### 1. FACE DETECTION
   #### --> HOG(Histogram of Gradients)-
         Here every single pixel of face is detected and creates a unique systematic gradient of each face on the basis of alignment of eyes, nose, lips &          chin etc.
### 2. FACE EXTRACTION
  #### --> Face Landmark estimation algorithm-
        In this algorithm 68 landmarks (specific points) are specifed on every faces.
### 3. FACE ENCODING
  #### --> Convolutional Neural Network
        This is time taking to search for the matching face in our file if number of students or employees is sufficiently large.
        So, to overcome this encoding of every faces is performed. In this 128 measurements for every faces are given which is called are embedding.
### 4. FINDING PERSON'S NAME FROM ENCODING
  #### --> SVM Classifier (Classification algoritm)-
        It matches the encoding of captured faces with closely matching measurements of given images.
 
 
 
Using these algorithm attendance is marked on a csv file, but for **Monitoring Attendance** on real time basis I have created a **FACE ATTENDANCE SYSTEM**  Application using **Oracle APEX**, on which user have to give his username and password and then he can see the **Dashboard, Face Attendance Search, Face Attendance Report, Calendar** on which analytics of attendances are available using different data representation models. Data are modified on a regular time interval i.e., If student is marking his attendance on system then his details are sent on application through POST method of Oracle REST Data Services (ORDS) at that time and his attendance details are shown on the application.
