1:
docker build -t nginx .
docker run -d -p 80:80 --name nginx1 nginx




2:
docker build -t api .
docker run -d -p 8000:8000 --name stocks_gun api