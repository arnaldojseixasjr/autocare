# 🚗 AutoCare — Portal de Estética Automotiva Inteligente

> Aplicação web desenvolvida para modernizar o atendimento e a estimativa de orçamentos da AutoCare utilizando No-Code, padrões Web e Inteligência Artificial.

---

## 📌 1. Sobre o Projeto e Problema Negocial
A **AutoCare** é um centro de estética automotiva que sofria com gargalos no atendimento via WhatsApp. Os clientes demoravam a receber respostas sobre valores e tipos de serviços. 

**Solução:** Criação de um portal interativo onde o cliente consulta serviços, calcula o valor estimado do atendimento em tempo real e tira dúvidas 24/7 com um assistente virtual inteligente.

---

## 🛠️ 2. Tecnologias e Ferramentas Utilizadas
* **Plataforma No-Code:** Softr (estruturação da interface e layout responsivo)
* **Padrões Web (Código Customizado):** HTML5, CSS3 e JavaScript (ES6)
* **Inteligência Artificial:** Widget de Chatbot interativo simulado para atendimento dinâmico

---

## 💻 3. Personalizações com Padrões Web (HTML, CSS e JavaScript)
Para ir além dos componentes nativos da plataforma No-Code, foram injetados scripts personalizados via bloco *Custom Code*:

* **HTML/CSS:** Interface personalizada com tema escuro (*Dark Mode*), seletores de porte de veículo e caixa de mensagens estilizada.
* **JavaScript:** Função `calcularOrcamento()` que escuta a seleção do serviço e do porte do carro, processa o cálculo multiplicador e atualiza o valor na tela instantaneamente.

```javascript
// Exemplo do cálculo executado no Front-end
function calcularOrcamento() {
  let valorServico = parseFloat(document.getElementById('servico').value);
  let fatorPorte = parseFloat(document.getElementById('porte').value);
  let total = valorServico * fatorPorte;
  document.getElementById('resultado').innerText = "Total Estimado: R$ " + total.toFixed(2).replace('.', ',');
}

## 💻 4. Recurso Inteligente (IA / Automação)
Implementação de um assistente virtual na tela que reconhece intenções de busca do cliente (ex: perguntas sobre polimento ou vitrificação) e fornece orientações personalizadas sobre o melhor tratamento para o veículo

## 💻 5. Como Acessar e Testar a Solução
Link Público da Aplicação: [Acesse o Portal AutoCare no Ar](https://autocare.softr.app)

Instruções de Teste:
Acesse o link público no computador ou celular.
Selecione um serviço e o porte do veículo para ver o cálculo em JS funcionando.
Digite uma dúvida na caixa do Assistente Virtual (ex: "O que é polimento?")

## 💻 6. Evidências da Aplicação (Prints)
<img width="502" height="680" alt="Captura de tela 2026-09-16 183859" src="https://github.com/user-attachments/assets/78cf2587-8a7f-4781-88bf-79434f1e80b2" />

Autor
Nome do Aluno: Arnadlo de Jesus Seixas Junior
Curso/Disciplina: Padrões Web para No Code e Low Code — UniFECAF

