Node.js

Node.js é uma plataforma construída sobre o JavaScript runtime do Chrome
 para se construir facilmente aplicativos de rede rápidos e escaláveis. O
 Node.js usa um modelo de entrada/saída (I/O) orientado por eventos e não
 bloqueador que o torna leve e eficiente, perfeito para aplicativos de uso
 intensivo de dados em tempo real que são executados entre dispositivos
 distribuídos.
 
<https://nodejs.org/>

Instalar no Linux

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash

```
 export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
 [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm
 
 ``` 
 
 command -v nvm
 
Instalando o NODEJS

 nvm install node # "node" is an alias for the latest version
 
 nvm run node --version
 
 nvm install iojs
