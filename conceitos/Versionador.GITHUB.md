Significados:
github: é um versionador que controla a linha do tempo entre passado, futuro e presente de uma aplicação, que envia arquivos modificados preparados para nova versão da máquina local para o servidor web/remoto na nuvem github.com.

remoto: na nuvem na web no servidor.

parametro_para_LingaDeComando: demarca-se com 2 traços na frente e o nomeDaOpcao, são opções de linha de comando já configuradas que vc só usa. ex: --Hard,  quer dizer qye esse comando tem opções diferentes pra decidir como vc vai agir e vc escolheu essa --hard , ou seja ele vai dar reset mas dá forma Hard com certeza remoto outras opções tbm.

---

Ciclo_De_Versionamento :

modificados: vai pra stage área de controle de versao é tipo um buffer em memoria,
  visualisa_se_houve_mudancas: git status

adicionar_ao_controleDeVersao: git add . // adiciona todos ou `git add "nomearquivo.ext"` >> para adiciona somente esse 1 arquivo .

dar/intendificacao_comComentario_a_VersaoEnviada : git commit- m "mensagem O que foi modificado na versao?"

puxar_a versao_pro_remoto : git push

PraQualRepo: o git push funciona se ele sabe pea qual repo cai enviar, pra ele saber ou vc clona o repo ou informa qual é o repo com o comando ::
git remoto add origin <url do repo>

Publicar_Que_tem_Branch_Nova: git push --set-upstream origin <NomeBranch> // só faz uma vez pra master oadrao e quando mudar para outra branch nova pra avisar que existe uma nova a ser publicsda conhecida,

---

Manipular_Historico_de_Versoes

 informar_historico: git reflog // vai mostrar com o id e menssgem a versão atual e também a versão anterior -- essas informações podemos usar em outros comandos ex: reset.

voltar_a_versao_por_id : git reset --Hard <Id_da_Versao>

// todo: ver outros parâmetros disponiveis

---

branches :
Significado: são galhos aramazenadores onde em cada posso guardar uma coleção de versoes, obs: ao criar uma branca o git cria 2 da mesma 1 local e outra remoto

conceito: pra salvar da local pra remota é feito um merge.

Uso_Servical: vc sempre terá uma branch que será a Master e outras serviçais, essas serviçais depois que fazerem um trabalho sempre enviará esse trabalho feito via solicitação de aprovação para fazer parte da master.

Resumo_Conceito: a Master é a instável (só entra as novas funcionalidades aprovadas nela) e as outras serviçais são pra criar e testar as funcionalidades novas para serem aprovadas.

Convensao: nome de beach Nova ainda nao testada = stage ou sua funcionalidade que vai entregar.

ver_todas_branches: git branch
// após mais de uma adicionada a que estiver de cor diferente e com asteristivo * é a que estamos nela usando no momento.

mudar_outra_outra_branch : git checkout <NomeBranch>

VersionamentosNaBranch: é o mesmo feito na master  $Ciclo_De_Versionamento

Mergiar :
  Conceito: Mergiar é trazer atualizações versionadas de uma brach para outra.

Ciclo_para_Mergiar_Direto_Sem_Burocracia : [
- 1° entrar na branch que vai receber as atualizações

- 2° rodar : git pull // obrigatório ser antes do merge para ele trazer o mais atualizado do remoto.

- 3° rodar : `git merge < NomeBranch que puxarei as novidades >`

]


Ciclo_para_Mergiar_Com_Burocracia _Aprovacao :
// mediante aprovação então é Pull Request



]







