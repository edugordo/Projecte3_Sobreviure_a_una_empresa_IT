## Explicació de la Tasca

---

## T01: Gestor de contrasenyes

## 🔔 Descripció de la tasca:

**Alerta!!** EverPia ha estat atacada per ciberdelinqüents.  
La consultora on esteu de becaris ha patit una **fuita d’informació (data breach)** i informació confidencial sobre un projecte en desenvolupament està ara en mans de delinqüents que amenacen amb publicar-la si no es paga un rescat.

Aquesta situació ha causat una **gran alarma dins la companyia**, i s’ha creat un **comitè de crisi** per gestionar-la.

La investigació interna ha revelat que **un dels comptes tècnics va ser compromès** a causa de l'ús d'una **contrasenya feble o reutilitzada**.

---

## 🧭 Directriu de la Direcció Tècnica

Com a resposta a aquesta crisi, la Direcció Tècnica ha emès la següent directriu:

> Tot el personal tècnic ha de començar a utilitzar un **gestor de contrasenyes validat** per garantir l'ús de credencials úniques i robustes.

Se us encarrega la tasca d’**avaluar les opcions i crear la documentació necessària** per a la formació del personal tècnic.

---

## 📘 Fase 1: Anàlisi i Justificació (Document d'Informe)

Heu de redactar un **informe tècnic** que justifiqui la decisió de la Direcció i compari les opcions disponibles.  
Aquest informe ha d'incloure:

### 1. Introducció i Justificació
- Explicació de **per què les contrasenyes febles o reutilitzades** són un risc crític per a l'empresa (atac de diccionari, *credential stuffing*, etc.).
- Descripció de la **funció crucial d'un gestor de contrasenyes** per mitigar aquests riscos.

### 2. Comparativa Tècnica
Realitzeu una **taula comparativa detallada** entre les següents opcions:

#### 🔹 Bitwarden (Alternativa Online / Núvol)
Analitzeu:
- Sincronització  
- Model de seguretat (xifratge *end-to-end*)  
- Facilitat d'accés des de múltiples dispositius  
- Cost / model *freemium*

#### 🔹 KeePassX / KeePassXC (Alternativa Offline / Escriptori)
Analitzeu:
- Emmagatzematge local de l'arxiu (`.kdbx`)  
- Independència del núvol  
- Model *open source*  
- Portabilitat de l'arxiu

### 3. Avantatges i Inconvenients
Resumiu els principals **pros i contres** de cada model (*online* vs. *offline*) des del punt de vista de:
- Seguretat  
- Usabilitat  
- Continuïtat del negoci

### 4. Recomanació
Concloeu l'informe escollint **l'eina més adequada per al personal tècnic de l'empresa** i **justifiqueu la vostra elecció**.

---

## 🧰 Fase 2: Guia d'Ús Tècnica (Manual Operatiu)

Utilitzant l'eina seleccionada a la Fase 1 (*Bitwarden, KeePassX, o similar*), heu de crear una **Guia d'Ús per a l'Equip Tècnic**.  
Aquesta guia ha de ser clara i ha d’incloure **captures de pantalla i instruccions pas a pas**.

### La guia ha de cobrir els següents punts obligatoris:

#### 1. Instal·lació i Configuració Inicial
- Descàrrega i instal·lació
- Creació de la **base de dades principal** o **compte mestre**

#### 2. Generació de Contrasenyes Segures
- Com utilitzar el **generador de contrasenyes** de l'eina  
- Configuració de paràmetres: longitud, caràcters especials, etc.

#### 3. Exemples d'Ús i Emplenament Automàtic
- Com desar una credencial d’un **compte de correu electrònic**
- Com desar una credencial d’una **aplicació o servei web**
- Com fer servir **l’extensió del navegador** per emplenar automàticament les dades

#### 4. Gestió de Còpies de Seguretat (Backup)
- Explicació de com **fer una còpia de seguretat** de l’arxiu de contrasenyes  
  - Arxiu `.kdbx` en KeePass  
  - Exportació en Bitwarden
- Recomanacions sobre **bones pràctiques d’emmagatzematge segur**:
  - Clau USB xifrada  
  - Emmagatzematge xifrat al núvol

---

## 🗂️ Lliurament

Aquesta és una **tasca individual**.  
Caldrà lliurar els fitxers dins el **repositori del projecte-3** amb la següent estructura:

[Solució](Tasca01/solució.md)
