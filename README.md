# datasets

Datasets is a JSON-LD ```@context``` that describes a visual dataset of images to be used as input to computer vision classification and localization training pipelines.

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

The basic skeleton of a dataset follows this structure:

- dataset ([Dataset](Dataset.md))
  - name ([String](String.md))
  - description ([String](String.md))
  - download ([String](String.md))
  - classes ([Class](Class.md)[])
    - name ([String](String.md))
    - images ([Image](Image.md))
      - size ([Size](Size.md))
      - box ([Box](Box.md))
      

