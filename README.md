# Projeto-An-lise-e-Projeto-de-Sistemas-II

# Connectivity Forecast API

Reimplementação Java/Spring Boot da [API de referência](https://github.com/LiniiS/connectivity-forecast-api), usada como artefato educacional de APS II.

## Executar

Requisitos: Java 17 e Maven 3.9+

```bash
mvn test
mvn spring-boot:run
```

Swagger UI: `http://localhost:8080/swagger-ui.html`  
OpenAPI: `http://localhost:8080/v3/api-docs`

## Escopo

Limitações e escopo educacional API

Este projeto é uma reimplementação educacional da Connectivity Forecast API de referência, desenvolvida para fins de estudo na disciplina APS II.

O que está disponível:

API REST local, organizada por recursos e versionada em /api/v1.
Catálogo de modelos, incluindo modelos ativos e inativos.
Dados fictícios para testes e demonstrações, com 4 modelos ativos, 10 probes e 24 instantes de previsão, totalizando 960 previsões na fixture descrita.
Documentação OpenAPI e interface Swagger UI.

O que não está implementado:

Integração com a rede RIPE Atlas ou coleta de medições reais.
Treinamento, execução ou avaliação de modelos de previsão.
Persistência em banco de dados.
Implantação em ambiente de produção.

As previsões são mockadas e os resultados dependem dos dados de exemplo fornecidos pela aplicação. A classificação e as recomendações utilizam regras experimentais, sem validação científica. Portanto, os resultados não devem ser interpretados como previsões reais de conectividade nem como garantias de desempenho.

O projeto destina-se ao aprendizado, à experimentação e à demonstração de conceitos de desenvolvimento de APIs. Uma evolução futura poderá incluir dados reais, persistência, validação das regras e testes de qualidade preditiva.

## Estrutura

Separação em controllers, services, repositories, modelos de domínio/DTOs e configuração. API versionada em `/api/v1`, com recursos de health, modelos, localizações, previsões e atividades.

## Documentação

README e OpenAPI são pontos de partida. Completar em exercício: descrição dos endpoints, parâmetros e validações, exemplos de requisição/resposta, códigos de erro e origem dos campos. Referência à licença MIT da API de origem preservada neste projeto.

A API utiliza dados estáticos de exemplo e não representa previsões reais em tempo real.
