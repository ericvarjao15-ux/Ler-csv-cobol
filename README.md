📊 Leitor de Arquivos CSV em COBOL

Este é um programa em COBOL desenvolvido para ler e processar arquivos delimitados por vírgula (CSV). O código realiza a leitura do cabeçalho, faz o parse (UNSTRING) de cada registro e exibe os dados organizados no terminal.

📋 Funcionalidades

Leitura Sequencial: Leitura de arquivos linha por linha (LINE SEQUENTIAL).

Tratamento do Cabeçalho: Lê a primeira linha e identifica as colunas separadamente.

Divisão de Campos (UNSTRING): Divide a linha por vírgula (,) populando uma estrutura com array (OCCURS 3 TIMES).

Contagem de Registros: Exibe os dados numerando cada registro processado.

🛠️ Tecnologias e Dependências

Linguagem: COBOL (Dialeto COBOL-85 / COBOL 2002)

Compilador recomendado: GnuCOBOL
 (cobc)

🚀 Como Executar
1. Clonar o repositório
git clone https://github.com/seu-usuario/Ler-csv-cobol.git
cd Ler-csv-cobol

2. Compilar o código
cobc -x -o lercsv lercsv.cob

3. Executar o programa
./lercsv < exemplo.csv

📄 Exemplo de arquivo CSV
Nome,Idade,Cidade
Eric,22,Sao Paulo
Ana,25,Rio de Janeiro

💻 Saída do terminal
cabecalho:
Dado 1: Nome
Dado 2: Idade
Dado 3: Cidade

Registro #00001:
Dado 1: Eric
Dado 2: 22
Dado 3: Sao Paulo

Registro #00002:
Dado 1: Ana
Dado 2: 25
Dado 3: Rio de Janeiro
