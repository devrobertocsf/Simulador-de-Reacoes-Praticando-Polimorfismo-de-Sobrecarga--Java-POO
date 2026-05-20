# 🐕 Simulador de Reações - Praticando Polimorfismo de Sobrecarga (Java POO)

Este repositório foi desenvolvido para consolidar o entendimento sobre o **Polimorfismo de Sobrecarga (Estático)** em Java, demonstrando como uma única entidade pode responder a diferentes estímulos baseando-se estritamente na assinatura dos seus métodos.

## 🎯 O que é Polimorfismo de Sobrecarga?

Diferente do polimorfismo de sobrescrita (onde o método é substituído na classe filha), a sobrecarga ocorre quando temos **dois ou mais métodos com o mesmo nome dentro da mesma classe**, mas que se diferenciam por suas **assinaturas** (tipos, ordem ou quantidade de parâmetros). A decisão de qual método será chamado é tomada pelo compilador em tempo de compilação.

## 🚀 Conceitos Aplicados no Projeto

* **Sobrecarga de Métodos**: A classe `Cachorro` possui 4 variações do método `reagir()`, cada uma processando regras de negócio distintas:
* `reagir(String frase)`: Analisa o conteúdo do texto recebido (ex: "Olá" ou "Toma comida").
* `reagir(int hora, int min)`: Determina o comportamento com base no horário do dia.
* `reagir(boolean dono)`: Modifica a atitude caso a pessoa seja ou não o dono do animal.
* `reagir(int idade, float peso)`: Cruza dados de porte e maturidade do animal para ditar sua reação.


* **Sobrescrita Multi-nível (`@Override`)**: O projeto também revisita o polimorfismo dinâmico na árvore de herança do método `emitirSom()`:
* Em `Mamifero` exibe: *Som de Mamífero*
* Em `Lobo` substitui para: *Auuuuuuuu*
* Em `Cachorro` substitui para: *Au!Au!Au!*


* **Classes Abstratas**: Mantendo a segurança estrutural, a superclasse `Animal` permanece abstrata, impedindo instâncias órfãs de contexto no sistema.

## 📂 Estrutura das Classes

* `Animal.java` *(Abstract)*: Superclasse base que assina o método `emitirSom()`.
* `Mamifero.java`: Subclasse que herda de Animal.
* `Lobo.java`: Subclasse que estende Mamifero.
* `Cachorro.java`: Subclasse que estende Lobo e concentra as lógicas de sobrecarga.
* `Principal13.java`: Ponto de entrada que simula os estímulos e testa as reações do objeto no console.

## 💻 Exemplo de Saída no Console

```text
Rosnar
Abanar
Ignorar
Rosnar e latir
Au!Au!Au!
Latir
Rosnar

```

## 📄 Licença

Este projeto está sob a licença MIT. Sinta-se livre para clonar, estudar e utilizar o código!

---

*Projeto desenvolvido por Roberto como parte do portfólio de estudos em Ciência da Computação e Engenharia de Software com Java.*

---

