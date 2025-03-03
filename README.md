# Segurança no Azure

- Identidade, Acesso e Segurança
  
  - A implementação da segurança é de responsabilidade do cliente.
    
- Microsoft Entra ID

  - É o serviço de gerenciamento de identidades e acesso baseado em nuvem do Microsoft Azure.
  
  - Teve seu nome reformulado de Azure Active Directory para Microsoft Entra ID.
  
  - Serviço de diretórios, ao fazer o logon, toda a verificação relacionada a segurança é feita pelo Entra ID.
  
  - Logon único.
  
  - Sistema B2B, onde utilizamos outro serviço de autenticação para validar a entrada dos usuários no sistema, como pode exemplo, o login feito pelo Google, GitHub, etc.
  
  - A sincronização de usuários de um datacenter local para um domínio em nuvem pode ser feita através do locatário do Microsoft Entra ID.
  
  - Possibilidade de continuar salvando os usuários dentro do datacenter local e de maneira automática (após a configuração), o usuário salvo será replicado na nuvem, o usuário criado na nuvem não replica para o datacenter local.


### Autenticação vs Autorização

- Autenticação
  - Identifica a pessoa ou serviço buscando acesso a um recurso.
  - Solicita credenciais de acesso legítimo.
  - Base para criar princípios de identidade e controle de acesso seguros.

- Autorização
  - Determina o nível de acesso de uma pessoa ou serviço autenticado.
  - Define quais dados eles podem acessar e o que podem fazer com eles.

- Autenticação multifatorial (NFA)
  - Fornece segurança adicional para as identidades, exigindo dois ou mais elementos para autenticação completa.
  - Um exemplo de NFA é a necessidade de confirmar o login por um celular ou e-mail.
  - Pilares do NFA: “algo que você sabe”, “Algo que você possui” e “Algo que você é”

### Autenticações B2B do Microsoft Entra External ID

- Será uma colaboração externa através do Google, Facebook, Azure, etc. Para que o Microsoft Entra External ID permita acesso ao sistema.

### Autenticações B2C do identidades External do Azure ID

- A empresa cede uma parte dos seus recursos para que o usuário consiga acessar e consumir os recursos fornecidos.

- O provedor (Google, Facebook, GitHub) garante que o usuário está registrado e que a conta dele pode ser permitida no sistema.

### Acesso Condicional

- Associação de usuário ou grupo.

- Local do IP.

- Dispositivo.

- Aplicativo.

- Detecção de risco.

### Controle de acesso baseado em função (RBAC).

- Gerenciamento de acesso de granularidade fina.

- Divida as tarefas dentro da equipe e conceda somente a quantidade de acesso de que os usuários precisam para trabalhar.

- Habilite o acesso ao portal do Azure e o controle de acesso aos recursos.

- Monitoramento total do que o usuário está fazendo.

### Confiança Zero

- Protege os ativos em qualquer lugar com uma política central.

- A execução é responsabilidade do cliente.

- Proteção completa
  
  - Uma abordagem em camadas para proteger sistemas.
  
  - Pilares: Segurança física, identidade e acesso, perímetro, rede, computação, aplicativo e dados.
  
  - Uma abordagem em camadas para proteger sistemas de computador.
  
  - Fornece vários níveis de proteção.
  
  - Ataques contra uma camada são isolados das camadas subsequentes.
  
### Microsoft Defender para Nuvem

- O Microsoft Defender para Nuvem é um serviço de monitoramento que fornece proteção contra ameaças nos datacenters do Azure e locais.

- Faz a configuração para o ambiente da AWS e GCP.

- Análise de vulnerabilidade.
