FROM python:3.6
RUN mkdir /opt/myflaskapp
WORKDIR /opt/myflaskapp
COPY requirements.txt /opt/myflaskapp
RUN pip install --no-cache-dir -r requirements.txt
COPY . /opt/myflaskapp
CMD ["python3.6", "app.py"]

# docker build -t flask_app_server:1.0 .
