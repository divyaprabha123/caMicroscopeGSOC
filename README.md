## Browser based Object-Detection
### Coding Challenge GSOC-2020 - Cancer Region of Interest Extraction and Machine Learning
> This repo contains coding challenge for GSOC-2020 by caMicroscope.



## Code challenge
Using a machine learning toolkit of your choice, create a tool which identifies objects in the image, then returns positions in pixels corresponding to bounding boxes of a user-selected class of object in the image. For example, given an image with both cats and dogs, return bounding boxes for only cats.

## Approach
For this challenge I have built a browser based model with **Tensorflow.js** which allows the user to select the model and also the class. Tensorflow.js allows us to use machine learning directly in the browser as well as on the backend servers like Node.js. 

Tensorflow.js also provides pre-trained models to integrate with the web-app. The models are hosted on NPM and unpkg so they can be used in any project out of the box. They can be used directly or used in a transfer learning setting with TensorFlow.js. I have used **COCO-SSD**  model which detects objects defined in the COCO dataset.


## Installation

To set-up Tensorflow.js we can either use **script** tags or **NPM** with build tools like Parcel, WebPack, or Rollup. I have used npm with parcel to build js file

Steps:

```sh
npm install parcel-bundler
```

```sh
git clone https://github.com/divyaprabha123/caMicroscopeGSOC/
```

```sh
cd caMicroscopeGSOC
parcel index.html
```

Go to http://localhost:1234 to view
## Output Screenshot

### Image showing bounding box selected by user for cat 
![Alt text](https://github.com/divyaprabha123/caMicroscopeGSOC/blob/master/output/cat-bb.PNG)


### Image showing bounding box selected by user for Dog
![](https://github.com/divyaprabha123/caMicroscopeGSOC/blob/master/output/Dog-bb.PNG)

### Image showing bounding box selected by user for Person
![](https://github.com/divyaprabha123/caMicroscopeGSOC/blob/master/output/person-bb.PNG)
