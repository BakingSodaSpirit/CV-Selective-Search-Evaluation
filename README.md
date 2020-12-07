# CV-Selective-Search-Evaluation

Selective Search- Directing Object Detection to Potential Regions<br />

In the sliding window approach, an inspection window is passed over an image to select a patch and classify each image patch covered by the window using the object recognition model. It is an exhaustive search for objects over the entire image. Not only do we need to search all possible locations in the image, we have to search at different scales. This is because object recognition models are generally trained at a specific scale (or range of scales). This results into classifying tens of thousands of image patches.<br />

Region proposal algorithms identify prospective objects in an image using segmentation. In segmentation approaches, group adjacent regions which are similar to each other based on some criteria such as color, texture etc. Unlike the sliding window approach where we are looking for the object at all pixel locations and at all scales, region proposal algorithm work by grouping pixels into a smaller number of segments. The final number of proposals generated are many times less than sliding window approach. This reduces the number of image patches we have to classify. These generated region proposals are of different scales and aspect ratios.<br />

Dataset:<br />
beagle.png<br />
test.png<br />
