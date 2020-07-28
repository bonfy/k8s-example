FROM python:3.7-alpine

WORKDIR /app
ADD . /app
RUN pip install -r req.txt

EXPOSE 5000
CMD ["python", "app.py"]