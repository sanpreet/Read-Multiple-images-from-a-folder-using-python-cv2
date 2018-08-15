# Read-Multiple-images-from-a-folder-using-python-cv2
## Purpose of this code  

Reading Multiple images from a folder using python cv2. I am showing you the images inside the folder which I have used.

![final_images](https://user-images.githubusercontent.com/3431730/44170342-aecdfe00-a0f4-11e8-836d-b684139ddb67.png)

### How I have implemented this code
I have used for loop to read all the images present in the folder and converted it into matric and then from numpy array to rgb display. Please refer to below code to understand my point of view. :fire:


---

```
#import the library opencv
import cv2
#globbing utility.
import glob
#select the path
path = "A:\MY_company\Sanpreet_Singh\Client Work\OpenCV-Sanjeev\images\*.*"
for file in glob.glob(path):
print(file)
a= cv2.imread(file)
print(a)
# %%%%%%%%%%%%%%%%%%%%%
#conversion numpy array into rgb image to show
c = cv2.cvtColor(a, cv2.COLOR_BGR2RGB)
cv2.imshow('Color image', c)
#wait for 1 second
k = cv2.waitKey(1000)
#destroy the window
cv2.destroyAllWindows()
```


---

## How to run this code
To run this code, please download images and python file in a directory and run the following command
```
python reading_multiple_images_opencv2.py
```

