

# 🦅 Liskov Substitution Principle (LSP) 
![image](https://github.com/user-attachments/assets/a3020154-b1cd-4eb1-a106-cf5231fc8ddf)

## O que é o LSP?

O **Princípio da Substituição de Liskov (LSP)** diz que **subclasses devem poder substituir suas classes base** sem alterar o comportamento do sistema. 🔄 Em termos simples, se você pode substituir uma classe base por uma subclasse sem quebrar nada, você está seguindo o LSP. 🛡️

### 🚨 Problema comum:

Vamos imaginar uma classe `Bird` 🐦 que tem um método `Fly()`. Isso faz sentido para pássaros que voam, mas se criarmos uma subclasse `Penguin` 🐧, percebemos que pinguins não voam! Isso quebra o comportamento esperado. Se substituirmos `Bird` por `Penguin`, o sistema pode falhar. 💥

### ✅ Solução com LSP:

Para corrigir isso, devemos garantir que as subclasses respeitem o comportamento da classe base, ou então não herdar dela. Criamos uma hierarquia que faz sentido, onde somente aves que podem voar têm o método `Fly()`. 🦅

### 🛠️ Explicação do Projeto:

No projeto que implementa o LSP:
- A classe base `Bird` 🐦 define comportamentos comuns (como "andar" ou "nadar").
- Subclasses como `FlyingBird` 🦅 implementam a habilidade de voar.
- A classe `Penguin` 🐧 implementa comportamentos que fazem sentido para ela, como "andar" ou "nadar", sem herdar a habilidade de voar.

#### 🎯 Benefícios:
- **Previsibilidade**: Garantimos que as subclasses substituem corretamente a classe base, evitando surpresas. 🎉
- **Polimorfismo seguro**: O uso de herança 🧬 e polimorfismo se torna mais seguro e intuitivo, evitando bugs inesperados no sistema. 🛡️
 ## Estrutura do Projeto
  ![image](https://github.com/user-attachments/assets/31e86a19-81f7-4fa0-80f6-902725ec3b83)

