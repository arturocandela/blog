---
date: 2026-02-13
authors:
  - arturo
categories:
  - Seguretat
  - Docker
  - DevOps
tags:
  - TPM
  - LUKS
  - GPG
  - Docker
  - Laravel
  - Caddy
---

# 🔐 Hui ha tocat seguretat, claus i un poc de Docker

<!-- more -->

Hui ha sigut un dia d'eixos que no fan soroll, però que deixen les coses ben apretadetes.

He estat tocant la part de xifrat, tokens, empremta, GPG… i també avançant amb la intranet dockeritzada. No és espectacular, però és feina de la que dona tranquil·litat.

---

## 🔒 Xifrat amb TPM i tokens

He revisat la configuració de LUKS amb `systemd-cryptenroll`, mirant bé com estan muntats:

* El TPM2
* El token FIDO
* Els keyslots
* Les condicions d’arrencada

La qüestió no és només que el disc estiga xifrat. La qüestió és saber **quan es desbloqueja i per què**.

He deixat el TPM configurat més bé estricte. Si algú toca el kernel, la cadena d’arrencada o alguna cosa rara, que no arranque i punt.

Preferisc que es queixe el sistema abans que jo.

---

## 🖐️ Empremta dactilar

També he estat ajustant la part de l’empremta.

No com a substitut de la contrasenya —que això seria massa còmode— sinó com una capa més.

La biometria mola, però m’interessa més entendre com encaixa amb la resta. No vull coses “màgiques” que funcionen perquè sí.

---

## 🔑 GPG i firmar commits com toca

He fet neteja de claus GPG, he revisat UIDs i he deixat configurada la signatura automàtica en Git.

```bash
git config --global user.signingkey TU_CLAVE
git config --global commit.gpgsign true
```

Firmar commits no costa res i et deixa les coses ben fetes des del principi.

És com signar el que fas. Si el codi és teu, que es note.

---

## 🐳 Intranet amb Docker

En paral·lel he seguit amb la dockerització de la intranet.

Imatge:

```
arturocandela/intranet:laravel11-dev
```

Branca:

```
feature/dockerIntegration
```

Ara mateix ja pots clonar i fer:

```bash
docker compose up
```

I tens:

* Laravel 11
* HTTPS amb Caddy
* Ports 80 i 443
* Base preparada per a Selenium

Encara queda polir el correu i algun detall, però ja no és un experiment. Ja és usable.

I això em deixa tranquil.

---

## 📝 El blog

També he anat afinant el blog en:

👉 [https://arturocandela.github.io/blog/](https://arturocandela.github.io/blog/)

MkDocs, Material i GitHub Actions. Cada `push`, publicat. Sense històries.

M’agrada que les coses siguen simples i que funcionen.

---

## 🧩 I ja està

Hui no ha sigut dia de grans virgueries.

Ha sigut dia d’ajustar, revisar i deixar-ho tot un poc més fi.

Potser d’ací isca un projecte més ben pensat. O potser no. De moment volia entendre bé les peces abans de muntar res damunt.

I amb això, ja vaig bé.

