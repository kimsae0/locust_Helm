FROM python:2.7

ADD locust-tasks /locust-tasks
ADD run.sh .

RUN pip install -r /locust-tasks/requirements.txt

EXPOSE 5557 5558 8089

RUN chmod 755 run.sh
ENTRYPOINT ["bash", "./run.sh"]