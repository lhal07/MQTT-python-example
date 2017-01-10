Exemplo de troca de mensagens utilizando MQTT
=============================================

Para este exemplo utilizaremos como broker o [Mosquitto](mosquitto.org). Basta
instalá-lo e rodar normalmente utilizando o comando

``` bash
$ mosquitto
```

Para executar o cliente MQTT desenvolvido em python instale a lib paho-mqtt.

Em seguida temos apenas que executar uma instância do cliente que atuará como
servidor ouvindo as mensagens e outra que atuará enviando as mensagens.

Para o servidor execute:

``` bash
$ python simple_client.py --serve
```

Envie mensagens para o servidor utilizando o comando:

``` bash
$ python simple_client.py --send
```

Ele irá requisitar uma mensagem para ser enviada.

O código utilizado foi encontrado em [https://blog.butecopensource.org/mqtt-parte-2-enviando-e-recebendo-mensagens/]
