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

#  Armazenamento no Azure
   Redundância de Armazenamento:

  * LRS (armazenamento com redundância local) -> Implantação: Datacenter individual na região priária -> Durabilidade 11 noves; 
  * ZRS (armazenamento com redundância de zona) -> Implantação de três zonas de disponibilidade na região primária -> 12noves;
  * GRS (armazenamento com redundância geográfica) -> Implantação Datacenter único no primário e região secundária -> Durabilidade 16 noves;
  * GZRS (armazenamento com redundância de zona geográfica) -> Implantação de três zonas de disponibilidade na região primária e um único datacenter na região secundária -> 16 noves;

  Migração para o Azure

   * Plataforma de migração unificada;
   * Intervalo de ferramentas integradas e autônomas;
   * Avaliação e migração;

  OBS: o Azure Data Box auxilia a realizar migração, movendo até 80TB de dados do datacenter local e migrando para nuvem.

  Opções de gerenciamento de arquivos

   * AzCopy: 
     -> Utilitátio de linha de comando;
     -> Copiar blobs ou arquivos de ou para sua conta de armazenamento;
     -> Sincronização em uma direção.

   * Gerenciador de Armazenamento do Azure:
     -> Interface gráfica do usuário (de modo semelhante ao windows explorer);
     -> Compatível com windows, MacOs e Linux;

   * Sincronização de Arquivos do Azure:
     -> Sincroniza os arquivos do Azure e locais de forma bidirecional;
     -> Acamada de nuvem mantém os arquivos acessados com frequencia no local, enquanto libera espaço.

# Identidade, Acesso e Segurança

   * Entra ID: 
      Serviço de gerenciamento de identidade e acesso baseado em nuvem do microsoft Azure. 
      -> Autenticação 
      -> logon único (SSO)
      -> Gerenciamento de aplicativos
      -> Negócios para Negócios (B2B)
      -> Gerenciamento de dispositivos.

   * Autenticação e Autorização
     -> Autenticação: identifica a pessoa ou serviço buscando acesso a um recurso; solicita credenticiais de acesso legítimo; Base para criar princípios de identidade e controle de acesso seguros.

     -> Autorização: Determina o nível de acesso de uma pessoa ou serviço autenticado; Define quais dados eles podem acessar e o que podem fazer com eles. 

     -> Autenticação 2 fatores (MFA): Forenece segurança adicional para as identidades, exigindo dois ou mais elementos para autenticação completa. 

   * Acesso Condicional

     -> Associação de usuário ou grupo; local do IP; Dispositivo; Aplicativo; Detecção de risco.
   
   * Controle de acesso baseado em função:

    -> Gerenciamento de acesso de granularidade fina; 
    -> Divida as tarefas dentro da equipe e conceda somente a quantidade de acesso de que os usuários precisam para trabalhar;
    -> Habilite o acesso ao portal do Azure e o controle de acosso aos recursos.

  * Confiança Zero

   -> Proteja os ativos onde eles estiverem com a confiança zero.
    - Abordagem clássica: Restringe tudo a uma rede "segura"
    - Confiança Zero: Protege os ativos em qualquer lugar com uma política central

   -> Proteção completa: segurança física - Identidade de acesso - Perímetro - Rede - Computação - Aplicativo - Dados.

   -> Microsoft Defender para Nuvem: é um serviço de monitoramento que fornece proteção contra ameaças nos datacenters do Azure e locais. 

# Gerenciamento de Custos no Azure

 * # Gerenciamento de Custos:
  -> Calculadora de custos e preços
  -> Gerenciamento de custos e marcas

  Fatores que afetam os custos:

  1) Tipo de recurso: Os custos são específicos do recurso, portanto, o uso que um medidor rastreia e o número de medidores associados a um recurso, dependendo do tipo de recurso.

  2) Consumo: Com um modelo pago conforme o uso, o consumo é um dos maiores geradores de custos. 

  3) Manutenção: Monitorar seu volume do Azure e manter seu ambiente pode ajudá-lo a identificar e reduzir os custos que não são necessários, como ao desligar máquinas virtuais subutilizadas. 

  4) Área Geográfica: O mesmo tipo de recurso pode custar valores diferentes dependendo da área geográfica, o que afeta os custos do Azure.

  5) Tráfego de REde: Embora algumas transferências de dados de entrada sejam gratuitas, o custo para dados de saída ou dados entre recursos do Azure é afetado por zonas de cobrança.

  6) Assintatura: O tipo e a configuração da assintura também podem afetar o custo. Por exemplo, avalição gratuita permite explorar alguns recursos do Azure gratuitamente. 

* # Azure Marketplace:

 Permite que os clientes encontrem, experimente, comprem e provisonem aplicativos e serviços de centenas de provedores de serviços líderes, que são todos certificados para execução no Azure. 

* # Calculadora de Preços:

 Ferramenta que ajuda a estimar o custo dos produtos do Azure. As opções que podem ser configuradas na calculadora preços variam entre produtos, mas as opções básicas de configuração incluem:
  - Região
  - Camada
  - Opções de Cobrança
  - Opções de Suporte
  - Programas e Ofertas
  - Preço de Desenvolvimento/Teste do Azure

* # Calculadora de Custo Total de Propriedade (TCO)
 - Ferramenta para estimar a economia de custos possível ao migrar para o Azure.
 - Um relatório compara os custos das infraestruturas locais com os custos de uso de produtos e serviços do Azure na nuvem.

* # Marcas
 - Fornecem metadados aos recursos do Azure.
 - Organizam os recursos em uma taxonomia de maneira lógica.
 - Consistem em um par nome-valor.
 - Muito úteis para reunir informações de cobrança.


  


 





