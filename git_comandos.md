# gitcola
comando que utilizo no git

git config --global user.name "léo"                       		 -- configurando meu nome no git
git config --global user.email "lpoliveira132@gmail.com"  		 -- configurando meu email no git
git config --list							 -- vendo lista(usuario email entre outras)
mkdir git-leo								 -- criando pasta pro projeto
cd git-leo						  		 -- entrando na pasta
git init								 -- iniciando repositorio
ls -la 							 	         -- ve pasta do git
cd .git/ 								 -- entra na pasta onde tem config. branch e tals
cd ..  							                 -- volta(sai da pasta)
vim algo --(criando arquivo)						 -- criando arquivo
i para escrever esc para sair
dois pontos pra por wq que pe salvar e sair dai dou enter
depois do arquivo criado o git status vai mostrar em vermelho untracked
dai fazemos um git add nome do arquivo para ficar verde
git commit -m "comentario"                                               -- fazendo commit do git
git log para ver logs
git log --decorate 							--para ver detalhado
git log --author = "leo"						--para ver author do log
git shortlog
git diff                                                                --eu vejo oq fiz antes de comitar 
git checkout nome do arquivo volta a ultima alteração antes de por no stage
git reset HEAD nome do arquivo caso ja esteja no stage
caso eu ja tenha comitado eu tenho os seguintes comandos
git reset --soft volta o commit para o stage escolha sempre um anterior commit
git reset --mixed volta para antes do stage escolha sempre um anterior commit
git reset --hard deleta todo commit mesmo escolha sempre um anterior

criando chave
ssh-keygen -t rsa -b 4096 -C "lpoliveira132@gmail.com"
cd ~/.ssh/
$ ls
id_rsa  id_rsa.pub
$ cat id_rsa.pub
ssh-rsa 
AAAAB3NzaC1yc2EAAAADAQABAAACAQCU9g3cdgyt
I7YDq25TA2REobYzDhz/MFLHOr9mVoyYRYFPS6s7
VGLY9Qkm8U7ftSEqojl/9lTknGnA1/FD79NvoPKk
D7zrLFzVUTKjvMWMeWAzecfWQeoN4i20qvx2kmi6
IX1kksk8CNvmQbbPO8usTQVvin2T4wuGdbdr3i25
Ygxbb2cPlpEFoyyaUBwbxAUC6IolSEtqZ740gbwL
TReO+EXeoNqkYyxTVsg9DifmvUNMallh2AWIVa9j
4AmOUI5xXhzKkeK599sDPqwQcLBlhO60h6tZW10E
ikNMHI1O/pLx/Mr1yRExBTPpUcErJajYl0mumqM2
kpmPrzf/7EB/XAhIDHjYZt4+FdkYHCJtCo2Cl5W/q
WfWW6IVVbY81PVuWygAeknJdOCvFiqzcp0gA7ZeIG
HHZYdj3S6pOMd9nDM0DwY19iTH/t58e0+RCOC4hUh
lz9JRalByI0Nmzi3CRqCvz/HZBvC7v4djuIrVI8q/
kxPRkimlt8lPE8i5/XOwC4IkFjcpX7VoN3lzZ7IK
L5y/Yo7Dq3041HNeowkP97QRb5NWk5v7WYCMMgKT0
wL7CUMsu48imVDiJIgE1RVReUNj5bvLynVvxIO53j
P8hgVVjeBC5gbBpa08NrwzVJqoH0cdLvAPIIdWyVc
9p2w2iFgwkuqEb6X+bP1Mmwe37w== lpoliveira132@gmail.com

git push origin master para mandar suas atualizações para a web(github)
git checkout -b nome --cria um branch
git branch - mostra o branch que vc esta
git merge nome - chama o branch para se juntar ao master - esse entra na posição em que foi criado mesmo (meio)
git rebase nome - chama o branch para se juntar ao master porem ele vai para o topo
git stash salva uma coissa que vc ainda nao comitou pq quer mexerr ainda
git stash aply volta a mexer nele

git config --global alias.s status -- aqui eu quero que status seja executado usando só a letra S

git tag -a 1.0.0 -m "oq foi feito"

git revert numero do commit -- reverte oq o ultimo commit fez 
