graph TD
    % 1. Definição dos Acionistas
    A1["Lenita R. do Prado (15%)"]
    A2["Carlos Prado Filho (15%)"]
    A3["Antônio M. R. do Prado (15%)"]
    A4["Marilena R. do Prado (15%)"]
    A5["Mariana B. Prado (5%)"]
    A6["José R. Prado Filho (5%)"]
    A7["Amanda P. Teixeira (4,37%)"]
    A8["Giulia P. Teixeira (4,37%)"]
    A9["José Carlos P. Sombra (4,37%)"]
    A10["Guido A. Prado (4,37%)"]
    A11["Taís A. Prado (4,37%)"]
    A12["Lara A. Prado (4,37%)"]
    A13["Adriana R. do Prado (1,89%)"]
    A14["José Luís R. do Prado (1,89%)"]

    % 2. Definição da Holding e Subsidiárias
    B(Itaueira Agropecuária S/A)
    C1(ITAUEIRA NEGÓCIOS IMOBILIÁRIOS LTDA.)
    C2(ITAUEIRA COMERCIAL LTDA.)
    C3(ITAUEIRA CAMARÕES LTDA.)
    C4(ITAUEIRA IMOBILIÁRIAS LTDA.)
    C5(ITAUEIRA INDUSTRIAL LTDA.)

    % 3. Conexões
    % Cria a linha horizontal de acionistas
    A1 --- A2 --- A3 --- A4 --- A5 --- A6 --- A7 --- A8 --- A9 --- A10 --- A11 --- A12 --- A13 --- A14
    
    % Conecta a linha de acionistas (a partir de um nó central) à Holding
    A7 --> B
    
    % Conecta a Holding às suas subsidiárias
    B --> C1
    B --> C2
    B --> C3
    B --> C4
    B --> C5

    % Estilo da caixa principal
    style B fill:#f9f,stroke:#333,stroke-width:2px# Organograma
