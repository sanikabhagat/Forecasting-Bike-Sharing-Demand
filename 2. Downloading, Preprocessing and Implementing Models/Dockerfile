FROM python:3.6-onbuild

RUN pip install pip
RUN pip install pandas
#RUN pip install flask
RUN pip install scikit-learn


COPY Preprocesing.py /src/Preprocesing.py
COPY requirements.txt /src/requirements.txt

#Run the command
CMD ["python", "./Preprocesing.py"]
