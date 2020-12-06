## Задание Firewall

```
$ sudo ufw status verbose

Status: active
Logging: on (low)
Default: deny (incoming), allow (outgoing), disabled (routed)
New profiles: skip

To                         Action      From
--                         ------      ----
80/tcp                     ALLOW IN    Anywhere
22/tcp                     ALLOW IN    Anywhere
80/tcp (v6)                ALLOW IN    Anywhere (v6)
22/tcp (v6)                ALLOW IN    Anywhere (v6)
```

---

## Задание Wireshark

Когда на фаерволе порт закрыт не происходит тройного рукопожатия. Kali пытается отправить сегмент с флагом SYN и не получает ничего в ответ (строка с этой записью в Wireshark окршивается черным). В том случае, когда на файерволе порт открыт, тройное рукопожатие происходит, Kali посылает сегмент с флагом SYM, в ответ получает [SYN, ACK] и подтверждает сегментом с флагом ACK, т.е. соединение устанавливается и далее следует запись с уже протоколом FTP.
