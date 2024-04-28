FROM python:3.10-slim-buster


WORKDIR /nadia

COPY requirements.txt ./

RUN pip install --no-cache-dir --upgrade pip \
    && pip install --no-cache-dir -r requirements.txt

COPY nadia/ .

EXPOSE 5000

CMD ["python", "manage.py", "runserver", "0.0.0.0:5000"]