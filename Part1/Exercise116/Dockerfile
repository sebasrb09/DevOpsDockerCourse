FROM python:3.9-slim

WORKDIR /app

RUN apt-get update
RUN pip install --upgrade pip
COPY . .
#COPY requirements.txt /app/
RUN pip install -r requirements.txt
#COPY . /app/

#EXPOSE 8501

#ENTRYPOINT [ "streamlit", "run" ]
CMD streamlit run src/Colfuturo.py --server.port $PORT
#ENTRYPOINT [ "streamlit", "run" ,"src/Colfuturo.py","--server.port="]
#CMD ["src/Colfuturo.py","--server.port=8501", "--server.address=0.0.0.0"]