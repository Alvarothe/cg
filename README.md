# Gerenciador de Conversas com Cronômetro e Copiador de CPF

## Descrição
Este userscript adiciona funcionalidades avançadas à plataforma de atendimento, incluindo:
- Cronômetro por conversa (70 segundos) que é ativado quando a conversa é selecionada
- Numeração dinâmica de conversas sempre visível no canto superior direito
- Checkmark verde em fundo preto quando o cronômetro atinge o limite
- Botão para extrair e copiar CPFs válidos encontrados na conversa
- Botão para copiar o nome do participante e a URL da interação

## Pré-requisitos
- [Tampermonkey](https://www.tampermonkey.net/) ou similar instalado no navegador

## Instalação
1. Abra o Tampermonkey no seu navegador
2. Clique no ícone de "+" para criar um novo script
3. Cole todo o código fornecido no editor
4. Clique em "File" > "Save"
5. Atualize a página da plataforma de atendimento

## Configuração
### Cronômetro e Numeração
As seguintes variáveis podem ser ajustadas no script:
```javascript
const limitTimeMs = 70 * 1000; // Tempo limite em milissegundos
const updateIntervalMs = 10;    // Intervalo de atualização´´´