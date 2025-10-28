# 💽 T03: Gestió flexible de discos  
### 🔄 LVM (Linux) i Espais d’emmagatzematge (Windows)

---

## 📝 Breu descripció

Un cop superada la fase de formació, l’equip tècnic d’**EverPia** està preparat per afrontar un **nou repte real de client**.  

El **bufet d’advocats “Garriga i Associats”**, un dels més prestigiosos de la ciutat, gestiona una gran quantitat d’**informació legal sensible**.  
Per això, la **integritat**, la **disponibilitat** (alta redundància) i la **facilitat de gestió** del seu emmagatzematge són **crítiques**. ⚖️📂  

La direcció del bufet ha expressat la necessitat urgent de **renovar els sistemes de servidors** per garantir:
- Protecció davant fallades de disc 💾  
- Possibilitat d’**ampliar l’espai sense interrupcions** ⚙️  

> 🎯 Com a tècnics d’EverPia, el vostre encàrrec és **dissenyar i documentar dues solucions d’emmagatzematge**, una per **Linux** i una altra per **Windows**, que compleixin amb els principis d’**alta disponibilitat, redundància i escalabilitat**.

---

## 🧩 Objectiu general

Dissenyar i documentar **dues solucions d’emmagatzematge** (una per a cada entorn):

| Sistema | Tecnologia | Objectiu |
|:--------|:------------|:----------|
| 🐧 **Linux (Zorin OS)** | LVM (Logical Volume Manager) | Alta disponibilitat i escalabilitat dinàmica |
| 🪟 **Windows 11** | Storage Spaces (Espais d’emmagatzematge) | Mirroring, paritat i gestió visual simplificada |

📘 Aquesta prova de concepte es realitzarà en **màquines virtuals** de sistemes operatius clients.

---

## ⚙️ 1️⃣ Part Linux: LVM amb Zorin OS

Demostració de la utilitat del **Logical Volume Manager (LVM)** per a la gestió flexible i segura de discos.

### 🧾 Requisits i passos

#### 🔹 Configuració inicial
- Crear un **Grup de Volums (VG)** i un **Volum Lògic (LV)**  
- Utilitzar **dos discs durs simulats** de **10 GB** cadascun  
- Formatar i muntar el volum automàticament mitjançant `/etc/fstab`

#### 🔹 Alta disponibilitat
- Implementar una configuració **en mirall** (`lvm_mirror`)  
- Garantir la **protecció davant la fallada d’un disc**

#### 🔹 Instantànies (Snapshots)
1. Afegir **dos discs de 10 GB** addicionals al grup de volums  
2. Crear un volum (`lvm_dades`) amb el primer disc  
3. Formatar, muntar i afegir fitxers (p. ex. imatges)  
4. Crear un **snapshot (`lv_snapshot`)** amb el segon disc  
5. Documentar com **restaurar** el snapshot en cas de corrupció del volum original

#### 🔹 Escalabilitat
- Fer servir l’espai lliure dins el grup de volums per **ampliar el volum `lv_dades`**

---

## ⚙️ 2️⃣ Part Windows: Espais d’Emmagatzematge (Storage Spaces)

Demostració de les capacitats dels **Storage Spaces** de **Windows 11** per a la gestió segura i flexible dels discos.

### 🧾 Requisits i passos

#### 🔹 Configuració inicial
- Crear un **Storage Pool** amb **tres discos de 10 GB** simulats

#### 🔹 Estudi de configuracions
| Tipus de resiliència | Descripció | Avantatges |
|:----------------------|:------------|:-------------|
| 🔁 **Mirroring** | Usa 2 discos per duplicar dades | Alta disponibilitat |
| 🔂 **Triple Mirroring** | Usa 3 discos per triple còpia | Més seguretat davant múltiples fallades |
| ⚙️ **Parity** | Guarda informació de paritat | Més eficient en espai, menor rendiment en escriptura |

➡️ Afegir els discos necessaris i **documentar la creació** de cada configuració.  
➡️ Comparar **eficiència, redundància i espai disponible**.

#### 🔹 Demostració de la gestió
- Mostrar com visualitzar l’estat dels **discos** i del **pool** des de la **consola de gestió de Windows**
- Simular tasques de **manteniment i monitoratge**

---

## 👥 Organització del treball

El treball es realitzarà **en grup**:

| Equip | Tasca principal | Sistema |
|:------|:----------------|:--------|
| 🧑‍💻 Equip 1 | Gestió flexible amb **LVM** | Linux |
| 🧑‍💻 Equip 2 | Gestió flexible amb **Storage Spaces** | Windows |

### 🔧 Metodologia

1. **Divisió d’equips** (Linux / Windows)  
2. **Investigació individual**:  
   - Cercar comandes, opcions i documentació oficial  
3. **Execució per parelles**:  
   - Cada parella realitza la seva **part de demostració pràctica**  
4. **Revisió i integració de la documentació**  
5. **Publicació conjunta** al repositori GitHub

---

## 📂 Lliurament

La documentació dels dos casos s’ha de realitzar en **format Markdown** (`.md`), incloent:

- 📸 Imatges o captures de pantalla  
- 💬 Explicacions pas a pas  
- 📁 Estructura dins la carpeta:

