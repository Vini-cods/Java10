# Calculadora Java

Uma calculadora implementada em Java com interface gráfica elegante usando Swing, que realiza operações matemáticas básicas.

## 📋 Funcionalidades

- **Interface gráfica elegante**: Interface visual moderna construída com Java Swing
- **Soma**: Adição de números decimais
- **Subtração**: Subtração de números decimais
- **Multiplicação**: Multiplicação de números decimais
- **Divisão**: Divisão de números decimais com proteção contra divisão por zero
- **Display interativo**: Tela que exibe números e resultados em tempo real
- **Botão Clear (C)**: Limpa o display e reinicia os cálculos
- **Tratamento de erros**: Mensagens de erro para divisão por zero e entradas inválidas

## 🚀 Como usar

### Pré-requisitos

- Java JDK 8 ou superior instalado
- Java Swing (incluído no JDK)

### Compilação

```bash
javac Main.java
```

### Execução

```bash
java Main
```

Após executar, uma janela gráfica será exibida com a interface da calculadora.

## 📁 Estrutura do projeto

```
projeto/
├── Main.java          # Classe principal com interface gráfica Swing
└── README.md          # Este arquivo
```

## 🔧 Componentes da Interface

### `Main`

Classe principal que implementa toda a lógica da calculadora e sua interface gráfica.

#### Componentes visuais:

- **JFrame**: Janela principal da aplicação (400x600 pixels)
- **JTextField**: Display para mostrar números e resultados
- **JPanel**: Painel organizador dos botões em grade 4x4
- **JButton**: 16 botões para números, operadores e funções

#### Layout dos botões:

```
[ 7 ]  [ 8 ]  [ 9 ]  [ / ]
[ 4 ]  [ 5 ]  [ 6 ]  [ * ]
[ 1 ]  [ 2 ]  [ 3 ]  [ - ]
[ C ]  [ 0 ]  [ = ]  [ + ]
```

#### Funcionalidades dos botões:

- **Números (0-9)**: Inserem dígitos no display
- **Operadores (+, -, *, /)**: Definem a operação a ser realizada
- **Igual (=)**: Executa o cálculo e mostra o resultado
- **Clear (C)**: Limpa o display e reinicia a calculadora

## 💡 Como usar a interface

1. **Execute o programa** para abrir a janela da calculadora
2. **Clique nos números** para inserir valores no display
3. **Clique em um operador** (+, -, *, /) para definir a operação
4. **Digite o segundo número**
5. **Pressione "="** para calcular o resultado
6. **Use "C"** para limpar e começar um novo cálculo

### Exemplo de sequência:
- Clique em: `5` → `+` → `3` → `=`
- Resultado: `8.0` será exibido no display

## ⚠️ Tratamento de erros

- **Divisão por zero**: Exibe "Erro: Divisão por zero" no display
- **Entrada inválida**: Mostra "Entrada inválida" quando há problemas na formatação dos números
- **Reset automático**: Após um erro, use "C" para limpar e reiniciar

## 🖼️ Características visuais

- **Janela**: 400x600 pixels com título "Calculadora Elegante"
- **Display**: Campo de texto alinhado à direita com fonte Arial Bold 24pt
- **Botões**: Grade 4x4 com fonte Arial Bold 20pt e espaçamento de 5px
- **Layout**: BorderLayout com display no topo e botões no centro

## 📝 Notas técnicas

- Utiliza **Java Swing** para a interface gráfica
- Implementa **ActionListener** para capturar eventos dos botões
- Trabalha com números decimais (`double`) para maior precisão
- Usa arrays para armazenar estado (números e operador atual)
- **GridLayout** (4x4) para organização dos botões
- **BorderLayout** para estrutura geral da janela
- Tratamento de exceções com `try-catch` para `NumberFormatException`
