# Gerador de QRCodes para Contatos

Script desenvolvido em Python para gerar vários QRCodes a partir de uma lista de contatos.

## Como Usar

Os dados de cada contato devem ser preenchidos no arquivo CSV _"contatos.csv"_ com os seguintes campos:

> EMPRESA;NOME;EMAIL;CARGO;TELEFONE;SITE

Executar:

```
python src/main.py
```

Os QR Codes serão gerados e salvos na pasta _"qrcodes_gerados"_.

## Referências

Python qrcode:

-   https://pypi.org/project/qrcode/

Gerador de QRCode:

-   https://www.online-qrcode-generator.com/qrcode-generator
-   https://www.qr-code-generator.com/

Leitor de QRCode:

-   https://www.online-qr-scanner.com/
-   https://webqr.com/index.html

Tutoriais:

-   https://www.geeksforgeeks.org/generate-qr-code-using-qrcode-in-python/
-   https://youtu.be/RsN0aXfPR1E

VCARD Format:

-   https://en.wikipedia.org/wiki/VCard

## Exemplos

Para este CSV:

```
EMPRESA;NOME;EMAIL;CARGO;TELEFONE;SITE
Near Location;Erik Lima;erik.lima@nearlocation.com.br;Tech Lead;48 3233-1031;www.nearlocation.com.br
```

É criado este VCARD:

> BEGIN:VCARDVERSION:3.0TEL;WORK;VOICE:48 3233-1031URL:www.nearlocation.com.brEMAIL:erik.lima@nearlocation.com.brFN:Teste TestandoORG:Near LocationTITLE:Tech LeadEND:VCARD

Que gera este QR Code:

![QR Code](<qrcodes_gerados/Erik Lima.png> "Erik Lima")

Que corresponde a este Contato:

    Erik Lima
    Número: 48 3233-1031 (WORK)
    E-mail: erik.lima@nearlocation.com.br
    Empresa: Near Location
    Título: Tech Lead
    URL: www.nearlocation.com.br
