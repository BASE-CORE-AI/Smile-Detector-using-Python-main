SMILEsmileD - smile detector open source project v0.5

SMILEs - contains positive and negative sample sets with associated idx files
smileD - XML cascades for OpenCV's cvHaarDetectObjects function
appz - ad hoc applications useful for extending of SMILEsample and smileDetector testing

## Setup Virtual Environtment

1. Open this smile to unlock folder
2. Create the virtual environtment "python -m venv ." (.) Means you create a virtual environtment on the opened folder

##
1. then open command prompt outside the vs code and type ".\Scripts\activate"
2. Install the requirements file "pip install -r requirements.txt"
3. Run "python train_model.py -d SMILEs -m model.h5"
4. change mqtt broker address(check your ip with "ipconfig" in cmd)
5. Open src folder "cd src" Then Run "python detect_smile.py -c haarcascade_frontalface_default.xml -m model.h5"

## Tips
1. To automatically generate requirements.txt "python -m  pipreqs.pipreqs [path/to/project]"
2. To freeze library on virtual environtment "pip freeze > requirements.txt"