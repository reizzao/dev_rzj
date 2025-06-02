# Terminal Multiplex TMUX

Comandos:
- desconetar de instancia de terminal: original: ctrl+b e
ver_meus_terminais: tmux ls
voltar_ao_terminal_antigo: tmux a
escolher_janelas: ctr+b 0, ctr+b 1, etc... 
fechar_sessao_janela: exit

Configuracoes:
Criar_arquivos_de_configuracao:  .tmux.conf // crie este arquivo na HOME principal do user
 -- configuracoes do CaioDelgado : (https://github.com/caiodelgadonew/dotfiles/blob/main/tmux/.tmux.conf)
    recarregar_mudancas_das_configuracoes: $`tmux source .tmux.conf` e matar o terminal ctr+C
