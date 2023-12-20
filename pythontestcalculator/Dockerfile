FROM python:3.6-slim

COPY . /pythontestcalculator
WORKDIR /pythontestcalculator

RUN /usr/local/bin/python -m pip install --upgrade pip && pip3 install --no-cache-dir -r requirements.txt
RUN ["pytest", "-v", "--junitxml=reports/result.xml"]

CMD tail -f /dev/null
