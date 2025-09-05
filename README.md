# Desafio criando máquina Virtual na Azure.

Seguindo a conclusāo do modulo. Vimos os beneficios da nuvem.
Onde foram explanados sobre escalibilidade, elasticidade e o SLA.
Bem como:

**Escalibilidade**
Tem como intuito aumentar a configuracao para uma mais abrangente quando necessario, atendendo as necessidades enfrentadas pela demanda.

**Elasticidade**
Ter como intuito o auto ajuste para atender as demandas. Tanto para mais (criando mais servicos do mesmo) ou para menos (reduzingo a quantidade de maquinas visto que nao estao em utilizacao).

**SLA**
Service Level Agreement ou Tempo de acordo do serviço. Onde é o tempo pré estabelecido de intividade do serviço. Onde vemos muito nas clouds o uso de 11 9 para defeninr o possivel tem de baixa.

##Solicitaçāo da criāo de um servidor virtual na Micrisoft Azure.

Como solicitado no desafio segue um breve tutorial de criacāo de uma máquina virtual, via console:

No console Principal vá na opçāo Virutal Machine, depois em create.

Logo siga esses passos:

Na aba BASICS

1 - Selecionae a Subscription e o ResourceGroup onde ficara armazenado a VM que voce esta criando.

2 - Apos isso defina o nome da VM, Region e Availability Options que melhor atenda seu projeto;

3 - Depois defina Availability Zone;

4 - O tipo de Security Type;

5 - A imagem que voce ira utilizar em sua VM;

6 - O VM architeture;

7 - Familia da VM que deseja utilizar;

8 - O modelo de autentiçāo;

9 - O nome da Key pair name, caso seja um servidor linux. Caso windows nome do usuario e senha.

10 - COnfigure o Inbound Port Rules.

Na aba Disks

1 - Em OS Disk, ocnfigure o tamnho do disco e o type;

2 - Key management caso deseja inserir criptografia e o tipo de chave;

3 - E caso tenha a necessidade a configuracao de disco adcional.

Na aba Networking

1 - Selecione a Virtual Network;

2 - A subnet desejada;

3 - Se a mesma te Public IP ou nāo;

4 - Selecione o tipo de NIC e Public Inbound Ports;

5 - Selecione o Load balancing necessario de acordo com seu projeto.

Na aba Management

1 - Configure intens administrativos cmo Indetidade, liberacao de acesso por Microsot Entra ID, Auto-shutdown, backup e Guest OS updates;

Na aba MOnitoring

1 - Configure habilitacao de alertas, Diagnostics e Helth check;

Na aba advanced

1 - Configure o Custom data ou User data caso necessario, dependendo da aplciacao;

2 - Configure o Host, caso necessite inserir dentro de um Host group, ou tenha um Capacity ou caso necessitar um Proximity placement group.

Na aba TAGS

1 - Insera as tags de acordo com sua necessidade.

Na aba REVIEW & CREATE

1 - Valide o termo de criaçāo da VM e reveja as opções selecionadas.

E por final crie a VM.


Após criado você pode realizar o acesso via ssh.


Nāo esqueça de limpar os serviços quando nāo forem de uso produtivo. Para evitar custos.

Obrigado.
