Gerenciador de Conversas com Cronômetro e Copiador de CPF
Descrição
Este userscript adiciona funcionalidades avançadas à plataforma de atendimento, incluindo:

Cronômetro por conversa: Cada conversa tem um cronômetro de 70 segundos que é ativado quando a conversa é selecionada e pausado quando não está ativa.
Numeração dinâmica: As conversas são numeradas dinamicamente, com o número sempre visível no canto superior direito.
Checkmark de conclusão: Quando o cronômetro atinge 70 segundos, um checkmark verde é exibido em fundo preto.
Copiador de CPF: Botão para extrair e copiar CPFs válidos encontrados na conversa (no painel de scripts ou nas mensagens).
Copiador de Interação: Botão para copiar o nome do participante e a URL da interação.
Instalação
Instale o Tampermonkey no seu navegador.
Crie um novo script no Tampermonkey e cole o código fornecido.
Atualize a URL de correspondência (@match) no script para corresponder à sua plataforma, se necessário.
Configuração
Cronômetro e Numeração
As seguintes variáveis podem ser ajustadas no script:

limitTimeMs: Tempo limite do cronômetro em milissegundos (padrão: 70 segundos).
updateIntervalMs: Intervalo de atualização do cronômetro em milissegundos (padrão: 10ms).
Cores e estilos para cronômetro em execução, pausado e concluído.
Copiador de CPF e Interação
O script procura por CPFs em dois locais: no painel de scripts e nas mensagens da conversa.
O botão de interação requer que o nome do participante na conversa selecionada corresponda ao nome do participante externo.
Uso
Cronômetro e Numeração
O cronômetro de cada conversa é exibido no centro à direita do card da conversa.
O número da conversa é exibido no canto superior direito do card.
Ao selecionar uma conversa, o cronômetro é ativado (se não estiver concluído).
Ao desmarcar, o cronômetro é pausado.
Copiador de CPF
Clique no botão com o ícone de documento (localizado na barra de ferramentas).
Se um CPF for encontrado, ele será copiado automaticamente.
Se múltiplos CPFs forem encontrados, um popup será exibido para seleção.
Copiador de Interação
Selecione a conversa desejada.
Clique no botão com o ícone de seta para baixo (localizado na barra de ferramentas).
O nome do participante e a URL da interação serão copiados no formato: Nome do Participante - URL.
Validação de CPF
O script utiliza uma função de validação de CPF que ignora CPFs inválidos conhecidos (como repetições de dígitos). Você pode ajustar a lista de CPFs inválidos na constante INVALID_DOCUMENTS.