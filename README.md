# Assistente de Voz com OpenRouter (Colab)

Assistente de voz simples que grava áudio pelo navegador, transcreve com Whisper, gera resposta com modelos via OpenRouter e converte o retorno em fala usando gTTS.

---

## Arquitetura

Fluxo do pipeline:

1. Captura de áudio no navegador (MediaRecorder + visualizador waveform)
2. Conversão e transcrição com Whisper
3. Geração de resposta via API OpenRouter
4. Síntese de voz (TTS) com gTTS
5. Reprodução do áudio no notebook

---

## Tecnologias

* Python 3 (Google Colab)
* Whisper (Speech-to-Text)
* OpenRouter API (LLM)
* gTTS (Text-to-Speech)
* JavaScript MediaRecorder (captura de áudio)

---

## Pré-requisitos

* Conta no OpenRouter
* API Key válida
* Navegador com permissão de microfone

---

## Como executar no Colab

1. Abra o notebook `assistente_de_voz.ipynb`
2. Insira sua API KEY na célula de configuração:

```python
OPENROUTER_API_KEY = "SUA_CHAVE"
```

3. Execute as células na ordem
4. Clique em **Permitir microfone**
5. Grave o áudio e pressione **Parar gravação**
6. Aguarde a transcrição e a resposta em voz

---

## Estrutura do Projeto

```
assistente-de-voz/
 ├─ assistente_de_voz.ipynb
 └─ README.md
```

---

## Possíveis melhorias

* Streaming de resposta
* Troca de TTS por voz neural
* Interface web (Gradio ou Streamlit)
* Histórico de conversas
* Deploy em backend

---

## Licença

Uso educacional e experimental.
