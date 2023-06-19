Expérience de code avec Electron pour apprendre comment transférer MFSS 
dans un projet Electron ...
creation application Electron

-creation d'un package.json
(entry point doit être main.js & author et description peuvent prendre n’importe quelle valeur, mais sont nécessaires pour le packaging de l'application.)

npm init 

-installation Electron 

npm install --save-dev electron

Ajouter dans package.json
{
  "scripts": {
    "start": "electron ."
  }
}

-Lancer l'application Electron

npm start


Le point d’entrée de toute application Electron est son script main.

- Installer Forge pour créer l'exe et l'installateur
Ajoutez Electron Forge en tant que dépendance de développement et utilisez la commande import pour initialiser le squelette de base de Forge.

npm install --save-dev @electron-forge/cli

npx electron-forge import



✔ Checking your system
✔ Initializing Git Repository
✔ Writing modified package.json file
✔ Installing dependencies
✔ Writing modified package.json file
✔ Fixing .gitignore

We have ATTEMPTED to convert your app to be in a format that electron-forge understands.

Thanks for using "electron-forge"!!!


- Lancer la création d'une distribution 

npm run make

Electron Forge crée un dossier out où se trouvera vos fichiers de distribution