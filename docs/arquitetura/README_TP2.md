# TP2 – Arquitetura da Solução – Loja Virtual

## (i) Escolhas de Tecnologias

| Camada / Propósito | Tecnologia / Ferramenta | Justificativa |
|--------------------|--------------------------|----------------|
| Linguagem | C / C++ / (ou a que você usou no TP1) | Foi escolhida no TP1, o sistema já foi parcialmente implementado com essa linguagem |
| Banco de dados | SQLite / arquivo local / JSON / alguma solução leve | Simples de configurar, ideal para aplicação pequena |
| Interface | Interface de console / GUI simples (dependendo do TP1) | Interação direta com o usuário final |
| Modelagem / Diagramas | diagrams.net / draw.io / Structurizr | Ferramentas visuais fáceis e que geram exportáveis (.png, .svg) |
| Versionamento / Integração | Git + GitHub | Controle de versão, colaboração e visibilidade do projeto |

---

## (ii) Modelo Arquitetural – C4

### Nível 1 – Diagrama de Contexto

Descreve como o **usuário** interage com o sistema de loja virtual e com o banco de dados.  

![Diagrama de Contexto](arquitetura/contexto.png)

### Nível 2 – Diagrama de Containers

Mostra os módulos principais como:

- Frontend / interface (console ou GUI)  
- Lógica de domínio / serviço  
- Persistência de dados / banco de dados  

![Diagrama de Containers](arquitetura/containers.png)

### Nível 3 – Diagrama de Componentes

Dentro de cada módulo / container, exemplifica componentes como:

- Módulo de produtos (cadastro, listagem)  
- Módulo de carrinho (adicionar, remover, calcular total)  
- Módulo de pagamento / finalização  
- Componente de persistência / DAO / repositório  

![Diagrama de Componentes](arquitetura/componentes.png)

---

## (iii) Justificativa do Modelo

- A separação em **containers e componentes** facilita a manutenção e a escalabilidade, mesmo que o sistema seja simples.  
- Ao usar C4, é possível “descer o zoom” da visão geral até os detalhes, permitindo que quem for avaliar compreenda desde o panorama até a estrutura interna.  
- A escolha de tecnologias mais leves (banco embutido, interface simples) é coerente com o escopo de projeto acadêmico e minimiza sobrecarga de configuração.  
- O modelo modular (produto, carrinho, persistência) deixa claro onde cada responsabilidade está, evita acoplamentos desnecessários e facilita evolução futura.

---

## (iv) Planejamento para o TP3 – Tarefas e Issues

A seguir, as tarefas previstas para o próximo sprint (TP3):

- Implementar estrutura base do código (pastas, arquivos iniciais)  
- Criar módulo de produtos (cadastro, listagem)  
- Criar módulo de carrinho (adicionar, remover, mostrar itens)  
- Implementar persistência de dados (gravação / leitura)  
- Finalizar fluxo de compra (simulação de pagamento)  
- Escrever testes (unitários / integração)  
- Documentar cada módulo (README interno)  

Essas tarefas foram criadas como issues no GitHub e adicionadas ao **Project Board TP3**.

---

