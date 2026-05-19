=================================================================
  IDE MINI-PASCAL — ANALISADOR LÉXICO
  Universidade Eduardo Mondlane | LPC 2026
=================================================================

FICHEIROS DO PROJECTO:
  1. analisador_lexico.py  — Núcleo do analisador (AFD)
  2. sugestoes_ia.py       — Módulo de sugestões via IA (Claude)
  3. ide_mini_pascal.py    — Interface gráfica principal (IDE)
  4. README.txt            — Este ficheiro

REQUISITOS:
  • Python 3.8 ou superior
  • Tkinter (incluído no Python padrão)
  • Ligação à Internet (opcional, apenas para sugestões da IA)

COMO EXECUTAR:
  1. Certifique-se que os 3 ficheiros .py estão na mesma pasta.
  2. Abra o terminal nessa pasta.
  3. Execute:
        python ide_mini_pascal.py
     ou:
        python3 ide_mini_pascal.py

FUNCIONALIDADES DA IDE:
  • Editor de código com realce de sintaxe a cores
  • Numeração de linhas em tempo real
  • Análise léxica com F5 ou menu Analisar → Executar
  • Tabela de tokens com: Nº, Lexema, Classe, Linha, Coluna
  • Filtragem de tokens na tabela
  • Painel de erros com localização exacta
  • Botão "Pedir Sugestões à IA" para correcções automáticas
  • Resumo estatístico (contagem por categoria)
  • Abrir/Guardar ficheiros .pas/.txt
  • Suporte a comentários { ... } e (* ... *)
  • Recuperação de erros: análise continua após símbolos inválidos

TOKENS RECONHECIDOS:
  RESERVADA_*        — program, var, begin, end, if, then...
  IDENTIFICADOR      — nomes de variáveis e funções
  CONSTANTE_INTEIRA  — números como 0, 42, 1000
  CONSTANTE_CARACTERE— literais como 'a' ou ''abc''
  OP_*               — :=, +, -, *, =, <>, <, <=, >, >=
  DELIM_*            — ( ) [ ] , ; . .. :
  TIPO_*             — char, integer, boolean
  FIM_DE_FICHEIRO    — marcador EOF

ATALHOS DE TECLADO:
  F5          — Executar análise léxica
  Ctrl+N      — Novo ficheiro
  Ctrl+O      — Abrir ficheiro
  Ctrl+S      — Guardar ficheiro
  Ctrl+Shift+S— Guardar Como
=================================================================
