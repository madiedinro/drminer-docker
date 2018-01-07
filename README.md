


## Запусе контейнера

Парметры:
`-o` адрес пула
`-u` кошелек
`-p` придумайте пароль для доступа к статистике по http
`--donate-level=` сколько жертвовать автору майнера
`--max-cpu-usage=` и так понятно
`--cpu-priority=` приоритет при дележке CPU. 2 - нормальный


    docker run -d \
         --name miner \
         --restart=always \
         drodin/xmrig xmrig -o pool.monero.hashvault.pro:5555 \
           --donate-level=1 \
           -u 49Zc576k5cFHSPnuvJrBGqE4ReKbpXZZbB4h8CeeFhmD7P5L9yzLSJ1KY4KcCun4pe2M3xvrNERnL1AWtKMEBYzhTLpt6nH \
           -p Ja4mee5Aing5 -k --max-cpu-usage=75 --cpu-priority=2
