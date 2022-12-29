## An exodus theme I made so exodus would look more "cleaner" (can be a proof of concept of modifying exodus)
### Preview:
  - [Before](https://user-images.githubusercontent.com/111450473/199370479-67da4ea8-9f98-4998-ada6-e4b0264c0e06.png)
  - [After](https://user-images.githubusercontent.com/111450473/199372219-38725352-3bd8-45e4-877d-867b28256d12.png)
  
### 1. Needed tools
  - [Node.js](https://nodejs.org/en/download/) (make sure npm is added to path)
### 2. Setup
  - Close exodus
  - Open cmd
  - Install the asar package (used for packing and unpacking the app.asar file)
  ```cmd
  npm i asar
  ```
  - Change directory to %localappdata%\exodus\app-* version you're on *\resources\
  - Example: `%localappdata%\exodus\app-22.10.22\resources\`
### 3. Installing the theme
  - Unpack the app.asar archive with the command below
  ```cmd
  npm exec asar e app.asar ExodusFiles
  ```
  - Open file explorer then go to: `%localappdata%\exodus\app-* version you're on *\resources\ExodusFiles\src\static\css`
  - Drag and drop the css files into the folder
  - Repack the app.asar archive with the command below
  ```cmd
  npm exec asar p ExodusFiles app.asar
  ```
### 4. Launch exodus
  - aaaaaaaaaaaaaaa i hope it work for you
  

