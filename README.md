# Face-Detection-Recognition
## 1. Face Verification
### A) One way to do this is by comparing distance between images as - Given 2 images, compare and identify if these are the images of the same human. This is done by pixel-by-pixel comparison of both these 2 images. The distance between both images should be less than a given threshold, say 0.7. But this algorithm perfoms poorly due to variations in images such as lighting, facial emotions, orientation etc
### B) Better Idea - Element Wise Comparison as - 
#### i) Loading Pre-trained weights
#### ii) Encoding images as 128 dimensional vectors by loading inception module (This network uses 96x96 dimensional RGB images as its input. Specifically, inputs a face image (or batch of  mm  face images) as a tensor of shape  (m,nC,nH,nW)=(m,3,96,96)(m,nC,nH,nW)=(m,3,96,96). It outputs a matrix of shape  (m,128)(m,128)  that encodes each input face image into a 128-dimensional vector
