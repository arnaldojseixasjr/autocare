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
