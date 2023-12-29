# Projeto: Dashboard

Você trabalha como analista de anúncios em vídeo na agência de publicidade Sterling & Draper. Você dedica muito tempo analisando vídeos de tendências no YouTube para determinar qual conteúdo merece atenção de marketing.
Cada vídeo tem uma categoria específica (entretenimento, música, notícias e política etc.), região e data de tendência. 

Um vídeo pode estar na seção de tendências por vários dias seguidos.

Toda semana, os novos funcionários Melanie e Ashok fazem as mesmas perguntas:
- Quais categorias de vídeo foram tendências na semana passada?
- Como foram distribuídos entre as várias regiões?
- Quais categorias foram especialmente populares nos Estados Unidos?

Depois de conversar com os gerentes e administradores de banco de dados, você elaborou breves requisitos técnicos:
- Objetivo dos negócios: analisar o histórico de vídeos de tendências no YouTube
- Com que frequência o dashboard será usado: pelo menos uma vez por dia
- Usuário do dashboard de destino: gerentes de planejamento de anúncios em vídeo
- Conteúdo de dados do dashboard:
    - Vídeos de tendências do passado, divididos por dia e categoria
    - Vídeos de tendências, divididos por países
    - Uma tabela de correspondência entre categorias e países
- Parâmetros segundo os quais os dados devem ser agrupados:
    - Data e hora da tendência
    - Categoria de vídeo
    - País
- Os dados:
    - Histórico de tendências — valores absolutos com divisão por dia (dois gráficos: números absolutos e proporção percentual)
    - Eventos, discriminados por países — valores relativos (% de eventos)
    - A correspondência entre as categorias e os países — valores absolutos (uma tabela)
- Importância: todos os gráficos são igualmente importantes
- Fontes de dados para o dashboard: os engenheiros de dados prometeram criar uma tabela agregada chamada trending_by_time. Segue sua estrutura:
    - `record_id` — chave primária
    - `region` — país / região geográfica
    - `trending_date` — data e hora
    - `category_title` — a categoria de vídeo
    - `videos_count` — o número de vídeos na seção de tendências
- A tabela fica armazenada no banco de dados do youtube , criado especialmente para suas necessidades
- Intervalo de atualização de dados: uma vez a cada 24 horas, à meia-noite UTC
- Gráficos, controles do dashboard e sua disposição:
