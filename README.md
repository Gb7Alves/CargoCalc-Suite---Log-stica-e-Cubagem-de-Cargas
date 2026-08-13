# CargoCalc Suite - Logística e Cubagem de Cargas

Conjunto de ferramentas web de alta performance desenvolvido para otimizar operações logísticas de cálculo de cubagem, comparação de peso real versus peso cubado, cruzamento de notas fiscais (NDs) com AWBs via planilhas Excel e geração inteligente de dimensões.

---

## 🚀 Sobre os Projetos

Este repositório contém duas aplicações web independentes em arquivo único (`Single File Component`), focadas em usabilidade mobile (*mobile-first*), agilidade em galpão e robustez operacional:

### 1. Sistema de Cubagem e Relatórios (`cubagem-app-portfolio.html`)
* **Lançamento Manual de Volumes**: Cálculo instantâneo de metro cúbico ($m^3$), peso cubado com base em múltiplos fatores de conversão (ex: 167 $kg/m^3$ para aéreo) e comparação automática com o peso real.
* **Consulta e Relatórios via Planilha (SheetJS)**: Importação de planilhas Excel contendo o de/para de AWBs e NDs. O operador pesquisa o AWB e o sistema lista todas as notas vinculadas, indicando visualmente quais já possuem cubagem lançada e quais estão pendentes.
* **Trava de Segurança e Compartilhamento**: Validação inteligente que impede o compartilhamento do relatório caso existam NDs sem cubagem, gerando um resumo formatado ideal para envio direto via WhatsApp.

### 2. Gerador Inteligente de Cubagens (`gerador-cubagens-portfolio.html`)
* **Engenharia Reversa de Medidas**: O operador informa o peso cubado desejado e a quantidade de volumes; o algoritmo gera automaticamente dimensões realistas (comprimento, largura e altura diferentes entre si, evitando formatos cúbicos) que batem exatamente o resultado exigido.
* **Comparativo Simultâneo de Fatores**: Exibe em tempo real o impacto do mesmo volume gerado em diferentes fatores de cubagem (100, 167, 200, 250, 300 $kg/m^3$).
* **Resumo Copiável**: Botão de cópia rápida formatado para compartilhamento instantâneo.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5 & CSS3**: Layout responsivo com design moderno escuro, paleta personalizada e tipografia otimizada (*Space Grotesk* e *IBM Plex Mono*).
* **JavaScript (ES6+)**: Lógica robusta de manipulação de dados, validação rigorosa de formulários e formatação monetária/logística.
* **SheetJS (xlsx)**: Processamento de arquivos Excel diretamente no navegador (*client-side*), sem necessidade de backend.

---

## ⚙️ Como Utilizar

Por serem aplicações em arquivo único (*zero-config*), você não precisa instalar dependências, servidores ou rodar comandos de build (`npm install`). 

1. Baixe os arquivos HTML deste repositório.
2. Dê um duplo clique em qualquer um deles (`cubagem-app-portfolio.html` ou `gerador-cubagens-portfolio.html`).
3. O aplicativo abrirá diretamente no seu navegador de preferência.

---

## 📄 Licença

Este projeto é distribuído sob a licença MIT. Sinta-se à vontade para estudar, modificar e utilizar em seus próprios portfólios ou operações.
