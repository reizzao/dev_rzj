# Instalacoes Pacotes ALL

# IMPORTANTE
Pos_Formatacao_de+_P :insira essa chama no `~/.bashrc` para funcionar o My sShell Personal
`
# -------------------------------------------------
# MINHAS CUSTOMIZAÇÕES

# CHAMA MY PERSONAL SHELL
if [ -f $HOME/dotdev/myshell/._init ]; then
    . $HOME/dotdev/myshell/._init
fi


# -------------------------------------------------
`


# FLOW <Produtividade Dev>

$`sudo apt install tmux`
// terminal multipliplas janelas : tmx
Plugins:
valer_instalar_configurados: ctr+A I // obs: o control pe o profixo configurado e o I éo o I maiusculo Capital.

Plugin Tmux tpm - baixa ter ele clonado na maquina
Repositorio: (https://github.com/tmux-plugins/tpm)
Clonar_para_maquina: $`git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm`

Fontes:
Como_instalar: faça download na web, descompacta e cola na raiz em : ~/.fonts
obs: geralmente essa pasta nao existe por padrao - entao cria e cole as novas fontes nela
com o comando: $`mkdir ~/.fonts`
Carregar_fontes_adicionadas : $`fc-cache -fv` // apos ler as fontes só configurar o terminal para usar a desejada.

Nerdfonts : (https://www.nerdfonts.com/) , obs: entre na pagina de donwloads
    Top_Fontes: [
        - Nome: Source Code Pro , Demos: (https://www.programmingfonts.org/#source-code-pro)
    ]

Terminal_MultJanelas:
Tmux: recarregar_mudancas_de_configuracao: $`tmux source ~/.tmux.conf`
Customizador_design: catppuccin, acesso: (https://github.com/catppuccin/tmux)

Terminal_Alacritty : instalacao: $`:sudo apt install alacritty -y`
configuracao_toml : (https://github.com/caiodelgadonew/dotfiles/tree/main/alacritty/.config)
obs:baixe a configuracao.toml e add no ~/.config/alacritty/ (obs: senao tiver o diretorio alacritty crie-o e cole o arquivo de config.)
Abrir_Terminal: add ele nos favoritos da bar de apps do seu pc e abra no click.

Customizar_Terminal
 // Mostrar desenho bonito de arvore de diretorios
 $`sudo apt install tree -y`
 // usar: no diretorio desejado $`tree -a -I .git`


# Editores
Vim: $`sudo apt install vim` // VIM PURO - não é obrigatorio instalar.

Neovim : `
  // dependencias
  sudo apt install git curl gcc g++ lua-filesystem clang clangd`
  // versao stable
  sudo add-apt-repository ppa:neovim-ppa/stable
  // att
  sudo apt update
  // install
  sudo apt install neovim -y
  // versao
  nvim --version

  // Libs-Plugins-gerenciadores
  // LazyVim :
  [Instalacao no Site_Oficial:] (https://www.lazyvim.org/), obs: q para sair
  `

Lib_Para_link_Simbolico
    Nome: stow, beneficio: ele ja linka um arquivo com toda pasta ao inves de entrar e fazer link de arquivo por arquivo dentro da pasta.
    instalar: `sudo apt install stow -y`
    confere_instalacao: `stow --version`

    usar: entra na pasta alvo , digite: `stow <alvo>
    // este alvo será criado um link simbolico na HOME ex: stow tmux - linkar o tmux da HOME com o desta pasta alvo que eu dei o comando.`
    conferir: `ls -la ~/`

    remover_link_by_stow: `stow -D <alvo>`

    uso_frequente: `
    // dentro da pasta dotfiles : dar os comandos para linkar com os do repo clonado :: obs: na primeira vez os alvos de origem nao precisam existir.

    comandos :
    stow alacritty
    stow nvim
    stow tmux
    `

gerenciador_pacotes
    Nome: apt,
    acessar_infos_site_pacotes_instalados : `apt show <nomepacote>`

MyFlow_Dotfiles :
-
- no dotfiles imitar a estrutura que seria na maquina
- usar stow para link simbolico para enganar a maquina, ela procurará um alvo e este alvo sera o que linkei na /dotfiles que por sua vez está guardada no github.
