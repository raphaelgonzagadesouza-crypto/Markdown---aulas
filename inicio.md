
# Guia Sinistra

### Configuração de Software
  Este repositório apresenta meu conhecimento sobre configurações de software.

> ## Linux
  #### Comandos básicos do Linux
  - sudo apt install x (instala o programa x)
  - sudo apt search (procurar programas/pacotes)
  - sudo apt update (buscar atualizações)
    
# Aula de Malwares

> ## O que é Malware?
Malware é qualquer software desenvolvido com a intenção de causar danos, roubar informações, espionar usuários ou obter acesso não autorizado a um sistema.

> ## Tipos de Malware

#### Ransomware
- Criptografa arquivos da vítima.
- Exige pagamento de resgate para recuperação.
- Sintomas: arquivos com extensões alteradas e nota de resgate.
- Ferramenta: Explorador de Arquivos.

#### Keylogger
- Registra tudo o que é digitado pelo usuário.
- Rouba senhas e informações confidenciais.
- Sintomas: atividade suspeita em segundo plano e arquivos de log.
- Ferramentas: Gerenciador de Tarefas e PowerShell (`Get-Process`).

#### Cryptojacker
- Usa CPU/GPU da vítima para minerar criptomoedas.
- Sintomas: uso elevado da CPU, lentidão e superaquecimento.
- Ferramentas: `top`, `htop` e Gerenciador de Tarefas.

#### Backdoor
- Permite acesso remoto não autorizado ao computador.
- Sintomas: portas de rede abertas e conexões suspeitas.
- Ferramentas: `netstat -an` e `netstat -ano`.

#### Trojan
- Disfarça-se de programa legítimo.
- Depende da ação do usuário para ser executado.
- Sintomas: processos suspeitos em segundo plano.
- Ferramentas: Gerenciador de Tarefas e propriedades do arquivo.


> ## Ferramentas de Diagnóstico

#### Windows
- `Ctrl + Shift + Esc` → Gerenciador de Tarefas.
- `resmon` → Monitor de Recursos.
- `netstat -ano` → Conexões e portas abertas.
- `Get-Process` → Lista processos ativos.
- `eventvwr` → Visualizador de Eventos.

#### Linux
- `top` / `htop` → Uso de CPU e processos.
- `ps aux` → Lista processos.
- `netstat -an` → Conexões de rede.
- `lsof -i` → Arquivos e conexões abertas.

# Aula de Diagnóstico de Problemas em Software
Este material apresenta conceitos básicos para identificar, diagnosticar e resolver problemas de software utilizando ferramentas nativas do Windows.

> ## Tipos de Problemas

#### Bug
- Programa trava ou fecha inesperadamente.
- Geralmente causado por falhas no código.

#### Configuração
- Programa não inicia devido a parâmetros incorretos.
- Pode ser resolvido ajustando as configurações.

#### Dependência
- Bibliotecas ou componentes ausentes impedem a execução do software.
- Normalmente requer instalação de componentes adicionais.

#### Desempenho
- Alto consumo de CPU ou memória.
- Sintomas: lentidão e baixa performance do sistema.

#### Serviço
- Serviço do Windows parado ou com falha.
- Pode impedir o funcionamento de aplicações.

> ## Ferramentas de Diagnóstico

#### Gerenciador de Tarefas (`Ctrl + Shift + Esc`)
- Monitorar uso de CPU e memória.
- Identificar processos com alto consumo.
- Gerenciar programas de inicialização.

#### Visualizador de Eventos (`eventvwr`)
- Consultar logs do sistema.
- Identificar erros e eventos críticos.
- Auxiliar na investigação de falhas.

#### Gerenciamento de Serviços (`services.msc`)
- Iniciar e parar serviços.
- Configurar inicialização automática ou manual.
- Definir ações de recuperação após falhas.

#### Prompt de Comando (CMD)
- `ipconfig` → Exibe informações da rede.
- `ipconfig /all` → Exibe detalhes completos da configuração.
- `tasklist` → Lista processos em execução.
- `taskkill` → Finaliza processos pela linha de comando

# Aula de Otimização de Software

> ## Tipos de Manutenção

#### Preventiva
- Evita problemas antes que ocorram.
- Ex.: limpeza de arquivos, atualizações e antivírus.

#### Corretiva
- Corrige falhas após acontecerem.
- Ex.: remover vírus e reinstalar drivers.

#### Preditiva
- Monitora o sistema para prevenir futuras falhas.
- Ex.: temperatura da CPU e SMART do HD.

> ## Ferramentas do Windows

- `cleanmgr` → Limpeza de Disco.
- `%temp%` → Remove arquivos temporários.
- Windows Update → Instala atualizações e correções.
- Windows Defender → Proteção e varredura contra malwares.
- `sfc /scannow` → Repara arquivos do sistema.
- Gerenciador de Tarefas → Gerencia processos e programas de inicialização.

# Aula de Compatibilidade e Conflitos de Software

> ## Compatibilidade de Software

- Permite que um programa funcione corretamente em diferentes sistemas.
- Envolve compatibilidade com sistema operacional, hardware e versões.

> ## Principais Causas

- Sistema operacional incompatível.
- Dependências desatualizadas.
- Falta de permissões.
- Drivers ou hardware sem suporte.

> ## Soluções

#### Modo de Compatibilidade
- Executa programas antigos em versões mais novas do Windows.
- Indicado para softwares com pequenas incompatibilidades.

#### Máquina Virtual (VM)
- Permite instalar outro sistema operacional dentro do computador.
- Ideal para executar programas antigos ou específicos.

#### Softwares Alternativos
- Utilizar programas mais atuais quando o original não possui mais suporte.
- Buscar alternativas em sites oficiais ou projetos open-source.

# Aula de Manutenção de Software

> ## Papel do Técnico

Um técnico deve seguir um processo organizado:

- Investigar os sintomas.
- Analisar as possíveis causas.
- Aplicar a solução adequada.
- Documentar todo o procedimento.

> ## Ferramentas Essenciais do Windows

- **Gerenciador de Tarefas:** monitora CPU, memória, disco e processos.
- **services.msc:** gerencia serviços do Windows.
- **msconfig:** configura inicialização e opções de boot.
- **Visualizador de Eventos:** identifica erros do sistema.
- **Limpeza de Disco:** remove arquivos temporários.
- **Windows Update:** instala atualizações e correções.

> ## Etapas da Manutenção

- Instalação de softwares e sistemas.
- Configuração do ambiente.
- Atualização de drivers e sistema.
- Diagnóstico de falhas.
- Otimização do desempenho.

> ## Problemas Mais Comuns

- Programas iniciando automaticamente.
- Serviços essenciais desativados.
- Alto consumo de CPU ou memória.
- Erros recorrentes do sistema.
- Falta de manutenção preventiva.

> ## Metodologia de Diagnóstico

- Fazer perguntas antes de agir.
- Levantar hipóteses com base nos sintomas.
- Utilizar ferramentas para confirmar o problema.
- Identificar a causa e aplicar a solução.

> ## Casos Práticos

Durante a atividade são analisados cinco tipos de problemas:

- Inicialização automática.
- Serviços parados.
- Alto consumo de recursos.
- Erros do sistema.
- Falta de manutenção.



> ## Informações Complementares

<img width="550" height="426" alt="cage-bunny" src="https://github.com/user-attachments/assets/92d1099e-d0e4-4dbb-a8d8-d8e5552420e7" />

