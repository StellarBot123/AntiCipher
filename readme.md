# 🛡️ StellarShield – Anti Backdoor FiveM

> **StellarShield est un outil de protection en temps réel contre les backdoors FiveM.**  
> Il surveille ton artifact et neutralise automatiquement toute tentative d’exécution malveillante.  
> Inspiré du fonctionnement de *cipher-panel.com*, mais **open-source et gratuit**. 🚀

---

## 📖 Sommaire
1. ⚙️ Pré-requis  
2. 🛠️ Installation  
3. 🔐 Utilisation  
4. 🧠 Bonnes pratiques  
5. ⚠️ Compatibilité  
6. ✨ Conclusion  

---

## ⚙️ Pré-requis
- Un **artifact clean** téléchargé depuis le site officiel de Cfx.re  
  👉 [Télécharger ici](https://runtime.fivem.net/artifacts/fivem/build_proot_linux/master/)  
- Un accès **root** ou utilisateur avec `sudo`  
- Un serveur **FiveM éteint** (⚠️ ne surtout pas le démarrer avant la protection)

---

## 🛠️ Installation

```bash
# Cloner StellarShield
git clone https://github.com/ton-repo/StellarShield.git
cd StellarShield

# Compiler (Go requis)
go build -o StellarShield main.go
🔐 Utilisation
1. Démarrer StellarShield
⚠️ Toujours lancer StellarShield avant ton serveur FiveM :

bash
Copier
Modifier
./StellarShield
Tu verras :

👀 Les dossiers surveillés

📦 Les fichiers suspects interceptés

📡 Les notifications envoyées sur ton webhook Discord

✨ Confirmation que la protection est active

2. Démarrer ton serveur FiveM
Une fois StellarShield lancé, tu peux démarrer ton serveur normalement :

bash
Copier
Modifier
cd /home/FiveM/server/alpine/
bash run.sh +exec server.cfg
🧠 Bonnes pratiques
🔄 Met à jour régulièrement ton artifact avec une version clean.

🛡️ Toujours lancer StellarShield avant ton serveur.

👀 Surveille ton webhook Discord pour être alerté en cas de détection.

📥 Sauvegarde tes configs (server.cfg, ressources clean).

⚠️ Compatibilité
✅ Fonctionne parfaitement sur VPS Linux (Ubuntu recommandé)

⏳ Pas encore compatible avec :

Pterodactyl Panel

RDP Windows

👉 Merci de patienter, ces plateformes seront prises en charge plus tard.
Actuellement je ne suis pas disponible pour développer leur support.

✨ Conclusion
Avec StellarShield, ton serveur est enfin :
✅ Protégé contre les backdoors
✅ Sécurisé même si des fichiers infectés sont déjà présents
✅ Facile à utiliser, sans config compliquée

💡 Retiens bien : sans StellarShield lancé en amont, les anciennes backdoors peuvent se réactiver.

👨‍💻 Développé avec ❤️ pour la communauté FiveM
