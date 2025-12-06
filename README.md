![python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

# 🎯 Programação Orientada a Objetos (POO)

Repositório desenvolvido para acompanhar o módulo **Programação Orientada a Objetos** durante a [Formação Python](https://www.rocketseat.com.br/formacao/python) da [Rocketseat](https://www.rocketseat.com.br/).

## 📋 Sobre o Módulo

Este módulo aprofunda os conhecimentos em Python através do paradigma de Programação Orientada a Objetos (POO), explorando conceitos fundamentais para criar código mais organizado, reutilizável e escalável.

O conteúdo abrange desde os fundamentos da POO até recursos avançados como herança múltipla e decoradores, preparando para o desenvolvimento de aplicações mais complexas e profissionais.

## 🚀 Tecnologias

- Python 3.x

## 📚 Conteúdo Programático

### Fundamentos de POO

- **O que é POO**: Introdução ao paradigma orientado a objetos
- **Classes e Objetos**: Definição, instanciação e utilização
- **Atributos e Métodos**: Propriedades e comportamentos dos objetos
- **Construtor `__init__`**: Inicialização de objetos

### Pilares da POO

#### Encapsulamento

- Modificadores de acesso (público, protegido, privado)
- Convenções de nomenclatura (`_protegido`, `__privado`)
- Getters e Setters
- Proteção de dados e controle de acesso

#### Abstração

- Classes abstratas
- Métodos abstratos
- Módulo `abc` (Abstract Base Classes)
- Definição de contratos e interfaces

#### Herança

- Herança simples
- Relação "é um" (is-a)
- Sobrescrita de métodos (override)
- Método `super()`
- Reutilização de código

#### Polimorfismo

- Polimorfismo de método
- Polimorfismo de sobrecarga
- Duck typing em Python
- Flexibilidade e extensibilidade

### Conceitos Avançados

#### Herança Múltipla

- Herdar de múltiplas classes
- Função `super()`
- Boas práticas e cuidados

#### Decoradores

- **O que são decoradores**: Funções que modificam outras funções
- **Sintaxe**: Uso do `@` decorator
- **Decoradores customizados**: Criação de decoradores próprios
- **Decoradores comuns**:
  - `@staticmethod`: Métodos estáticos (sem acesso à instância)
  - `@classmethod`: Métodos de classe (acesso à classe)
  - `@abstractmethod`: Definir métodos abstratos
  - Decoradores para validação e logging

## 🛠️ Como Utilizar

1. Clone este repositório:

```bash
git clone https://github.com/devayresrouxj/rocketseat-python-oo.git
```

2. Navegue até o diretório do projeto:

```bash
cd rocketseat-python-oo
```

3. Execute os arquivos Python:

```bash
python nome_do_arquivo.py
```

## 💡 Exemplos de Conceitos

### Classe Básica

```python
class Pessoa:
    def __init__(self, nome, idade):
        self.nome = nome
        self.idade = idade
```

### Herança

```python
class Funcionario(Pessoa):
    def __init__(self, nome, idade, salario):
        super().__init__(nome, idade)
        self.salario = salario
```

### Encapsulamento

```python
class ContaBancaria:
    def __init__(self, saldo):
        self.__saldo = saldo  # Atributo privado

    @property
    def saldo(self):
        return self.__saldo
```

### Abstração

```python
from abc import ABC, abstractmethod

class Animal(ABC):
    @abstractmethod
    def fazer_som(self):
        pass
```

## 🎓 Competências Desenvolvidas

Após este módulo, você será capaz de:

- Estruturar código usando classes e objetos
- Aplicar os 4 pilares da POO em projetos reais
- Criar hierarquias de classes com herança
- Proteger dados sensíveis com encapsulamento
- Definir contratos com classes abstratas
- Implementar polimorfismo para código flexível
- Utilizar herança múltipla de forma adequada
- Criar e aplicar decoradores customizados
- Desenvolver aplicações mais organizadas e manuteníveis

## 📖 Recursos Adicionais

- [Documentação Oficial Python - Classes](https://docs.python.org/pt-br/3/tutorial/classes.html)
- [PEP 8 - Convenções de Nomenclatura](https://peps.python.org/pep-0008/#naming-conventions)
- [Real Python - OOP in Python](https://realpython.com/python3-object-oriented-programming/)
- [Python ABC Module](https://docs.python.org/3/library/abc.html)
- [Python Decorators Guide](https://realpython.com/primer-on-python-decorators/)

## 📝 Licença

Este projeto está sob a licença MIT.

---

Desenvolvido com 💜 durante a Formação Python da Rocketseat
