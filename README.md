# Lab-DIO-AZ900
Resumo das aulas aprendidas

O Azure é a nuvem da Microsoft. Ele serve para guardar dados, rodar sistemas e criar aplicações pela internet, sem precisar de servidor físico.

# 1. Regiões

São os locais físicos onde ficam os datacenters do Azure (ex: Brasil, EUA, Europa).
Você escolhe a região mais perto para ter menos atraso e mais velocidade.

# 2. Resource Group (Grupo de Recursos)

É como uma pasta.
Dentro dela você coloca tudo que faz parte de um sistema (máquina virtual, banco, rede etc).

# 3. Computação (Compute)

É onde o sistema “roda”.

Exemplos:

Máquina Virtual (VM) → computador na nuvem

App Service → site ou API sem se preocupar com servidor

Azure Functions → código que roda só quando é chamado

# 4. Armazenamento (Storage)

Serve para guardar arquivos e dados.

Exemplos:

Blob Storage → imagens, vídeos, documentos

File Storage → parecido com uma pasta de rede

Discos → usados pelas máquinas virtuais

# 5. Segurança e Identidade

Controla quem pode acessar o quê.

Exemplos:

Azure Active Directory (Entra ID) → login e permissões

RBAC → controle de acesso por função

# 6. Monitoramento

Para ver se está tudo funcionando.

Exemplos:

Azure Monitor

Application Insights

Logs e alertas

## Computação e Rede

 * 1 Serviços de Computação e Máquinas Virtuais do Azure:

A Computação do Azure é um Serviço sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

# Conjunto de Dimensionamento de VMS:
 
  Oferecem uma oportunidade de balanceamento de carga para dimensionar os recursos automaticamente. 

Conjunto de Disponibilidade de VMS:
 

# Área de trabalho Virtual:
 
  - crie um ambiente completo de virtualização da área de trabalho sem precisar exeecutar outros servidores de gateway.
  - Reduza o risco de que o recurso seja deixado para trás.
  - Implantações reais de várias sessões. 
  OBS: hoje o AVD foi descontinuado e a ferramenta que substitui é o windows APP.

# Conteineres do Azure:
  Fornece um ambiente leve e virtualizado.

  - Instâncias de Conteiner do Azure: uma oferta de PaaS que executa um conteiner ou pod de conteineres.

  - Aplicativos de Conteineres do AZ: uma oferta de PaaS, como instãncias de coneiteres, que pode balancear a carga e escalar. 

  - Serviço de Kubernetes do Az: um serviço de orquestração para conteineres com arquiteturas distribuidas e grandes volumes de conteineres. 

# Azure Functions: 
  Uma oferta de PaaS que dá suporte a operações de computação sem servidor.

# Serviços de rede do AZ

 A rede virtual do AZ (VNet) permite que os recursos do azure se comuniquem uns com os outros, com a internet e com as redes locais. 
 As sub-redes virtuais segmeta sua rede para atender às suas necessidades.
 O emparelhamento de rede conecta suas rede privadas diretamente.

 # Gateway de VPN:
   É usado para enviar tráfego criptografado entre uma rede virtual do Azure e uma no local pela internet pública.
  - ExpressRoute estende as redes locais para o Azure por meio de uma conexão privada facilitada por um provedor de conectividade. 
  - DNS do Azure: 
  
    * Confiabilidade e desempenho aproveitando uma rede global de servidores de nome DNS usando rede Anycast. 
    * a segurança do DNS do AZ baseia-se no gerenciador de recursos do AZ, habilitando o controle de acesso baseado em função e o monitoramento e o registro em log. 
    * Facilidade de uso para gerenciar seus recursos externos com um único serviço.
    * As rede virtuais personalizaveis que permitem que use nomes de domínio privados e totalmente personalizados em suas redes virtuais privadas. 
    

 





