FROM python:3.7-stretch

#install modules
RUN pip install Flask

#Needed by flask module
ENV FLASK_APP=server.py 

#Copy source files into image
COPY templates ./templates
COPY server.py .

EXPOSE 5000 

CMD ["flask","run", "--host=0.0.0.0"]