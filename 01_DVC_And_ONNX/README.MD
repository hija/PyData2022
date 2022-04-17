# Data Version Control
![https://dvc.org/](https://dvc.org/img/dvc_icon-color--square_vector.svg)

**Data Version Control** is an approach to version control data, such as the training data, but also models in a similiar fashion as git is being used to version control source code.

DVC installs via brew (`brew install dvc`) which is a big plus for me, since it makes it easy to install and uninstall the DVC.


These are the talks / tutorials I watched regarding Dask:

| Name                                                                            | Author           | Link                                         |
| ------------------------------------------------------------------------------- | ---------------- | -------------------------------------------- |
| Flexible ML Experiment Tracking System for Python Coders with DVC and Streamlit | Antoine Toubhans | [🔗](https://2022.pycon.de/program/RTPEWV/) |

# Open Neural Network Exchange
![https://onnx.ai/](https://upload.wikimedia.org/wikipedia/commons/c/c0/ONNX_logo_main.png)

The ONNX is a format for machine learning models. Personally, I used to export my models with pickle and joblib, however, this has major drawbacks, e.g. it is very prone to vulnerabilities and it is not interchangable with other programming langauges.

The **Open Neural Network Exchange** format saves the structure, weight and further information in a serialized data format which can be used in a variety of programming languages. Additionally, it seems to be less prone to vulnerabilities than pickle. With the format, you could, for example, build your machine learning model in Python with scikit-learn and later use it in CoreML in your iOS app.