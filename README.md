(This project is not maintained.)
## DataTransformer
A simple tool for **Data Splitting** and **Data Encoding**.

## Usage
For **Data Processing**:
```python
python DataProcess.py -task [Task] -infile [InputFile] -outfile [Outputfile] [Options]
```
For **Data Encoding**:
```python
python DataEncode.py -task [Task] -infile [InputFile] -outfile [Outputfile] [Options]
```
Since no third-party package is used in this tool, so it supports [**pypy**](http://pypy.org/) for fast execution.
```python
pypy DataProcess.py -task [Task] -infile [InputFile] -outfile [Outputfile] [Options]
pypy DataEncode.py -task [Task] -infile [InputFile] -outfile [Outputfile] [Options]
```
More parameter options can be found in `--help` or wiki page (not finished for now).
```python
python main.py --help
```

## File Format
* [**File Format**](https://github.com/chihming/DataTransformer/wiki/File-Format)

## Supported Task
**DataProcess.py**
* [**dsplit**](https://github.com/chihming/DataTransformer/wiki/dsplit) -- split data into train & test
* [**djoin**](https://github.com/chihming/DataTransformer/wiki/djoin) -- join relational feature to data

**DataEncode.py**
* [**data2sparse**](https://github.com/chihming/DataTransformer/wiki/data2sparse) -- convert **general** data into **sparse** data format
* [**data2rel**](https://github.com/chihming/DataTransformer/wiki/data2rel) -- convert **general** data into **relational** data format

## TODO Task
* **sparse2rel** -- convert **sparse** data into **relational** data format
* **data2vw** -- convert **general** data into [Vowpal Wabbit](https://github.com/JohnLangford/vowpal_wabbit) (VW) data format
* **sparse2vw** -- convert **sparse**  dataformat into VW format
* **vw2sparse** -- convert VW dataformat into **sparse**  format

## Supported Encoding Method
* `-cat` -- like one-hot encode, usually for categorical feature (supports for multi-labeled features)  
* `-num` -- directly use the value, usually for numerical data
* `-knn` -- automatically get similar features as meta features


## TODO Encoding Method
* `-wcat` -- encode multi-labeled features with different weights

## Demo
* [**Movielens 1M/10M**](https://github.com/chihming/DataTransformer/wiki/Movielens-Dataset)


