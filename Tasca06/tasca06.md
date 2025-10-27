# T06: Fonaments del servei DNS

## 📝 Breu descripció
Com membres cada cop més integrats de l'equip tècnic de la consultora EverPia, teniu davant un nou repte. El vostre client, una empresa de màrqueting digital (DigiCore), experimenta de tant en tant errors de connectivitat a certes aplicacions. El seu equip tècnic creu que la causa principal podria ser una resolució de noms (DNS) incorrecta o lenta.

Se us ha encarregat realitzar una auditoria teòrica i pràctica del servei DNS per tal de formar el personal del client i oferir eines de diagnosi ràpides.

---

## 📚 Fase teòrica: Sessió formativa
Caldrà elaborar un material formatiu pel personal del client. Els conceptes que heu d’explicar són:

- **🌳 Jerarquia i Estructura:** Explicació de l'estructura en arbre del DNS (Root > TLDs > Segon Nivell).  
- **🔄 Procés de Resolució:** Consulta iterativa i recursiva. Què és un servidor d'arrel (Root Server) i un servidor autoritatiu.  
- **📂 Tipus de zones:** Directa i inversa. Zona primària i zona secundària.  
- **📜 Tipus de Registres Clau (Records):** A, CNAME, MX, NS i SVR.  

### Conceptes Essencials
- **✅ Resposta Autoritativa:** Què significa i com identificar-la.  
- **⏱️ Time To Live (TTL):** Funció i impacte en propagació i rendiment.  
- **🛠️ Start of Authority (SOA):** Informació essencial i crítica.  
- **🔁 Reenviadors:** Condicionals i incondicionals.  
- **🏠 Resolució local:** Mecanismes de resolució sense servidor entre equips clients, inclòs el protocol mDNS.  

**🎬 Activitat:** Crear un vídeo formatiu de 10-15 minuts explicant aquests conceptes.

---

## 💻 Fase Pràctica: Diagnosi de Noms (Auditoria amb CLI)
Heu de demostrar l'ús de les principals utilitats de diagnosi DNS en Linux/macOS i Windows.

**Configuració:** Equip Zorin amb dues interfícies:  
- NAT  
- Adaptador pont amb IP correcta segons indicacions.



