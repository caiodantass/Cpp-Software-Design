# ⚡ C++ Object-Oriented Software Design & Architecture

[![C++](https://img.shields.io/badge/Language-C%2B%2B11%20%2F%2014-00599C.svg?logo=c%2B%2B)](https://isocpp.org/)
[![Architecture](https://img.shields.io/badge/Architecture-Clean%20OOP-success.svg)](#principais-habilidades-técnicas)
[![Build Tool](https://img.shields.io/badge/Build-Makefile-lightgrey.svg?logo=gnu)](Makefile)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

Coleção de soluções em **C++ Moderno** com foco em modelagem de domínio, arquitetura orientada a objetos, robustez contra falhas e padrões de projeto limpos e desacoplados.

O repositório demonstra a aplicação prática de engenharia de software na resolução de problemas complexos de simulação, modularização de sistemas corporativos e streaming multimídia.

---

## 🎯 Destaques do Projeto

* **Arquitetura Polimórfica & Extensível**: Design de hierarquias desacopladas preparadas para extensão sem quebra de contratos estabelecidos (Open/Closed Principle).
* **Sobrecarga Expressiva de Operadores**: Criação de interfaces fluentes e código idiomático em C++ com `operator<<` e `operator>>`.
* **Tratamento Robusto de Exceções**: Resiliência sistêmica contra falhas de execução via `std::exception` handling.
* **Automação de Build Multi-ambiente**: Compilação otimizada com suporte a `Makefile`, garantindo reprodutibilidade em ambientes Linux/Unix e Windows.

---

## 🏗️ Módulos do Sistema

### 1. 🎬 Smart TV & Streaming Multimedia Engine
> *Sistema completo de simulação de ecossistema de entretenimento sob demanda.*

* **Domínio Modelado**: Gerenciamento de ciclo de vida de dispositivos inteligentes, execução assíncrona/temporal de mídias e ecossistema de aplicações instaláveis.
* **Design das Classes**:
  * **Core de Execução**: `SmartTV`, `App`, `Streaming`, `Time`.
  * **Motor Polimórfico de Mídia**: `Producao` (classe base polimórfica), `Filme`, `Serie`.
  * **Entidades Relacionais**: `Pessoa`, `Ator`, `Diretor`.
* **Diferenciais Técnicos**:
  * Abstração de contratos de reprodução via métodos virtuais (`play()`).
  * Gestão de dependências dinâmicas entre plataformas de streaming (Netflix, Prime Video, HBO Max) e catálogo de produções.
  * Parser e persistência de dados em formato de arquivo texto estruturado (`tv.txt`).

---

### 2. 📺 Hardware Device & App Lifecycle Management
> *Modelagem de baixo acoplamento para gestão de recursos e ciclo de vida de periféricos.*

* **Domínio Modelado**: Instalação, desinstalação e monitoramento de consumo de aplicativos em dispositivos smart.
* **Design das Classes**: `SmartTV`, `Aplicativo`.
* **Diferenciais Técnicos**:
  * Sobrecarga idiomática de operadores de fluxo para manipulação de hardware:
    ```cpp
    tv << netflix;   // Instalação elegante e limpa
    tv >> instagram; // Desinstalação com validação de estado
    ```
  * Encapsulamento estrito e integridade de estado garantida por invariantes da classe.

---

### 3. 🏢 Corporate Domain & Identity System
> *Engine de modelagem de regras de negócio corporativas e representação de identidades.*

* **Domínio Modelado**: Entidades fiscais, controle de pessoal e relacionamento B2B/B2C.
* **Design das Classes**: `Pessoa`, `PessoaFisica`, `PessoaJuridica`, `Cliente`, `Funcionario`, `Empresa`.
* **Diferenciais Técnicos**:
  * Herança em múltiplos níveis com isolamento de responsabilidades.
  * Formatação e serialização personalizada de fluxos de saída via sobrecarga de `std::ostream`.

---

## 🧠 Principais Habilidades Técnicas Demonstradas

| Habilidade / Conceito | Aplicação no Projeto |
| :--- | :--- |
| **Abstração & Encapsulamento** | Modelagem orientada a domínio com proteção estrita de atributos e interfaces públicas claras. |
| **Polimorfismo em Tempo de Execução** | Classes base virtuais (`Producao`) permitindo tratamento genérico de catálogos e execuções dinâmicas. |
| **Operator Overloading** | Implementação de semânticas customizadas de entrada/saída e injeção de recursos (`<<`, `>>`). |
| **Tratamento de Exceções** | Blocos de tratamento preventivo de falhas de hardware, rede e limites de memória. |
| **Gestão de Dependências e Build** | Estruturação modular com separação clara de headers (`.h`), implementação (`.cpp`) e compilação via `Makefile`. |

---

## 🛠️ Stack Tecnológica

* **Linguagem Principal**: C++ (ISO/IEC 14882)
* **Compilador**: GCC / Clang
* **Sistema de Automação de Build**: GNU Make
* **Controle de Versão**: Git & GitHub

---

## 🚀 Como Compilar e Rodar Localmente

### Pré-requisitos
* Compilador C++ com suporte a C++11 ou superior (`g++` / `clang++`)
* Utilitário `make` instalado

### Passo a passo

```bash
# 1. Clone o repositório
git clone https://github.com/caiodantass/POO.git
cd POO

# 2. Acesse o módulo desejado (exemplo: Motor de Streaming)
cd "PROJETO_FINAL - POO"

# 3. Compile utilizando o Makefile automatizado
make

# 4. Execute a aplicação
./main
```

> **Compilação direta alternativa**:
> ```bash
> g++ -std=c++11 -Wall -Wextra *.cpp -o main && ./main
> ```

---

## 👨‍💻 Autor

**Caio Dantas**  
* Engenheiro de Software / Desenvolvedor  
* GitHub: [@caiodantass](https://github.com/caiodantass)  
* LinkedIn: [linkedin.com/in/caiodantass]([https://linkedin.com/in/caiodantass](https://www.linkedin.com/in/caio-l%C3%ADvio/])) 
