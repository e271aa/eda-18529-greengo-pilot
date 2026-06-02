# EDA GreenGo — Sistema de Mobilidade Elétrica

Projeto académico desenvolvido no âmbito da cadeira de **Estruturas de Dados Avançadas (EDA)**.

O sistema simula a gestão de uma empresa de mobilidade elétrica chamada **GreenGo**, permitindo gerir meios de transporte elétricos e clientes através de uma interface de consola em modo menu.

## Estruturas de Dados

O projeto utiliza **listas ligadas simples** como estrutura principal de armazenamento em memória:

- `Meio` — representa um veículo elétrico (código, tipo, bateria, autonomia)
- `Cliente` — representa um cliente registado (código, nome, telefone, endereço)
- `Gestor` — estrutura de autenticação

## Funcionalidades

### Meios de Mobilidade Elétrica
- Inserir, remover e listar meios
- Persistência em ficheiro de texto (`.txt`) e ficheiro binário (`.bin`)

### Clientes
- Inserir, remover e listar clientes
- Persistência em ficheiro de texto (`.txt`)

### Gestor
- Autenticação por username e password

## Compilação

> Requer ambiente Windows (utiliza `windows.h` e `conio.h`). Compilador recomendado: MinGW/GCC.

```bash
gcc fase1.c meio.c cliente.c -o greengo
```

## Execução

```bash
./greengo
```

## Estrutura do Projeto

```
eda-18529-greengo/
├── fase1.c      # Programa principal e menus
├── meio.c       # Lógica dos meios de transporte
├── meio.h       # Declarações de meios
├── cliente.c    # Lógica de clientes
├── cliente.h    # Declarações de clientes
└── gestor.h     # Estrutura do gestor
```

---

Desenvolvido por Ruben Martins · nº 18529
