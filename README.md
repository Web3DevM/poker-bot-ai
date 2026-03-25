# Poker Bot AI For Holdem

Hello! The project took a little over a month to complete.

I spent a week researching poker, writing notes, and getting a general understanding of the topic.

A week was spent writing the GUI (graphical user interface), creating the overall project architecture, and writing the code.

A week was spent on computer vision and preparatory work.

A week was spent training my YOLO models. I managed to train two models: one for table detection, the other for card detection.

Finally, a week was spent putting everything together, testing, fixing bugs, and compiling it into an executable file.

# Computer Vision

Computer Vision is a field of artificial intelligence that allows computers to "see" and interpret images and videos.

If you think about it, it's a pretty cool technology! Essentially, it's a mechanism for processing an image or video (a sequence of images), in which an algorithm finds the desired object, adds its coordinates, its name, and its confidence.

There are many different methods, programs, and libraries that implement CV.

I chose YOLO.

# A Brief Introduction to Roboflow

Roboflow is a web service for annotating and managing datasets, greatly simplifying the process of preparing data for training computer vision models.

Roboflow makes it easy to upload images, annotate them, and apply various types of augmentation to increase the data volume. This is especially helpful when you're working alone and need a lot of data.

Notes:

Roboflow is a cloud platform and runs in a browser. All data is stored on servers. For businesses, this can be sensitive. For a pet project, it's fine.

# Augmentation

Augmentation is the artificial expansion of a training dataset (train) using various image transformations (rotations, flips, noise, color changes, etc.).

We take one image and create 3-5 new, slightly modified ones from it.

Changing the color scale doesn't change the image for a human eye; it remains essentially the same, but for a model, it's a different set of pixels. By performing simple transformations and applying filters (like those in Instagram), we increase the dataset exponentially.

This also helps the model be resilient to noise, unexpected angles, and various anomalies in the data.

