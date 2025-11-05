# UD4.AA2 Instal·lació OpenLDAP

---

![](IMG/1.png)

Configurem el nom del servidor perque tingui nom de domini

---

![](IMG/2.png)![](IMG/3.png)

Per comunicar-se amb el client, configurarem el primer adaptador amb "Xarxa NAT", mentre que el segon adaptador el posarem en "Amfitrió" per la gestió web des de la màquina

---

![](IMG/4.png)![](IMG/5.png)

Instal·lem el servei LDAP i les seves utilitats per fer proves

---

![](IMG/6.png)

Comprovem que el servei esta funcionant amb la comanda **"systemctl status slapd"**

---

![](IMG/7.png)

![](IMG/8.png)
--
![](IMG/9.png)![](IMG/10.png)![](IMG/11.png)![](IMG/12.png)![](IMG/13.png)![](IMG/14.png)
Comprovem que el directori s'ha creat amb el nom correcte, en cas que ens haguem equivocat en la configuració, amb la comanda **"dpkg-reconfigure slapd"**, podem tornar a configurar el nom que volem, en cas que no haguem fet bé la configuració anterior. Si podem la comanda, haurem de segui la següent configuració per posar el nom del domini correctament

---

![](IMG/15.png)![](IMG/16.png)

El format *.ldif* es el predeterminat per declarar objectes al directori. **"ldapadd"** Permet afegir elements al directori que li indiquem en la comanda

---

![](IMG/17.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---

### Altres Comandes. ***"ldap-utils"***
- **ldapdelete:** Per eliminar objectes dins del directori que li inf¡diquem en la comanda, també es po teliminar el propi directori amb aquesta utilitat
- **ldappasswd:** Serveix per canviar la contrassenya d'un usuari
- **ldapmodify:** Serveix per editar una entrada ja existent dins del directori

---

# UD4.AA3 Configuració directori usant LAM

---

![](IMG/18.png)

Descarregan directament el paquet sencer del gestor, s'ens descarregaràn totes les dependències necessaries

---
![](IMG/19.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/20.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/21.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/22.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/23.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/24.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/25.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/26.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/27.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/28.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/29.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/30.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/31.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/32.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/33.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/34.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/35.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---
![](IMG/36.png)

**"ldapsearch"** Serveix per fer consultes i buscar dins del directori que li indiquem en la comanda

---

# UD4.AA4 Autentificació utilitzatnt LDAP

---
