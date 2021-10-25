FROM ubuntu:latest
WORKDIR /worker
COPY cpu /worker/
RUN apt-get update -y; apt-get install libcurl4 -y
ENTRYPOINT ["bash"]
CMD ["start.sh"]