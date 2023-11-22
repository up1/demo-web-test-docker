FROM python:3
WORKDIR /app
COPY requirement.txt .
RUN --mount=type=cache,target=/root/.cache/pip pip install -r requirement.txt
COPY . .
CMD [ "robot", "-d", "/app/report/", "*.robot" ]