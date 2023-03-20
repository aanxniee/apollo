# 🌿 apollo

Cerebral Palsy (CP) affects about 1 in 345 children and is the most common motor disability in childhood. Early diagnosis minimizes of complications such as hip dislocation, scoliosis and spasticity. Despite this, assessment for CP can take 18-24 months missing the crucial rapid neural development stage for intervention. CP assessments are also not be as widely accessible as they are lengthy and must be done over long periods of time. 

apollo is an app that aims to make CP assessments more accessible by bringing it straight to the patient's home. apollo uses machine learning and computer vision to determine early markers of cerebral palsy using the HINE model. HINE is a simple  scoreable, and standardized clinical neurological examination for infants between 2 and 24 months of age. It consists of 26 items, that are divided into 5 categories and assess the functions of the cranial nerves, body posture, movement, tone, reflexes, and reactions. Each item is evaluated on a 4 point scale, with 0 being the worst and 3 being the best. Refer to the HINE model below.

apollo assesses 2 of the 5 categories, posture and tone. the app uses OpenCV live video and Mediapipe to retrieve the infant's body coordinates and analyzes these coordinates using scikit-learn to produce a corresponding HINE score. The scores across the 2 categories are compiled and exported to be further examined by a licensed physician. 

## Tech Stack
- Python
- OpenCV
- Mediapipe
- scikit-learn
- Pandas
- Numpy

## How it Works
To use apollo, open your camera/webcam and then get into a position specified by the HINE model. Apollo will predict the corresponding pose and score.

![image](https://user-images.githubusercontent.com/63011927/226383370-c97571d4-b68e-4386-981b-0979bf482fd6.png)
![image](https://user-images.githubusercontent.com/63011927/226384643-5e1d2f0d-e149-423f-bf37-4d665db01ae2.png)
![image](https://user-images.githubusercontent.com/63011927/226384789-da21861a-c45d-4c2f-9234-ee6673ae575f.png)

## HINE
![image](https://user-images.githubusercontent.com/63011927/226380458-216b10ca-5175-4265-9b0c-04392e033ec9.png)
![image](https://user-images.githubusercontent.com/63011927/226380562-aeb666b2-8f88-4187-9203-d76a5dc18b1d.png)

Full HINE model:
[HINE.pdf](https://github.com/aanxniee/apollo/files/11019653/HINE.proforma_07_07_17.pdf)
