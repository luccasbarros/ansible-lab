# Respostas

## Defina o que é:
### Tasks:
R: Tasks são unidades de ação no ansible. São scripts que são executadas do modo como você molda eles. Você tem a possibilidade de executar simultâneas tasks em uma só vez..

### Plays:
Uma play é um mapeamento entre um conjuntos de hosts especificado por um gerenciador de hosts (normalmente grupos), onde nesses hosts
as tarefas são executadas para definir a função que o sistema vai desempenhar.

### Playbooks
Playbook é a principal feature no Ansible. Ele desempenha o papel de executar as tasks. Nele contem passo-a-passo do que o usuário gostaria
que a máquina executasse.

### Roles
Permitem que você carregue automaticamente arquivos relacionados como as vars, tasks, handlers e os artefatos, baseado em uma estrutura.
Uma vez que você agrupa seu conteúdo em roles, você facilmente consegue reutilizar e compartilhar com outros usuários.

### Ansible Galaxy
O Ansible Galaxy é um repositório que contém roles compartilhadas. É nele, que por exemplo, conseguimos dar um init em uma estrutura de ansible.
No Ansible Galaxy que conseguimos compartilhar as roles, algumas linhas de comandos/scripts para gerenciar as roles.

## Como usar arquivos existentes do Vault no Ansible Tower?
Você pode utilizar var_files no playbook, que então descriptografa o arquivo do vault correspondente quando um manual é executado.
Basicamente você armazena essas variáveis em pastas como group_vars ou hosts_vars, então a sincronização é feita sem mesmo usar credencial,
e navegando até o grupo ou host por exemplo, você nota a variável criptografada.

## Como você faria para implementar o AWX?
Primeiro configuraria a habilitação do repositório epel
Configuração do Docker e ativação
Realizaria o clone do repositório do AWS
Editaria o inventory
Executaria o script de install com o ansible-playbook, e então, logava no AWX com as credenciais padrão


## Pra que serve o AWX?
É um projeto de código aberto da Ansible Tower. Nos permite controlar o uso dos projetos em Ansible Tower no ambiente, fornecendo uma interface de usuário baseado em web
e um mecanismo de tarefas baseado no Ansible. É uma ferramenta de automatização de tarefas, nos permitindo fazer o deploy de aplicações, provisionar servidores, automatizar tarefas, e outras funções.
