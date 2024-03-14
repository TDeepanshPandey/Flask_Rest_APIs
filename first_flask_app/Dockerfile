FROM python:3.10
WORKDIR /app
COPY requirement.txt .
RUN pip install -no-cache-dir --upgrade -r requirement.txt
COPY . .
#CMD ["flask", "run", "--host", "0.0.0.0"]
CMD ["gunicorn","--bind", "0.0.0.0:80", "app:create_app()"]