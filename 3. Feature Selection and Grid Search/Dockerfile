FROM python:3.6-onbuild

RUN pip install pip
RUN pip install pandas
#RUN pip install flask
RUN pip install scikit-learn
RUN pip install boruta
RUN pip install mlxtend  


COPY FeatureSelection.py /src/FeatureSelection.py
COPY requirements.txt /src/requirements.txt

#Run the command
CMD ["python", "./FeatureSelection.py"]