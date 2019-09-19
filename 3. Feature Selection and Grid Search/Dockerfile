FROM python:3.6-onbuild

#Installing dependencies
RUN pip install pip
RUN pip install pandas
RUN pip install boto
RUN pip install boto3
RUN pip install Boruta
RUN pip install mlxtend
RUN pip install luigi
#RUN pip install urllib
RUN pip install scikit-learn


COPY train.csv /src/train.csv
COPY test.csv /src/test.csv
COPY FeatureSelection.py /src/FeatureSelection.py
COPY requirements.txt /src/requirements.txt

#Run the command
CMD ["python", "./FeatureSelection.py"]