# Crater Detection for Rover Routing (CDRR)

# Problem & Solution
Crater detection is an important task for rover path planning and safe campaign of Lunar rovers. There exists blind spots/zones on terrain that require rovers to make spontaneuous decisions. With preexistant images and crater locations, our project was to classify craters and their locations to allow scientists to create ideal rover routes and make maps. 

# Methodology
To implement moon crater identficiation using prexisting data, we used two R-CNN models: ResNet 50 and YOLO v5. The ResNet 50 model was optimized to find that K=2 and alpha=0.01 were the best hyperparameters when the model was trained on 50 epochs of our dataset. The YOLO v5 model was pre-trained on the COCO dataset to find the best weights/biases for object detection and was fine-tuned to our crater image and coordinate dataset.

# Applications
Using detection edges, the information could be used to map a terrain and any blind spots could be filled based on probability of neighboring crater detection. The applications of our information could be data collection for lunar models, geological analysis, safety and monitoring of lunar conditions, exploratory missions, conservation, and more. Our project could also be furthered by altering the hyperparameters to optimize different models, alter detection to measure the depth of craters, identifying the probability of running into blind spots or the danger of being around a crater of certain depth, and we could also run our models on datasets of images on other planets! In the future, we could use an extended version of our project to collaborate with the CMU Prism Ranger, build a lunar positioning system, or track a rover's location (by running basic edge detection to determine position based on detected craters).

# Outcomes
This project was created to compete in HackCMU 2023: Space Theme. This project ended up winning the "Best Security" award, sponsored by Sandia National Labs.
