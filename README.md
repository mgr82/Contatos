# Contatos
Esse é um projeto de extração de dados de contato de imagens 
# 📇 AI to vCard Generator

Uma ferramenta minimalista e offline-first projetada para converter blocos de texto `BEGIN:VCARD` gerados por Inteligências Artificiais (Gemini, ChatGPT, Claude) em arquivos `.vcf` reais que podem ser importados nativamente pelo Android (Samsung One UI) ou iOS.

## 🚀 O Problema
Ao solicitar que uma IA extraia dados de uma foto de cartão de visita, ela devolve o **texto** do código. No entanto, o Android não permite "Salvar como Contato" apenas copiando texto; ele precisa de um **arquivo físico** `.vcf`.

## 🛠 A Solução
Este "micro-app" serve como uma ponte:
1. Você cola o texto gerado pela IA.
2. O script gera um arquivo `.vcf` temporário no navegador.
3. O download inicia automaticamente, acionando o aplicativo de Contatos do smartphone.

## ✨ Funcionalidades
- **Processamento 100% Local:** Nenhum dado é enviado para servidores externos; tudo roda no navegador do seu dispositivo.
- **Detecção de Nome:** O nome do arquivo é gerado automaticamente baseado no campo `FN:` do vCard.
- **Leve e Rápido:** Um único arquivo HTML com menos de 2KB.
- **Dark Mode:** Interface otimizada para economia de bateria em telas OLED.

## 📱 Como usar (Instalação Rápida)

### Opção 1: Via GitHub Pages (Recomendado)
1. Faça o fork ou copie este repositório.
2. Vá em **Settings** > **Pages**.
3. Em "Branch", selecione `main` e salve.
4. Acesse o link gerado no seu celular.
5. No navegador do celular (Chrome/Samsung Internet), toque no menu e selecione **"Adicionar à Tela Inicial"** para usar como um app nativo.

### Opção 2: Uso Local
1. Baixe o arquivo `index.html`.
2. Salve na memória interna do seu celular.
3. Abra com qualquer navegador.

## 🤖 Exemplo de Workflow com IA
**Prompt no Gemini/GPT:**
> "Extraia os dados desta imagem e formate como um bloco de código vCard 3.0"

**No App:**
1. Copie o código gerado.
2. Cole na área de texto desta ferramenta.
3. Clique em **SALVAR CONTATO**.
4. O celular perguntará: *"Deseja importar para os Contatos?"* -> **Sim**.

## 📝 Licença
MIT License - Sinta-se livre para modificar e melhorar.
