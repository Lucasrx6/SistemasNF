# 📊 Sistema de Acompanhamento de Números NF

Um sistema web inteligente para acompanhar e prever a necessidade de solicitação de números de Nota Fiscal, evitando travamentos por falta de numeração.

## 🚀 Características

- **📱 Mobile-First**: Interface otimizada para smartphones
- **🧠 Previsão Inteligente**: Calcula automaticamente quando solicitar novos números
- **⚡ Atualização Rápida**: Interface simples para informar estoque atual
- **📈 Dashboard Visual**: Cards informativos com status em tempo real
- **💾 Dados Persistentes**: Armazenamento local automático
- **🎯 Alertas Inteligentes**: Sistema de cores para indicar urgência

## 🛠️ Tecnologias

- **HTML5** - Estrutura semântica
- **CSS3** - Estilização responsiva
- **JavaScript ES6+** - Lógica da aplicação
- **Bootstrap 5.3** - Framework CSS e ícones
- **LocalStorage** - Persistência de dados

## 📦 Instalação

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/sistema-nf-tracking.git
```

2. Abra o arquivo `index.html` em seu navegador ou utilize um servidor web local:
```bash
# Usando Python
python -m http.server 8000

# Usando Node.js
npx http-server
```

3. Acesse `http://localhost:8000` no seu navegador

## 🎯 Como Usar

### 1. Primeiro Acesso
- O sistema já vem com dados de exemplo para demonstração
- Registre seus pedidos reais em **"Gerenciar Pedidos"**

### 2. Atualização Diária
- Use o campo **"Atualização Rápida"** para informar quantos números restam
- O sistema calculará automaticamente o consumo médio

### 3. Monitoramento
- Acompanhe os cards do dashboard:
  - **Números Disponíveis**: Estoque atual
  - **Próximo Pedido**: Data prevista para solicitar
  - **Uso Médio/Dia**: Consumo calculado automaticamente

### 4. Alertas
- 🟢 **Verde**: Situação normal
- 🟡 **Amarelo**: Atenção - estoque baixo
- 🔴 **Vermelho**: Crítico - solicitar urgentemente

## 📋 Funcionalidades Detalhadas

### Dashboard Inteligente
- Visualização em tempo real do status dos números NF
- Cálculos automáticos baseados no histórico de uso
- Previsão da próxima data ideal para pedido

### Cálculo de Consumo
```javascript
// Exemplo de cálculo
Último pedido: 25/07/2025 - 2000 números
Estoque atual: 623 números
Números utilizados: 2000 - 623 = 1377
Dias decorridos: ~27 dias
Média diária: 1377 ÷ 27 = 51 números/dia
```

### Sistema de Previsão
- Considera o consumo médio diário
- Leva em conta o prazo de entrega (padrão: 3 dias)
- Calcula com base no estoque mínimo de segurança
- Sugere a data ideal para fazer o pedido

### Configurações Ajustáveis
- **Prazo de Entrega**: Tempo que a empresa leva para fornecer
- **Estoque Mínimo**: Quantidade de segurança antes do pedido
- **Google Sheets**: Campo preparado para integração futura

## 📊 Exemplo de Uso Real

**Cenário**: 
- Último pedido: 25/07/2025 (2000 números)
- Data atual: 21/08/2025
- Estoque informado: 623 números

**Cálculo Automático**:
- Números utilizados: 1377 em 27 dias
- Média: 51 números/dia
- Com estoque mínimo de 500: pedido recomendado em ~2 dias

## 🔧 Configurações

### Ajustes Básicos
- **Prazo de Entrega**: 1-30 dias (padrão: 3 dias)
- **Estoque Mínimo**: Quantidade para alerta (padrão: 500)

### Backup e Restauração
- Use o botão flutuante 📥 para baixar backup em JSON
- Dados salvos automaticamente no navegador

## 🚧 Roadmap

- [ ] Integração com Google Sheets para automação
- [ ] Notificações push para alertas
- [ ] Relatórios em PDF
- [ ] API para integração com sistemas ERP
- [ ] Dashboard para múltiplas empresas
- [ ] Histórico de consumo por período

## 🤝 Contribuindo

1. Faça um Fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📄 Estrutura do Projeto

```
sistema-nf-tracking/
├── index.html          # Arquivo principal
├── README.md          # Este arquivo
└── assets/
    └── screenshots/   # Capturas de tela (opcional)
```

## 📱 Screenshots

### Dashboard Principal
*Interface responsiva com cards informativos*

### Atualização Rápida
*Campo para informar estoque atual*

### Histórico de Pedidos
*Gestão completa de pedidos anteriores*

## ⚠️ Requisitos do Sistema

- **Navegador moderno** com suporte a ES6+ e LocalStorage
- **Conexão com internet** para carregar Bootstrap e ícones
- **JavaScript habilitado**

## 🐛 Problemas Conhecidos

- LocalStorage tem limite de ~5-10MB por domínio
- Dados são perdidos se o usuário limpar o cache do navegador
- *Recomendação*: Fazer backup regular dos dados

## 📧 Suporte

Para dúvidas, sugestões ou problemas:
- Abra uma [Issue](https://github.com/seu-usuario/sistema-nf-tracking/issues)
- Entre em contato: [seu-email@exemplo.com]

## 📜 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

**Desenvolvido com ❤️ para otimizar o controle de números de NF e evitar travamentos operacionais.**

## 🏷️ Tags

`nota-fiscal` `sistema-web` `javascript` `bootstrap` `controle-estoque` `previsao` `mobile-first` `dashboard`
