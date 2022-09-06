# CovidFaceMaskDetection


## Running Preprocessing
`python src/preprocessing.py Data/orignal/`

`python src/preprocessing.py <Path/to/orignal/images> <Path/to/create/preprocessed/images>`

## Training model
`python src/training.py preprocess/`

`python src/training.py <Path/to/preprocess/images>`

## Training model with Restart
`python src/training.py preprocess/ models/model9.pth splitData.pkl`

`python src/training.py <Path/to/preprocess/images> <path/to/model/to/use> <path/to/data/file/with/data/split> <path/to/data/file/with/data/history> `

## Running model to classify
`python src/classify.py Data/orignal/Surgical_mask/ models/model9.pth `

`python src/classify.py <Path/to/dictory/of/images> <path/to/model/to/use>`



## Running model to analysis
`python src/analyze.py`
Need file in trainHistoryDict/data.pkl



`conda env create -f environment.yml`
