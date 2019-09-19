FROM python:3.6-onbuild

RUN pip install pip
RUN pip install pandas
#RUN pip install flask
RUN pip install scikit-learn 

COPY static /src/static
COPY templates /src/templates
COPY app.py /src/app.py
COPY requirements.txt /src/requirements.txt
COPY RF_Reg.pkl /src/RF_Reg.pkl

EXPOSE 5000

ENTRYPOINT ["python"]

#Run the command
CMD ["app.py"]