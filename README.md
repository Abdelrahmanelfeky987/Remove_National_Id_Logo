# Remove_National_Id_Logo
Given a picture of an Egyptian national id, you are tasked to remove the logo of جمهورية
مصر العربية and replace it with the color of its background,
#Steps
* Collect addidtional data from kaggle dataset [egyptian-ids](https://www.kaggle.com/datasets/mostafaebrahiem/egyptian-ids) 

* Annotate the data using `roboflow` and using different types of augmentation
  - Rotation
  - Shearing

* Train yolov8n to detect logo of جمهورية مصر العربية from images starting with initial parameters from pre-trained yolo

* Remove logo from the image 
  - Extract  logo by get coordinates of the bounded box `ROI`
  - Get the background color
  - Fill the bounded box `ROI` by the background color

 * Save the image without logo
