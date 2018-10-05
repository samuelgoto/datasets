# datasets

# Dataset

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| name          | [String](#String)       | The name of the dataset                                          |
| description   | [String](#String)       | A short description about the dataset                            |
| url           | [String](#String)       | Where this dataset is to be found                                |
| download      | [String](#String)       | A link to a downloadable version of this dataset                 |
| citation      | [Bib](#Bib)[]           | The citation requirements while using this dataset               |
| release       | [String](#String)       | The release number                                               |
| createdDate   | [Date](#Date)           | The date the dataset was created                                 |
| publishedDate | [Date](#Date)           | The date the dataset was published                               |
| modifiedDate  | [Date](#Date)           | The date the dataset was last modified                           |
| classes       | [Class](#Class)[]       | An array of classes in this dataset                              |

# Class

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| name          | [String](#String)       | The name of the class                                            |
| description   | [String](#String)       | A short description about the class                              |
| images        | [Image](#Image)[]       | An array of images in this class                                 |

# Image

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| name          | [String](#String)       | The name of the class                                            |
| url           | [String](#String)       | The url with the bits of the image                               |
| size          | [Size](#Size)           | The size of the image                                            |
| boxes         | [Box](#Box)[]           | An array of bounding boxes where the class appears in the image  |

# Size

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| width         | [Number](#Number)       | The width (in pixels) of the image                               |
| height        | [Number](#Number)       | The height (in pixels) of the image                              |


# Box

| Property      | Type                    | Description                                                      |
| ------------- |:-----------------------:| :----------------------------------------------------------------|
| left          | [Number](#Number)       | The leftmost limit of the bounding box (in pixels)               |
| right         | [Number](#Number)       | The rightmost limit of the bounding box (in pixels)              |
| top           | [Number](#Number)       | The top limit of the bounding box (in pixels)                    |
| bottom        | [Number](#Number)       | The bottom limit of the bounding box (in pixels)                 |


# Bib

# String

# Date
