3 Interpretador SHELL

# Deletar
- deletar_arquivos_espeficificos: `rm alvo1 alvo2`
- deletar_varios_de_uma_extensao: `rm *.js  // deletar todos com extensao .js`
- deletar_arquivo: rm -rf <file>
- deletar_diretorio: rm <diretorio>
- parametros_para_remover: -i //vai pedir autorização | -f não precisara autorizar mesmo que seja protegido.

# Manuseio_Arquivos
criar_arquivo: `use:: >> arquivo.ext // use 2 setas antes do nome do arquivo que é o Here Document ao invés de touch arquivo.`
copiar_um_arquivo_pro_outro: `mv arquivoOrigem.ext arquivoDestino.ext`

desinstalar_instalado_via_apt : sudo apt autoremove
<PACOTE>  // desinstala as dependências também.


 * Mostrar diretório atual:
   pw

   * pwd (print working directory) exibe o caminho completo do diretório em que você está atualmente.
 * Criar arquivo:
   touch nome_do_arquivo.txt

   * >> ou touch cria um arquivo vazio com o nome especificado. Se o arquivo já existir, ele atualiza o timestamp de acesso e modificação do arquivo.
   * Você também pode criar um arquivo e adicionar conteúdo a ele imediatamente usando o redirecionamento:
     echo "Conteúdo do meu arquivo" > meu_novo_arquivo.txt

 * Renomear arquivo:
   mv nome_antigo.txt novo_nome.txt

   * mv (move) é usado para mover ou renomear arquivos e diretórios. Quando o destino está no mesmo diretório, ele efetivamente renomeia o arquivo.
 * Deletar arquivo:
   rm nome_do_arquivo.txt

   * rm (remove) é usado para deletar arquivos. Tenha cuidado ao usar rm, pois os arquivos excluídos geralmente não podem ser recuperados facilmente.
 * Mostrar local do arquivo em uso (do próprio comando que você está executando no shell):
   which nome_do_comando

   * which localiza o caminho de um comando no sistema de arquivos. Por exemplo, para saber onde o comando ls está localizado:
     which ls

   * Se você quiser saber o caminho do script shell que você mesmo está executando (dentro do próprio script), você pode usar variáveis como $0:
     echo "O caminho deste script é: $0"

 * Copiar arquivo, movendo para um novo arquivo (criando uma cópia e mantendo o original no lugar):
   cp arquivo_original.txt copia_do_arquivo.txt

   * cp (copy) faz uma cópia do arquivo de origem para o arquivo de destino. O arquivo original permanece inalterado.
Exemplo prático de uso sequencial:
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

