# build using "docker build . -t jupyter"

FROM python

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

LABEL Name=jupyter Version=0.0.1
EXPOSE 8000

WORKDIR /app

RUN pip install numpy pandas
RUN pip install matplotlib
RUN pip install jupyter

#run using  "docker run -p 8000:8000 jupyter"
CMD ["jupyter","notebook", "--ip","0.0.0.0","--port", "8000"  ,"--no-browser", "--allow-root"]


