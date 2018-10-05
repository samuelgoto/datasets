# datasets

Putting aside a lot of additional metadata, the skeleton of a dataset is the following:

- dataset ([Dataset](Dataset.md))
  - name ([String](String.md))
  - description ([String](String.md))
  - download ([String](String.md))
  - classes ([Class](Class.md)[])
    - name ([String](String.md))
    - images ([Image](Image.md))
      - size ([Size](Size.md))
      - box ([Box](Box.md))
