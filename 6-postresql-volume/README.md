docker run --name postgres-demo -d -v /home/vasa/data:/data/ps postgres - делаем первый bind mount 
docker stop postgres-demo - останавливаем контейнер
ls /home/vasa/data - просматриваем содержимое каталога
mv /home/vasa/data /home/vasa-1/data - переносим каталог
docker run --name postgres-demo-2 -d -v /home/vasa-1/data:/data/ps postgres - запускаем второй контейнер с новым каталогом