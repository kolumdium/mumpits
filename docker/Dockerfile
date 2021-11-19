FROM continuumio/miniconda3

WORKDIR /app/

RUN apt-get update
RUN apt-get install ffmpeg -y

RUN git clone https://github.com/kolumdium/Mumpits.git

RUN conda install -c conda-forge discord.py[voice] python-dotenv youtube-dl ffmpeg pynacl

CMD [ "python", "Mumpits/main.py" ]
