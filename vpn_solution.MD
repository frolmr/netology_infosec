## Какая версия OpenSSL используется

`OpenSSL 1.1.1f 31 Mar 2020`

---

## Какой алгоритм (и с какой длиной ключа) используется для шифрования

`BF-CBC` c длиной ключа 128 бит

---

## Какой алгоритм (и с какой длиной ключа) используется дла HMAC аутентификации

`SHA1` с длиной ключа 160 бит

---

## Что будет выведено в консоли сервера (`sudo openvpn --ifconfig 10.1.0.1 10.1.0.2 --dev tun --secret vpn.key --cipher AES128 --auth SHA256 --verb 3`), если:

### Подключиться с клиента командой: `sudo openvpn --ifconfig 10.1.0.2 10.1.0.1 --dev tun --remote 10.0.0.1 --secret vpn.key --cipher AES256 --auth SHA256 --verb 3`

```
Authenticate/Decrypt packet error: cipher final failed
```

### Подключиться с клиента командой: `sudo openvpn --ifconfig 10.1.0.2 10.1.0.1 --dev tun --remote 10.0.0.1 --secret vpn.key --cipher AES128 --auth SHA512 --verb 3`

```
Authenticate/Decrypt packet error: packet HMAC authentication failed
```
