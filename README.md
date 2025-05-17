# Obra.IA_Alura

## Visão Geral

Obra.IA é um sistema inteligente projetado para auxiliar pedreiros e profissionais da construção civil na criação de orçamentos detalhados e precisos para diversos tipos de obras. Utilizando uma arquitetura baseada em agentes de inteligência artificial, o sistema automatiza o processo de identificação de materiais, mão de obra e a busca por preços atualizados, fornecendo uma estimativa de custo completa e revisada.

## Funcionalidades Principais

* **Planejamento Inteligente de Orçamentos:** Analisa o tipo e a área da obra para determinar os materiais e a mão de obra necessários.
* **Busca Automatizada de Preços:** Utiliza ferramentas de busca online para encontrar preços de materiais de construção e taxas de mão de obra, considerando a localização da obra (quando fornecida).
* **Geração Detalhada de Orçamentos:** Calcula os custos totais de materiais e mão de obra, apresentando um orçamento claro e organizado.
* **Revisão Inteligente de Orçamentos:** Analisa o orçamento gerado, verificando a razoabilidade dos preços e identificando possíveis omissões ou áreas de melhoria.
* **Flexibilidade de Localização:** Adapta as buscas de preço à localização da obra para orçamentos mais precisos.
* **Interface de Usuário Simples:** Permite ao usuário inserir facilmente as informações da obra (tipo, área e localização).

## Arquitetura do Sistema

O Obra.IA é composto por quatro agentes de inteligência artificial que trabalham em colaboração:

1.  **Agente Buscador de Obra:** Responsável por buscar informações relevantes para a obra na internet, como preços de materiais e taxas de mão de obra, utilizando a ferramenta de busca do Google.
2.  **Agente Planejador de Orçamentos:** Analisa o tipo e a área da obra para determinar os materiais de construção e os tipos de mão de obra necessários, formulando consultas de busca para o Agente Buscador.
3.  **Agente Redator de Orçamentos:** Utiliza o plano de orçamento e os resultados da busca para calcular os custos e formatar um orçamento detalhado.
4.  **Agente Revisor de Orçamentos:** Analisa o orçamento gerado, verificando a razoabilidade dos preços e a completude das informações.

## Como Utilizar

1.  Execute o script principal do Obra.IA.
2.  O sistema solicitará o tipo de obra (ex: "parede de alvenaria", "aplicação de reboco").
3.  Em seguida, será pedida a área da obra em metros quadrados (m²).
4.  Opcionalmente, você pode fornecer a localização da obra (cidade, estado) para refinar a busca de preços.
5.  O sistema iniciará o processo de planejamento, busca, redação e revisão do orçamento, exibindo os resultados de cada agente.
6.  Ao final, um orçamento detalhado será apresentado.

## Requisitos

* Python 3.x
* Biblioteca `google-generativeai` (Google AI Python SDK)
* Acesso à API da Google GenAI (configuração de chave de API necessária)
* Biblioteca `google-adk` (Google Assistant Development Kit - pode ter dependências específicas de instalação, verificar a documentação)
* Biblioteca `IPython` (para visualização formatada em ambientes como Colab ou Jupyter)
* Biblioteca `datetime` (para manipulação de datas)
* Biblioteca `json` (para trabalhar com formato JSON)

## Instalação

1.  **Instale o Python:** Certifique-se de ter o Python 3.x instalado em seu sistema.
2.  **Instale as bibliotecas necessárias:**
    ```bash
    pip install google-generativeai google-adk IPython
    ```
3.  **Configure a chave da API da Google GenAI:** Siga as instruções da documentação da Google AI Python SDK para obter e configurar sua chave de API.
4.  **Verifique a instalação do Google ADK:** A instalação e configuração do Google ADK podem ter etapas adicionais dependendo do seu ambiente. Consulte a documentação do ADK para garantir que esteja configurado corretamente.

## Próximos Passos e Melhorias Futuras

* **Implementação completa da busca de preços em tempo real:** Integrar o Agente Buscador para obter dados de preço diretamente da internet com base nas consultas do Planejador.
* **Extração inteligente de preços:** Desenvolver mecanismos para extrair preços relevantes dos resultados da busca de forma confiável.
* **Cálculo automático de quantidades de materiais:** Estimar as quantidades de materiais necessários com base no tipo e área da obra.
* **Interface gráfica de usuário (GUI):** Criar uma interface mais amigável para interação com o sistema.
* **Persistência de dados:** Salvar orçamentos gerados e informações de obras.
* **Integração com catálogos de materiais:** Utilizar bancos de dados de materiais de construção para informações mais precisas.
* **Consideração de normas técnicas:** Incorporar informações de normas (como ABNT) nos orçamentos.
* **Cálculo de BDI (Benefícios e Despesas Indiretas):** Adicionar a opção de incluir o BDI no orçamento.

## Contribuição

Contribuições para o projeto são bem-vindas! Se você tiver ideias de melhorias, correções de bugs ou novas funcionalidades, sinta-se à vontade para abrir um pull request.

## Licença

[MIT License]

## Autor

[Luana Silva]
