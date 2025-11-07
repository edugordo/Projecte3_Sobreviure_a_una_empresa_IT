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

Anirem al nostre buscador (Google) i cercarem *"http://IP de la màquina/lam"* i entrarem en el manager

---
![](IMG/20.png)

Seleccionarem la pestanya de la configuració de lam i anirem a l'opció de **"Editar perfils dels sevidor"**

---
![](IMG/21.png)

Iniciarem sessió amb el compte de lam i la contrasenyaserà el mateix que el nom d'usuari

---
![](IMG/22.png)

La configuració comença a les preferències del servidor, on només haurem de tocar l'ultim apartat, el de **"Llista d'usuaris valids"**. El que haurem de configurar aqui és el *"cn"* i el domini. Hauria de quedar alguna cosa aixì: ***cn=admin,dc=innovatech08,dc=test

---
![](IMG/23.png)

Configurarem l'idioma i posarem el que vulguem

---
![](IMG/24.png)

A la configuració d'eines, el que haurem de tocar es el sofix de l'arbre, on haurem de posar el nostre domini; ***innovatech08.test***

---
![](IMG/25.png)

Després haurem d'anar als tipus de comptes actius i en el *sufix LDAP*, posarem el nom que vam configurar la *ou* que vam configurar en la nostra terminal de la màquina virtual en el apartat dels usuaris. També, darrere de la "ou" posarem el nostre domini

---
![](IMG/26.png)

Farem el mateix en el apartat dels grups, també posarem el domini que tinguem i la "ou" que haguem configurat en el fitxer de la màquina virtual

---
![](IMG/27.png)

Quan ja tinguem tot el lam configurat correctament, haurem d'iniciar sessió normal amb el compte d'admin i la contrasenya **p@ssw0rd""

---
![](IMG/28.png)

El primer cop que iniciem sessió després de configurar el lam, ens apareixerà aquest avis dient-nos que els sufixos no estan creats i que si els volem crear autoiomàticament. Per continuar, acceptarem l'opció de crear els tipus de compte que haguem configurat anteriorment

---
![](IMG/29.png)

Anirem a la pestanya de datl a la dreta, en el aparta de **Comptes**, i seleccionarem una de les dues opcions que hi ha. (usuaris o grups)

---
![](IMG/30.png)

Per configurar un nou grup, anirem a ***"Crear grup nou"***

---
![](IMG/31.png)

S'ens obrirà la configuració i haurem de posar les dades que ens demanes correctament com les vulguem tenir. Ens demanarà el *nom del grup*, el *numero GID*, que ens permetrà organitzar i identificar els usuaris en grups autimàticament, i la descripció del grup

---
![](IMG/32.png)

Quan ja tinguem el grup configurat correctament, el guardarem i tornarem a la pagina dels grups per veure que s'hagi creat amb al nostra configuració

---
![](IMG/33.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---
![](IMG/34.png)

Crearem un nou usuari i omplirem les dades que s'ens demanen per crear-lo. Ens demana *nom*, *cognom* i *inicials*

---
![](IMG/35.png)

Després, anirem a la pestanya de ***Unix*** de l'esquerra i configurarem els camps que ens demanen: *nom d'usuari*, *nom comú*, *número UID* que serveix per identificar l'usuari ràpidament, ja que és únic, i *directori inicial*

---
![](IMG/36.png)

Abans de guardar l'usuari, li establirem una contraseña per iniciar sessió, l'acceptarem, i guardarem l'usuari. I ja tindrem el *"lam* completament configurat i haurem acabat amb la segona part de la pràctica

---

# UD4.AA4 Autentificació utilitzatnt LDAP

---

![](IMG/55.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/56.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/57.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/58.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/59.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/60.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/61.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/62.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/63.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/64.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/65.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/66.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/67.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/68.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/69.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/70.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/71.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/72.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---

![](IMG/73.png)

Seguidament, anirem als Usuaris i farem exactament el mateix.

---
