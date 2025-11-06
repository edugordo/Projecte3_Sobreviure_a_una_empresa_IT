# 🧭 **P04: Documentació Servidor DNS**

## 📝 **Breu descripció**

Molt benvinguts a la vostra nova tasca, consultors! 👋

Com a membres de l'equip de sistemes d'**EverPia**, us heu enfrontat al repte de configurar un **servidor de noms (DNS)** com a prova de concepte pel nostre client **Digicore**, però ara mateix el resultat de la vostra feina es troba en una màquina virtual.

🎯 L’objectiu és poder **publicar aquestes configuracions a GitHub**, d’aquesta manera assegurem que, quan es vulgui replicar la configuració, no caldrà començar des de zero.
Només caldrà descarregar els arxius dins del servidor Linux triat i reiniciar el servei per tenir el servidor completament operatiu. ⚙️

---

## 🚀 **Fase 1: Preparació de la Connectivitat i Extracció dels Arxius**

Per poder copiar fitxers de la vostra màquina virtual **Ubuntu Server** a la vostra màquina física (host), heu d'assegurar la **connectivitat de xarxa**.

---

### 🔌 **Pas 1.1: Configuració de la Interfície Host-Only**

* **Afegir la Interfície Virtual:**
  A la configuració de la vostra màquina virtual Ubuntu Server, afegiu una **segona interfície de xarxa** i assigneu-li el **mode Host-Only**.

* **Configureu-la i activeu-la.**

* **Comproveu la connectivitat** des de la màquina física.

---

### 🔒 **Pas 1.2: Còpia Segura dels Fitxers Clau amb SCP**

Un cop establerta la connectivitat **Host-Only**, utilitzareu el protocol **SCP (Secure Copy Protocol)**, que és segur i ve inclòs amb el servei **SSH**, per transferir els fitxers de configuració a la vostra màquina física.

📁 **Els arxius a copiar són els següents:**

```
/etc/bind/named.conf.options
/etc/bind/named.conf.local
/etc/bind/zones
```

💻 **Per copiar els arxius a la màquina física**, cal obrir un terminal al PC i executar la comanda `scp`.

👉 *El punt (.) al final de la comanda indica que l’arxiu es copiarà al directori actual de la vostra màquina física.*

---

## 🌐 **Fase 2: Integració a GitHub**

---

### 📂 **Pas 2.1: Crear carpeta i arxiu `README.md`**

El primer pas serà crear la carpeta **`producte04`** i el seu arxiu **`README.md`**.
Recordeu que la carpeta es crea automàticament en donar a l’opció **New File** i en el nom indicar que es troba dins una carpeta (exemple: `producte04/README.md`).

📘 A l’arxiu `README.md`, a més de posar el **títol del producte**, cal fer una **explicació del contingut**.

---

### ☁️ **Pas 2.2: Pujar arxius**

Procediu a **pujar els diversos arxius**, tenint en compte que haureu de crear la carpeta **`zones`** prèviament a pujar els arxius de les zones.

💡 Podeu usar el procediment següent:

1. Crear un fitxer anomenat `zones/esborrar`.
2. Pujar els arxius de zones al repositori.
3. Un cop pujats, esborreu el fitxer `zones/esborrar`.

---

## 🎯 **Objectius específics de la tasca / Finalitat de la tasca**

Usar **GitHub** per **documentar configuracions de servidors**, valorant els avantatges de poder **replicar configuracions de forma ràpida i segura** (*repetitibilitat*). 🧩

---

✨ *Aquesta tasca fomenta la documentació tècnica, la col·laboració i la reutilització de configuracions dins d’un entorn professional.*

---

✅ [Guia](guia.md)
