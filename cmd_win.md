# Roteiro de Aula: Introdução ao Prompt de Comando (CMD)

**Disciplina:** Sistemas Operacionais  
**Tema:** Aula 01 - Interface de Linha de Comando, Navegação e Gerenciamento de Arquivos/Diretórios  
**Público:** Curso Técnico  
**Duração Estimada:** 2 horas/aula  

---

## 1. Introdução Teórica (20 minutos)

* **Definição:** O CMD (Command Prompt) é o interpretador de linha de comando padrão dos sistemas operacionais da família Windows NT. É uma Interface de Linha de Comando (CLI), diferente da Interface Gráfica do Usuário (GUI).
* **Justificativa de Uso:** Essencial para administração de sistemas, automação de tarefas via scripts (`.bat`), resolução ágil de problemas, diagnósticos de rede e consumo reduzido de recursos de hardware operacional.
* **Estrutura do Prompt:** Explicação da sintaxe inicial, como `C:\Users\Aluno>`.
  * `C:` - Unidade de disco atual.
  * `\Users\Aluno` - Caminho (path) ou diretório atual em que os comandos serão executados.

---

## 2. Explicação dos Comandos Básicos (40 minutos)

A execução de cada comando deve ser feita no projetor simultaneamente à explicação teórica.

### Controle da Interface
* `cls`: Limpa a tela do terminal (Clear Screen).
* `exit`: Encerra o interpretador de comandos.
* `help` ou `comando /?`: Exibe o manual e parâmetros de um comando específico.

### Navegação no Sistema de Arquivos
* `dir`: Lista os arquivos e diretórios da pasta atual. 
  * *Variações úteis:* `dir /w` (formato de lista ampla) e `dir /p` (pausa a cada página).
* `cd <nome_da_pasta>`: Entra em um subdiretório.
* `cd ..`: Sobe um nível na hierarquia de pastas.
* `cd \`: Vai direto para a raiz da unidade de disco atual.



### Gerenciamento de Diretórios
* `mkdir <nome_da_pasta>` ou `md <nome_da_pasta>`: Cria uma nova pasta.
* `rmdir <nome_da_pasta>` ou `rd <nome_da_pasta>`: Remove uma pasta (apenas se estiver vazia).
* `tree`: Mostra a hierarquia de pastas em formato de árvore visual.

### Manipulação Simples de Arquivos
* `echo Texto de exemplo > arquivo.txt`: Cria um arquivo de texto e insere a string especificada nele.
* `type arquivo.txt`: Lê e exibe o conteúdo de um arquivo de texto diretamente no terminal.
* `del arquivo.txt`: Deleta um arquivo.

---

## 3. Atividade Prática: Estruturação de Ambiente (45 minutos)

**Instruções para execução individual no laboratório:**

1. Abrir o interpretador de comandos pressionando `Win + R`, digitando `cmd` e pressionando `Enter`.
2. Navegar até a pasta raiz da unidade C: utilizando o comando adequado (`cd \`).
3. Criar um diretório chamado `Lab_Sistemas`.
4. Entrar no diretório `Lab_Sistemas`.
5. Criar a seguinte estrutura de subdiretórios dentro de `Lab_Sistemas`:
   * `Redes`
   * `Bancos_de_Dados`
   * `Manutencao`
6. Entrar no diretório `Redes`.
7. Criar um arquivo de texto chamado `config.txt` que contenha a frase "Parametros de rede local".
8. Retornar ao diretório `Lab_Sistemas`.
9. Executar o comando que exibe a árvore de diretórios (`tree`) para verificar se a estrutura foi criada corretamente.
10. Ler o conteúdo do arquivo `config.txt` diretamente pelo terminal, sem sair da pasta `Lab_Sistemas` (utilizar o caminho relativo: `type Redes\config.txt`).
11. Acessar o diretório `Manutencao` e tentar apagá-lo usando o comando `rd`. Ocorrerá um erro. Analisar e aplicar a solução correta (sair do diretório primeiro, para então apagá-lo).

---

## 4. Fechamento e Avaliação (15 minutos)

* Sessão de tira-dúvidas sobre erros comuns enfrentados durante a prática (ex: esquecer espaços ou usar barras invertidas de forma errônea).
* Verificação visual nas máquinas para confirmar o sucesso da atividade.
