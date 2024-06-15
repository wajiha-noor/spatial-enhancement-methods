PROJECT STRUCTURE:
/static
    - original.png
    - gamma_corrected.png
/templates
    - index.html
    - upload.html
    - display.html
dip.py

PREREQUISITES:
Python 3.x
Flask
OpenCV
NumPy
Pillow

USAGE:
Open your web browser and navigate to http://127.0.0.1:5000/.
Click on "Upload Image" to go to the upload page.
Choose a file and upload it.
View the processed images.

EXPLANATION:
The process_image function performs several image processing operations:

Laplacian: Detects edges by calculating the second derivative of the image.
Sharpened Image: Sharpens the image by subtracting the Laplacian from the original image.
Sobel Combined: Computes the gradient magnitude using the Sobel operator.
Smoothed Image: Smooths the combined Sobel image using a blur filter.
Result Image: Combines the smoothed and sharpened images.
Final Image: Adds the result image to the original image.
Gamma Correction: Applies gamma correction to the final image to adjust the brightness.

TEMPLATE FILES:
index.html: The homepage that displays the background.
upload.html: The upload page where users can upload an image.
display.html: The page that displays the processed images.

SAMPLE OUTPUT:
Upon uploading an image, the following processed images will be generated and saved in the static folder:

original.png: The original grayscale image.
gamma_corrected.png: The final image after all processing and gamma correction.

CONTRIBUTING:
Contributions are welcome! Please open an issue or submit a pull request for any changes.

CONTACT:
For any questions or issues, please contact wajihanoor848@gmail.com.
