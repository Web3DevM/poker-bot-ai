# Poker Bot AI For Holdem

Hello! The project took a little over a month to complete.

I spent a week researching poker, writing notes, and getting a general understanding of the topic.

A week was spent writing the GUI (graphical user interface), creating the overall project architecture, and writing the code.

A week was spent on computer vision and preparatory work.

A week was spent training my YOLO models. I managed to train two models: one for table detection, the other for card detection.

Finally, a week was spent putting everything together, testing, fixing bugs, and compiling it into an executable file.

<img width="1560" height="616" alt="4bd738247d0d6041f2ecac8ec43b62ea" src="https://github.com/user-attachments/assets/e409ccb2-928f-4da1-ba5a-045185ab49cf" />


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

<img width="1560" height="781" alt="ef68e5ab0a2a2ddb048c20540f64257c" src="https://github.com/user-attachments/assets/779814a7-1bce-45f3-86dd-3e1d59d621c5" />

# Augmentation

Augmentation is the artificial expansion of a training dataset (train) using various image transformations (rotations, flips, noise, color changes, etc.).

We take one image and create 3-5 new, slightly modified ones from it.

Changing the color scale doesn't change the image for a human eye; it remains essentially the same, but for a model, it's a different set of pixels. By performing simple transformations and applying filters (like those in Instagram), we increase the dataset exponentially.

This also helps the model be resilient to noise, unexpected angles, and various anomalies in the data.

It took just over four weeks from the idea to a working prototype. I did everything myself: from the project structure and mathematics to the recognition models and interface. AI tools helped at every step: in some cases they sped up the work, in others they suggested solutions, but I still had to guide and refine everything manually.

In the end, I created an MVP that actually works: it sees cards, understands the board situation, calculates EV, and suggests actions.

![316507960-5831544b-14c2-412c-acb0-a72d67a3c589](https://github.com/user-attachments/assets/fd8fd7ab-c0e0-4a81-9279-a91db06bdd05)

