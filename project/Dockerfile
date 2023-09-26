FROM python:3.8
LABEL maintainer="tonydev93"
EXPOSE 3111

COPY ./techtrends /techtrends
WORKDIR /techtrends

RUN pip install -r requirements.txt
RUN python init_db.py

# command to run on container start
CMD [ "python", "app.py" ]
