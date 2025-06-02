3 Interpretador SHELL

# Deletar
- deletar_arquivos_espeficificos: `rm alvo1 alvo2`
- deletar_varios_de_uma_extensao: `rm *.js  // deletar todos com extensao .js`
- deletar_arquivo: rm -rf <file>
- deletar_diretorio: rm <diretorio>
- parametros_para_remover: -i //vai pedir autorização | -f não precisara autorizar mesmo que seja protegido.

# Manuseio_Arquivos
criar_link_simbolico: $`ln -s <origem> <destino>  // ln de link simbolico`
desfazer_link_simbolico: `unlink <arquivo>`
criar_arquivo: `use:: >> arquivo.ext // use 2 setas antes do nome do arquivo que é o Here Document ao invés de touch arquivo.`
copiar_um_arquivo_pro_outro: `mv arquivoOrigem.ext arquivoDestino.ext`

desinstalar_instalado_via_apt : sudo apt autoremove
<PACOTE>  // desinstala as dependências também.

Pesquisas :

- localizar_alvos : link : (https://g.co/gemini/share/7fafc91c02f1)

mostrar_estrutura_sem_ocultos: `ls -l`
mostrar_estrutura_com_ocultos: `ls -la`
mostrar_detalhes_arquivo: `ls -la <url_alvo>`
mostrar_detalhes_tamanho_arquivo: `ls -lah <url_alvo> // o h mostra o tamanho.`
mostrar_o_que_e_o_arquivo: `file <url_alvo>`


# 1. Mostrar diretório atual
pwd

# 2. Criar um arquivo
>> meu_arquivo.txt

# 3. Verificar se o arquivo foi criado
ls

# 4. Renomear o arquivo
mv meu_arquivo.txt meu_arquivo_renomeado.txt

# 5. Verificar o nome do arquivo após renomear
ls

# 6. Copiar o arquivo renomeado para um novo arquivo
cp meu_arquivo_renomeado.txt copia_do_arquivo.txt

# 7. Verificar os arquivos presentes
ls

# 8. Deletar o arquivo original renomeado
rm meu_arquivo_renomeado.txt

Pesquisar:
- ver_todos_arquivos_ocultos: ls -lah

# 9. Verificar os arquivos após deletar
ls

# 10. Mostrar o local de um comando (exemplo: 'cat')
which cat

---
Fazer_Acao_em_Multiplos_Arquivos: insira o asteristico onde seria o nome d eum unico arquivo
	Exemplo: `mv *.ttf ~/fonts // vai mover tudo que tiver extensao .ttf para a pasta fonts`

Rodar_comando_onde_estiver: <comando> ~/local

---

Descompactar_Arquivos
Zip : `unzip <arquivo.ext>`

---

Conceitos: [
  Shell -> Interface entre o usuário e os recursos do Kernel. Ela pode ser por meio gráfica (GUI) ou por linha de comando (CLI).

Shell Script -> Um arquivo que contém scripts que vão ser executados por um interpretador de linhas de comando

Bash -> É um exemplo de intepretador de comandos.
]

# Comandos_Bash

encontrar_arquivo: locate parteDoNomeArquivoAlvo // vai trazer ocorrências de locais

mostrar_conteudo_arquivo: cat ./endereco/alvo.extencao

valer_novas_configs_sistema: reset


---

Temos os parâmetros : [
que Vamos Enviar, nas funções o indicamos com $
que já são prontos Definidos pelo comando que informamos após o comando com -nomeParamQueQueroUsar  ou --nomeParamQueQueroUsar
]

