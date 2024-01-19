# YOLOv3 to TensorFlow Lite Conversion

It is assummed that you already have a pre-trained YOLOv3 model setup that needs to be converted into TensorFlow Lite.

## Steps:

1. Clone the repository on your local machine.

2. Create a folder named `YOLOv3_TFLite` on your local machine and copy the YOLOv3 model weights i.e. `yolov3_training_last.weights` and `classes.txt` files inside it. The directory structure should look something like the following.
```
YOLOv3_TFLite
|__ yolov3_training_last.weights
|__ classes.txt
```
3. Sign in to your Google account and upload the `YOLOv3_TFLite` folder on Google Drive. Change the access permission to `Anyone with the link` for both the files inside the `YOLOv3_TFLite` folder.

4. Open Google Colab and upload the `YOLOv3_to_TFLite_Conversion.ipynb` notebook from the repository you had cloned and run the notebook cells one-by-one as instructed. For detailed explain, refer the following [document](https://github.com/NSTiwari/YOLOv3-to-TensorFlow-Lite-Conversion/blob/main/YOLOv3%20to%20TensorFlow%20Lite%20Conversion.pdf).

5. Once the YOLOv3 model is converted into its TF Lite version, download the `detect.tflite` onto your local machine from the `YOLOv3_TFLite` folder saved on Google Drive. Copy `detect.tflite` and `classes.txt` inside the `YOLOv3-to-TensorFlow-Lite-Conversion` repository you had cloned earlier.

6. Create a folder named `test_images` inside the repository and add some images inside it which you would like to test the model on.

7. Open `test_tflite.py` file and edit **Line 151** by replacing `<your_test_image>` with the name of image file you want to test.

8. Run the following command: `python test_tflite.py`

## Output:

![GitHub Logo](/output.jpg)

- Read the [Medium](https://medium.com/tfug-mumbai-weekly/yolov3-to-tensorflow-lite-conversion-4602cec5c239) blog.
