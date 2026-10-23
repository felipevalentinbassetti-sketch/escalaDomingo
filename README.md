# 📅 Painel de Gestão de Escala de Domingos

Sistema web responsivo e em tempo real desenvolvido para acompanhamento, gestão e compensação de escalas de trabalho aos domingos entre **Felipe** e **Luana**.

O objetivo principal da aplicação é fornecer **transparência, previsibilidade e sincronização instantânea** dos dias de trabalho e folga, aplicando automaticamente as regras de compensação por coberturas passadas ou futuras.

---

## 🚀 Funcionalidades Principais

* **🔄 Sincronização em Tempo Real (Firebase Firestore):** Todas as alterações de escala ou trocas registradas por um usuário são refletidas instantaneamente em todos os dispositivos conectados ao link compartilhável.
* **⚡ Regra Automática de Compensação:** Ao registrar uma cobertura (ex: quando um irmão cobre o outro em um evento/hackathon), o sistema recalcula e aplica automaticamente o turno no dia atual e no subsequente para fins de justa compensação.
* **📊 Painel de Métricas e Resumos:** Cards informativos no topo indicam o próximo responsável, total de turnos acumulados no período e o status atual das trocas ativas.
* **🔍 Filtros Dinâmicos:** Permite filtrar a visualização por responsável (*Apenas Felipe* / *Apenas Luana*) e por tipo de evento (*Escala Regular* / *Cobertura*).
* **📱 Design Limpo e Responsivo:** Desenvolvido com uma interface moderna estilo *dashboard* corporativo, otimizada para computadores e smartphones.

---

## 🛠️ Tecnologias Utilizadas

* **HTML5 & JavaScript (ES6+):** Estrutura do documento e lógica de recalculagem de turnos.
* **Tailwind CSS:** Framework utilitário de CSS para estilização ágil e responsiva.
* **Lucide Icons:** Biblioteca de ícones vetoriais leves para sinalização visual.
* **Firebase Firestore & Auth:** Banco de dados NoSQL em tempo real e autenticação anônima para persistência na nuvem sem necessidade de login complexo.

---

## 📅 Regra de Negócio e Escala

1. **Revezamento Padrão (1x1):** Em condições normais, o revezamento é intercalado (um domingo para Felipe, um domingo para Luana).
2. **Regra de Cobertura (2 Domingos Seguidos):** Quando o Responsável $A$ necessita de cobertura no seu domingo:
   * O Responsável $B$ assume o turno.
   * Como compensação justa, o Responsável $B$ assume também o domingo seguinte, cumprindo 2 domingos consecutivos.
   * A escala regular é retomada normalmente após o cumprimento da compensação.

---

## 📦 Como Executar e Hospedar

### Execução Local
1. Clone este repositório ou baixe o arquivo `index.html`.
2. Abra o arquivo `index.html` em qualquer navegador web moderno.
3. A aplicação se conectará automaticamente ao banco de dados e exibirá o cronograma atualizado.

### Hospedagem Gratuita (GitHub Pages)
1. Faça o upload do código para o seu repositório no GitHub.
2. Acesse **Settings** > **Pages** no repositório.
3. Em *Source*, selecione a branch `main` (ou `master`) e salve.
4. Compartilhe o link gerado pelo GitHub Pages para acesso dinâmico de qualquer lugar.

---

## 📄 Licença

Este projeto é de uso privado e de livre adaptação para gestão familiar de turnos e escalas.
