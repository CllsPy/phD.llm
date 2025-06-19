# 1. Visão Geral

## Resumo
O `phd.llm`  é uma aplicação desenvovlida com o intuito de facilitar e impuslionar a pesquisa científica através do uso de LLMs capazes de encontrar lacunas em papers e encontrar quais outros trabalhos lidaram com ela, se houver solução.

## Problema
No doutorado é esperado que o doutorando seja capaz de analisar um extenso corpo de trabalhos e seguinda propor avanços em relação ao que foi escolhido. Esta tarefa demanda tempo, tempo que poderia estar sendo convertido na parte criativa, nos testes. O phd.llm surge como uma solução para esta problemática. A ferramenta será capaz de avaliar e compreender os trabalhos, extrair lacunas e apresentar quais ainda não foram resolvidas.

## Público Alvo
A plataforma destina-se, mas não somente, a aulas que estejam iniciando o seu doutorado e precisem de suporte na etapa de avaliação, na qual o estudante procura por lacunas a serem solucionadas em sua área de expertise.

## Tecnologia
O stack escolhido será o FARM, sobretudo em função da agilidade das aplicações construídas através do mesmo e do amplo suporte da comunidade em relação as ferramentas.

* **FastAPI** → API moderna e performática.
* **AI/LLM** → Gemini.
* **React** → Interface dinâmica para usuário.
* **MongoDB** → Armazenar histórico de buscas, papers analisados, feedback etc.

# 2. Objetivos do MVP
O MVP tem como objetivo garantir que a principalmente funcionalidade esteja disponível: Identificar lacunas em papers.

## Limitação
Uma limitação do MVP será a de que neste primeiro momento não será possível realizar múltiplas análsie simultaneamente.

## FRs
* Input do usuário (título ou DOI de paper)
* Busca do paper via arXiv / Semantic Scholar
* Extração de conteúdo (resumo, seções)
* Prompting para LLM identificar lacunas
* Busca de papers que abordam essas lacunas
* Exibir resultados ao usuário (resumo, links)
*  Armazenamento de histórico

## NFRs
* Baixa latência na resposta da API
* Alta disponibilidade do sistema
* Manutenibilidade do código
* Logs e rastreabilidade de requisições
* Segurança de API Keys e dados sensíveis

# 3.  Arquitetura do Sistema
![image](https://github.com/user-attachments/assets/69604811-1d21-4a45-abeb-6d0d983dfd1c)


