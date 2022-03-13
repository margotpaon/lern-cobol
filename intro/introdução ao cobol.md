# Introdução ao COBOL

- COBOL (sigla de COmmon Business Oriented Language) - Linguagem Comum Orientada para os Negócios é uma linguagem de programação orientada para o processamento de banco de dados comerciais.

- Ele possue 4 divisões importantes que são elas:

  - **IDENTIFICATION DIVISION**: - Essa divisão serve para passar informações documentais para que pessoas que não são programadoras possa entender superficialmente o que acontece. E ela possue as seguintes sessões **PROGRAM-ID** é onde damos nome para o programa e ele deve ter de 1 a 30 caracteres e 8 para Mainframe antigos, **AUTHOR** claúsula opcional para colocar o nome do programador, **DATE-WRITTEN** é opcional e serve para informar quando o programa foi criado, **DATA-COMPILED** outra opcional fala quando o programa foi compilado, **SECURITY** podem conter ou não informações sobre o acesso ao programa e **REMARKS** opcional que pode conter observações, históricos de atualizações e demais autores.

  - **ENVIRONMENT DIVISION**: - Serve para fazer a ligação entre o sistema operacional e o programa e possue duas sessões **_*CONFIGURATION SECTION*_** e **_*INPUT-OUTPUT SECTION*_**.

    - A **_CONFIGURATION SECTION_** é onde é feita a configuração do ambiente e é composto por 3 partes **_SOURCE-COMPUTER_** que identifica qual computador foi feito, **_OBJECT-COMPUTER_** identifica o computador do ambiente de produção.
      As duas primeiras servem apenas para comentários e não são obrigatórias somente se o programador as declarar **_SPECIAL-NAMES_** já essa sessão é onde se específica o sinal monetário, tipo de ponto decimal, caracteres simbólicos e também possibilita a comunicação do programa com outros programas de outras linguagens.

    - A **INPUT-OUTPUT SECTION** destina-se a configuração do ambiente de Leitura e Gravação e possue duas partes **FILE-CONTROL** que serve para especificação dos arquivos que o programa irá acessar e a **I-O-CONTROL** que foi descontinuada em versões mais atuais, valendo apenas para ambientes de MainFrame.

  - **DATA DIVISION** é onde definimos estruturas de registros, váriaveis e constantes do programa, ou seja, essa divisão é responsável pela alocação de memória e nele temos as seguintes sessões: **FILE SECTION** descre os dados armazenados externamente, **WORKING-STORAGE SECTION** descreve os dados internos, **LOCAL-STORAGE SECTION** descreve os dados internos que são alocados por invocação e a **LINKAGE SECTION** aqui teremos dados dispobilizados por outro programa.

  - **PROCEDURE DIVISION**
