# zprofile_catalina_alias
Atalhos pré-definidos para aumentar sua produtividade dentro do terminal do macOS Catalina

==== Cópie e cole dentro do seu arquivo .zprofile da raíz da sua home, ~/ ====
# PATH para ambiente de desenvolvimento
export PATH="$PATH:/Users/$USER/development/flutter/bin:/Users/$USER/Library/Android/sdk"

# Atalhos para terminal
alias res="reset" # Limpa a tela do terminal por inteira, assim podem ficar sem tantos códigos a mostra
alias sos="source ~/.zprofile" # Reinicia o arquivo .zprofile para validar novas alterações feitas no mesmo
alias cls="clear" # Limpa o terminal adicionando espaços acima

# Atalhos para utilização do brew, gerenciador de pacotes
alias insbrew="/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"" # Instalando o brew antes de mais nada
alias bins="brew cask install" # Utilizado para instalar um programa pelo brew
alias brem="brew cask uninstall" # Utilizado para desinstalar um programa instalado pelo brew
# Atalhos de instalação do programas disponíveis no repositório do brew
alias vcode="brew cask install virtual-studio-code" # Instalando o VS Code
alias transmission-cli="brew cask install transmission-cli" # Instalando o Transmission
alias firefox="brew cask install firefox" # Instalando o Firefox

# Atalhos para Flutter, aumento de produtividade
alias fld="flutter doctor" # Verifica status de instalação do flutter
alias flv="flutter doctor -v" # Verifica pendências de libs para utilização do flutter com mais detalhes
alias flr="flutter run" # Comando para rodar seu aplicativo em desenvolvimento, necessário estar dentro da pasta do App
alias flc="flutter emulators --create" # [--name nome_do_emulador]

# Atalhos para Dart, instalação do interpretador
alias bdl="brew tap dart-lang/dart" # Adicionado o repositório de terceiros do interpretador ao brew
alias bdart="brew install dart" # Instala o interpretador
