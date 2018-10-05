# datasets

[Datasets](#dataset) is a JSON-LD ```@context``` that you can use to publish a visual dataset of images to be used as input to computer vision classification and localization training pipelines.

Here is a concrete example:

```javascript
{
  "@context": "https://code.sgo.to/datasets",
  "@type": "Dataset",
  "name": "Dog breeds",
  "description": "Different breeds of dogs",
  "classes": [{
    "@type": "Class",
    "name": "Chihuahua",
    "images": [
      "http://code.sgo.to/dogs/images/n02085620-Chihuahua/n02085620_10074.jpg",
      "http://code.sgo.to/dogs/images/n02085620-Chihuahua/n02085620_10621.jpg"
    ]
  }, {
    "@type": "Class",
    "name": "Maltese",
    "images": [
      "http://code.sgo.to/dogs/images/n02085936-Maltese_dog/n02085936_10073.jpg",
      "http://code.sgo.to/dogs/images/n02085936-Maltese_dog/n02085936_10148.jpg"
    ]
  }]
}
```

# Dataset

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| name          | [String](#string)       | The name of the dataset                                          |
| description   | [String](#string)       | A short description about the dataset                            |
| url           | [String](#string)       | Where this dataset is to be found                                |
| download      | [String](#string)       | A link to a downloadable version of this dataset                 |
| citation      | [Bib](#bib)[]           | The citation requirements while using this dataset               |
| release       | [String](#string)       | The release number                                               |
| createdDate   | [Date](#date)           | The date the dataset was created                                 |
| publishedDate | [Date](#date)           | The date the dataset was published                               |
| modifiedDate  | [Date](#date)           | The date the dataset was last modified                           |
| classes       | [Class](#class)[]       | An array of classes in this dataset                              |
      
# Class

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| name          | [String](#string)       | The name of the class                                            |
| description   | [String](#string)       | A short description about the class                              |
| images        | [Image](#image)[]       | An array of images in this class                                 |

# Image

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| name          | [String](#string)       | The name of the class                                            |
| url           | [String](#string)       | The url with the bits of the image                               |
| size          | [Size](#size)           | The size of the image                                            |
| boxes         | [Box](#box)[]           | An array of bounding boxes where the class appears in the image  |

# Size

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| width         | [Number](#number)       | The width (in pixels) of the image                               |
| height        | [Number](#number)       | The height (in pixels) of the image                              |

# Box

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| left          | [Number](#number)       | The leftmost limit of the bounding box (in pixels)               |
| right         | [Number](#number)       | The rightmost limit of the bounding box (in pixels)              |
| top           | [Number](#number)       | The top limit of the bounding box (in pixels)                    |
| bottom        | [Number](#number)       | The bottom limit of the bounding box (in pixels)                 |

# Bib

A bib description.

# String

A text string.

# Date

A date value in ISO 8601 date format.

# Number

A numeric value.
