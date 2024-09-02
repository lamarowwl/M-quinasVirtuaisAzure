# Guia para Criar uma Máquina Virtual no Azure

Este guia passo a passo irá ajudá-lo a criar uma máquina virtual (VM) no Azure usando o portal Azure.

## Pré-requisitos

Antes de começar, você precisará:

1. Uma conta do Azure. Se você não tiver uma, pode criar uma [aqui](https://azure.microsoft.com/free/).
2. Acesso ao [Portal do Azure](https://portal.azure.com/).

## Passo 1: Acesse o Portal do Azure

1. Vá para o [Portal do Azure](https://portal.azure.com/) e faça login com suas credenciais.

## Passo 2: Crie um Novo Recurso

1. No painel de navegação à esquerda, clique em **Criar um recurso**.
2. Na barra de pesquisa, digite **Máquina Virtual** e selecione **Máquina Virtual** nos resultados da pesquisa.
3. Clique no botão **Criar** para iniciar o assistente de criação de VM.

## Passo 3: Configurações Básicas

1. **Assinatura**: Selecione a assinatura do Azure que você deseja usar.
2. **Grupo de Recursos**: Selecione um grupo de recursos existente ou clique em **Criar novo** para criar um grupo novo.
3. **Nome da Máquina Virtual**: Insira um nome para a VM.
4. **Região**: Escolha a região onde você deseja criar a VM (ex: "Leste dos EUA").
5. **Opções de Disponibilidade**: Escolha o tipo de redundância que você deseja para sua VM, como **Nenhuma**, **Conjunto de Disponibilidade** ou **Zonas de Disponibilidade**.
6. **Imagem**: Escolha o sistema operacional para a VM (por exemplo, **Windows Server 2019 Datacenter** ou **Ubuntu Server 20.04 LTS**).
7. **Tamanho**: Clique em **Ver todos os tamanhos** para escolher o tamanho da VM de acordo com as necessidades de CPU e memória.

## Passo 4: Configurações de Administração

1. **Autenticação de Conta de Administrador**: Escolha entre **Senha** ou **Chave SSH** para autenticação.
   - Se escolher **Senha**, insira um **Nome de Usuário** e **Senha**.
   - Se escolher **Chave SSH**, insira um **Nome de Usuário** e cole sua chave pública SSH.
2. **Portas de Entrada**: Selecione **Permitir portas de entrada selecionadas** e escolha **RDP (3389)** para Windows ou **SSH (22)** para Linux.

## Passo 5: Configurações de Disco

1. **Tipo de Disco do Sistema Operacional**: Escolha entre **SSD Padrão**, **SSD Premium** ou **HDD Padrão**.
2. **Discos de Dados**: Adicione discos de dados adicionais conforme necessário clicando em **Criar e anexar um novo disco**.

## Passo 6: Configurações de Rede

1. **Rede Virtual**: Selecione uma rede virtual existente ou crie uma nova.
2. **Sub-rede**: Escolha uma sub-rede existente ou crie uma nova.
3. **Endereço IP Público**: Escolha **Habilitado** para atribuir um IP público à VM.
4. **Grupo de Segurança de Rede (NSG)**: Selecione **Criar novo** para configurar regras de firewall para a VM.

## Passo 7: Revisar e Criar

1. Clique em **Próximo: Revisar + criar** para revisar suas configurações.
2. Verifique se todas as informações estão corretas.
3. Clique em **Criar** para iniciar a implantação da VM.

## Passo 8: Acessando sua Máquina Virtual

1. Após a criação, vá para **Máquinas Virtuais** no painel de navegação à esquerda.
2. Selecione sua nova VM na lista.
3. Clique em **Conectar** no topo da página.
   - Para VMs Windows, escolha **RDP** e baixe o arquivo RDP.
   - Para VMs Linux, escolha **SSH** e siga as instruções para conectar via terminal.

## Conclusão

Parabéns! Você criou com sucesso uma máquina virtual no Azure. Para mais configurações e gerenciamento de sua VM, visite a [documentação oficial do Azure](https://docs.microsoft.com/azure/virtual-machines/).
