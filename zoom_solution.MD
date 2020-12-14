## C помощью утилиты dig найдите 5 компаний (доменов), которые скорее всего используют Zoom для своей работы.

Решение:

В качестве источника для поиска компаний, я загуглил список 500 крупнейши компаний с их доменами.

Скопировал список доменов вот отсюда: https://dofo.com/blog/fortune-500-domain-names/. И поместил их в файл `domains`, т.к. dig умеет доставать домены из файла.

Дальше запустил команду (+ вывод, + фильтр по записям):
```
$ dig @8.8.8.8 txt -f domains +noall +answer | grep ZOMM

adm.com.                3599    IN      TXT     "ZOOM_verify_Bt8mIqWMQFuX5fBQkUsSbA"
nike.com.               299     IN      TXT     "ZOOM_verify_sCcWC00VT72Xd3cKn3ByDQ"
pmi.com.                12050   IN      TXT     "ZOOM_verify_LWymrHJkQeObJRpDuiFXrA"
abbvie.com.             3599    IN      TXT     "ZOOM_verify_aqYKculqR_S-RdMwpmh36g"
bms.com.                299     IN      TXT     "ZOOM_verify_mpvT1IQeSsaGE3DZoIvaUA"
lear.com.               3599    IN      TXT     "ZOOM_verify_zwhP2yU2TsCLeP4JTV8CtA"
danaher.com.            299     IN      TXT     "ZOOM_verify_iksXTjB5TsaeRbFA1dX1eQ"
principal.com.          3599    IN      TXT     "ZOOM_verify_Hsm4IZ3JTI21CjmnuUXGWA"
loews.com.              3599    IN      TXT     "ZOOM_verify_i36oHs6jS9ifgy24o-LWMA"
celgene.com.            3599    IN      TXT     "ZOOM_verify_TyFh0oiNRPC77FQQj7OTog"
rgare.com.              299     IN      TXT     "ZOOM_verify_bq7KUAvkR0mzpfO-8eHE_g"
mastercard.com.         899     IN      TXT     "ZOOM_verify_5iqN50tCRjWyMgQa3G__uQ"
blackrock.com.          299     IN      TXT     "ZOOM_verify_FsOJw095SMyypVXs8wlBQQ"
blackrock.com.          299     IN      TXT     "ZOOM_verify_u51YW9QoScOHBUzIhbDgtg"
ameriprise.com.         299     IN      TXT     "ZOOM_verify_dnZFy8rkSwed1MK-1fF84Q"
csx.com.                3599    IN      TXT     "ZOOM_verify_36KTVdvYS-qd1ZHoEZB2jw"
l3t.com.                599     IN      TXT     "ZOOM_verify_vUycL7IlTpaqJtdqtkegbg"
steeldynamics.com.      3599    IN      TXT     "ZOOM_verify_L2SVdKpBQVWTZZ-MLD1NkQ"
pacificlife.com.        599     IN      TXT     "ZOOM_verify_EBABr03oT-GWeUuOmYzPvw"
airproducts.com.        3599    IN      TXT     "ZOOM_verify_65S9aKaBTt-WQiqQbEYukQ"
newscorp.com.           59      IN      TXT     "ZOOM_verify_u5sJgPlcTwOWElmcBkLaEQ"
jll.com.                299     IN      TXT     "ZOOM_verify_sk_U0VwnRoO4w1kTnm06Pg"
activisionblizzard.com. 3599    IN      TXT     "ZOOM_verify_BHzUTWLHQXKgXasCp0AyvA"
harris.com.             3599    IN      TXT     "ZOOM_verify_Ngh9oo3rQL-CWBGe1x86mQ"
ralphlauren.com.        299     IN      TXT     "ZOOM_verify_fAoE2GPRS-asSUzTOodkqQ"
oldrepublic.com.        9       IN      TXT     "ZOOM_verify_Y4Ptof38QDSYGsAqrVHFeg"
pattersoncompanies.com. 299     IN      TXT     "ZOOM_verify_nRm6cPOiRk-uDxK6zTaQ8w"
```

---
