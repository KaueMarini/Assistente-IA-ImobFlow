# 🏢 Ecossistema IA Multi-Agentes para Imobiliárias

> Arquitetura de hiperautomação construída no **n8n** para atuar como um funil autônomo de vendas, atendimento multimodal e qualificação inteligente de leads imobiliários.

![Arquitetura do Fluxo n8n](./arquitetura-n8n.jfif)
*Visão geral da arquitetura de orquestração no n8n. O sistema é dividido entre o fluxo principal de roteamento cognitivo (acima) e os sub-agentes/microserviços especializados (abaixo).*

## 🚀 Visão Geral e Funcionalidades

Este projeto é um ecossistema de automação robusto que redefine a operação de uma agência imobiliária, transformando o atendimento e a qualificação de ponta a ponta. O sistema conta com:

* 📞 **Agente de Voz com LLM:** Um sistema que realiza ligações ativas para qualificação. Ele não apenas liga, mas mantém conversas 100% humanizadas onde tira dúvidas, recomenda imóveis com base no perfil do cliente e realiza agendamentos de visitas ou reuniões, tudo de forma autônoma.
* 🤖 **Sistema Multi-Agentes (Multimodal):** Nossos agentes são multimodais. Eles não se limitam a texto; entendem imagens e áudios enviados pelos clientes, e o mais importante: respondem a mensagens de áudio também com vozes humanas, tornando a interação incrivelmente natural.
* 📊 **Lead Scoring e Relatórios Semanais:** Ao fim de cada interação, o lead é automaticamente classificado. Toda semana, a diretoria recebe uma planilha detalhada com o resumo de todas as conversas e um "lead score" para cada cliente, facilitando a visualização de quem está mais engajado.
* 📈 **Agente de Follow-up:** Se um cliente para de responder, um agente de follow-up entra em ação, enviando mensagens periódicas para reengajar a interação e manter o funil aquecido.
* 🏡 **Agente de Negociação e Recomendação:** Um agente especialista que analisa o perfil completo do lead (orçamento, tipo, localização) e envia um portfólio com os imóveis que mais combinam com suas necessidades.

## 🛠️ Tecnologias e Infraestrutura

Para construir esse ecossistema e garantir uma comunicação estável e escalável em tempo real, integramos plataformas robustas:

* **Orquestrador Central:** n8n
* **Inteligência Artificial:** LLMs Generativos, Processamento de Linguagem Natural (NLP), Speech-to-Text (STT) e Text-to-Speech (TTS)
* **Comunicação e Mensageria:** Evolution API e Uzapi (integração direta com WhatsApp)
* **Gestão de Dados:** Integração nativa com CRMs e planilhas dinâmicas para relatórios.

## ⚙️ Como importar este fluxo

1. Faça o clone deste repositório ou baixe o arquivo `.json` do workflow.
2. No seu ambiente **n8n**, acesse a aba de Workflows.
3. No canto superior direito, selecione `Import from File...` e escolha o arquivo JSON.
4. **Nota de Segurança:** As credenciais (Chaves de API do LLM, Evolution API, bancos de dados) não são exportadas por padrão no n8n. Você precisará reconfigurar as suas próprias credenciais nos nós indicados antes de ativar o fluxo (`Set to Active`).

---
**Desenvolvido por [Kauê Nebot Marini](https://www.linkedin.com/in/kauemarini)** *AI & RPA Engineer*
