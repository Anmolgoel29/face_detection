# Image Recognition using python and machine learning for segregating images.

1. here we use convert images to embedding vectors and then compare to see the similarities between two different images.
2. known faces are converted to embedding vectors from given images .
3. know we detect faces in the input video/image and convert them into embedding vectors. These vectors are compared with the embedding vectors of the known faces.

## Steps:
1. Converting known faces into embeddings
-> load the haar cascade xml file
-> pass it to cv2 using a cascadeclassifier function.
-> read the known faces file
-> convert it to grayscale for faster computation
-> know run a function using the harr-cascade var, detectMultiScale( <image> , <scaleFactor (compression amount)> , <minNeighbours (least number of faces to look along with the first detected face)> , <minSize (min size of a face)>)


Main flow of the program would be as follows:
load the known faces from the folder and then convert them into embeddings

then one by one pick up all images from the media folder then extract faces and convert them into embeddings
if there are no face matches we delete the file else we keep it.