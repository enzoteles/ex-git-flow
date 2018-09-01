# Comandos Git


Ajustou o bug do menu do meu cartões,
Ajustou as branchs no git
Verificou a atividade de ativação do cartão
e corrigiu os bugs do chat e o chat de avaliação (mudando o link)

* Remover errors que ainda não foram para o commits 
- git reset - - hard
 
* Remover erros que já foram adicionados mais não foram comitados
- git reset - - hard HEAD


* comando mostra o gráfico da árvore do git
git log --pretty=format:"%h %s" –graph



- rebase

	  é quando você quer integragar o seu trabalho com alguma branch, mais tem suas restrições por que pode apagar algum commit, e é aconselhado usar mais em branch privada (local), e não em branch pública(remoto)

- stash

	  estratégia usada para quando você quiser fazer um checkout para outra branch sem precisar commitar o que você está fazendo na sua branch atual, ou quando você se esquece de mudar ou criar uma branch por exemplo e usar o stach para passar o que você fez para outra branch, como por exemplo se você fez algo na develop e não quis fazer isso diretamente na mesma, e prefere mudar para outra branch, pode usar tranquilo o stash.

- fetch
	 fetch, o Git reúne qualquer commit da ramificação de destino que não existe na sua ramificação atual e os armazena em seu repositório local . No entanto, ele não os mescla com sua ramificação atual . Isto é particularmente útil se você precisa manter seu repositório atualizado, mas está trabalhando em algo que pode quebrar se você atualizar seus arquivos. Para integrar os commits em seu branch master, você usa merge.

- checkout

	- comando usado para criar ou mudar de branch 

- track

	- Filiais de Rastreamento

Fazer check-out de uma ramificação local de uma ramificação remota cria automaticamente o que é chamado de ramificação de rastreamento. As ramificações de rastreamento são ramificações locais que têm um relacionamento direto com uma ramificação remota. Se você estiver em uma ramificação de rastreamento e digitar git push, o Git saberá automaticamente em qual servidor e ramificação pressionar. Além disso, a execução do git pull em um desses ramos busca todas as referências remotas e, em seguida, é mesclada automaticamente no ramo remoto correspondente.

Quando você clona um repositório, ele geralmente cria automaticamente um branch master que rastreia origem / master. É por isso que git push e git pull trabalham fora da caixa sem outros argumentos. No entanto, você pode configurar outras ramificações de rastreamento, se desejar - aquelas que não rastreiam ramificações na origem e não rastreiam a ramificação principal. O caso simples é o exemplo que você acabou de ver, rodando git checkout -b [branch] [remotename]/[branch]. Se você possui o Git versão 1.6.2 ou posterior, você também pode usar o  --trackatalho:

$ git checkout --track origin/serverfix
Branch serverfix set up to track remote branch refs/remotes/origin/serverfix.
Switched to a new branch "serverfix"
Para configurar uma ramificação local com um nome diferente da ramificação remota, você pode usar facilmente a primeira versão com um nome de ramificação local diferente:

$ git checkout -b sf origin/serverfix
Branch sf set up to track remote branch refs/remotes/origin/serverfix.
Switched to a new branch "sf"
Agora, seu ramo local sfirá automaticamente empurrar e puxar de origin/serverfix.


- ainda tem mais comandos


