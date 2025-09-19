# SVM_grupo1_odor
Trabalho em python com SVM sobre um tema de detectar cogumelo venenoso por odor

**Instruções:**
---

Contexto – Dataset S1 (Odor → Toxicidade)
O dataset Mushroom é um clássico em aprendizado de máquina. Ele descreve características morfológicas e ambientais de cogumelos, indicando se são comestíveis (e) ou venenosos (p). Entre os diversos atributos disponíveis (como formato do chapéu, cor, habitat e tipo de lamela), um dos mais marcantes é o odor.
 
Na natureza, o odor é um dos principais sinais de alerta na diferenciação de espécies de fungos. Alguns odores são inconfundivelmente associados à toxicidade (por exemplo, cheiro pungente ou fétido), enquanto outros odores podem estar presentes apenas em espécies seguras para consumo (como anisado ou amendoado).
 
No subconjunto S1 – Odor, cada cogumelo é descrito apenas pelo seu odor característico, que foi transformado em variáveis binárias (One-Hot Encoding). Assim, cada linha do dataset representa um cogumelo, com uma única coluna “ativa” indicando seu odor, e a coluna class informando se é comestível ou venenoso.
 
**A questão que guia este cenário é:**
---
➡ Será que o odor, isoladamente, é suficiente para prever se um cogumelo é venenoso ou comestível?

**Resposta:** Não, a máquina ainda vai cometer erros com apenas odor. É nada garantido essa informações, pois a ainda muitos mais outros critérios a ser analisados para poder ter uma resposta satisfatória, afinal todo cuidado é pouco, quando se trata de ingerir um alimento perigoso.
 
O grupo deverá aplicar um classificador SVM (Support Vector Machine) nesse dataset para responder a essa pergunta, avaliando métricas como acurácia e matriz de confusão para a classe venenosa. O objetivo é entender até que ponto uma única característica sensorial pode sustentar uma decisão crítica de classificação.
 
O grupo deve usar: GridSearchCV para buscar os melhores hiper-parâmetros (kernel, c e gamma), além de cross-validation.
