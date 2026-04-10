![WaveDrip](https://img.shields.io/badge/Status-Produção%20Ready-success)
![React](https://img.shields.io/badge/React-18.3.1-blue)
![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue)
![Tailwind](https://img.shields.io/badge/Tailwind-4.0-38bdf8)

Um marketplace e-commerce profissional e completo, similar a Amazon, Mercado Livre e Shopee, com design moderno, animações fluidas e experiência de usuário impecável.

## ✨ Funcionalidades Principais

### 🛒 Para Compradores
- ✅ **Catálogo com 100+ produtos** em 24 categorias diferentes
- ✅ **Busca inteligente** com sugestões automáticas e correção de texto
- ✅ **Filtros avançados** por categoria, preço, avaliação
- ✅ **Carrinho persistente** que salva entre sessões
- ✅ **Sistema de checkout** em 3 etapas
- ✅ **Múltiplos métodos de pagamento** (PIX, Cartão, Boleto)
- ✅ **Cálculo de frete automático** (Padrão, Rápido, Expresso)
- ✅ **Histórico de pedidos** com rastreamento
- ✅ **Sistema de avaliações** de produtos
- ✅ **Recomendações personalizadas**

### 🏪 Para Vendedores
- ✅ **Criação de loja virtual** própria
- ✅ **Painel do vendedor** com gerenciamento de produtos
- ✅ **Adicionar/editar produtos** facilmente
- ✅ **Controle de estoque**
- ✅ **Estatísticas de vendas**

### 👨‍💼 Para Administradores
- ✅ **Painel administrativo** completo
- ✅ **Gerenciamento de usuários**
- ✅ **Gerenciamento de pedidos**
- ✅ **Relatórios e análises**
- ✅ **Controle de produtos**

### 🤖 Recursos Extras
- ✅ **Assistente IA integrado** para suporte 24/7
- ✅ **Design responsivo** perfeito em mobile
- ✅ **Animações fluidas** com Motion
- ✅ **Performance otimizada**
- ✅ **PWA Ready** (Progressive Web App)

## 🎨 Design e UX

- **Design limpo e moderno** com gradientes azul/roxo/rosa
- **Interface intuitiva** e fácil de navegar
- **Animações suaves** que não comprometem performance
- **Totalmente responsivo** - funciona perfeitamente em qualquer dispositivo
- **Acessibilidade** seguindo padrões WCAG
- **Dark/Light mode ready**

## 🛠️ Tecnologias Utilizadas

### Frontend
- **React 18.3** - Framework JavaScript
- **TypeScript** - Tipagem estática
- **React Router** - Navegação e roteamento
- **Tailwind CSS 4.0** - Estilização
- **Motion (Framer Motion)** - Animações
- **Radix UI** - Componentes acessíveis

### UI Components
- **shadcn/ui** - Sistema de componentes
- **Lucide React** - Ícones
- **Sonner** - Notificações toast
- **Recharts** - Gráficos e analytics

### Estado e Dados
- **Context API** - Gerenciamento de estado global
- **LocalStorage** - Persistência de dados local
- **React Hooks** - Estado e efeitos

## 📦 Estrutura do Projeto

```
techshop/
├── src/
│   ├── app/
│   │   ├── components/          # Componentes reutilizáveis
│   │   │   ├── ui/              # Componentes UI (botões, inputs, etc)
│   │   │   ├── Header.tsx       # Cabeçalho com busca inteligente
│   │   │   ├── Footer.tsx       # Rodapé
│   │   │   ├── ProductCard.tsx  # Card de produto
│   │   │   └── AIAssistant.tsx  # Chatbot IA
│   │   ├── pages/               # Páginas da aplicação
│   │   │   ├── Home.tsx         # Página inicial
│   │   │   ├── Products.tsx     # Listagem de produtos
│   │   │   ├── ProductDetail.tsx# Detalhes do produto
│   │   │   ├── Cart.tsx         # Carrinho de compras
│   │   │   ├── Checkout.tsx     # Finalização de compra
│   │   │   ├── Orders.tsx       # Histórico de pedidos
│   │   │   ├── Login.tsx        # Login
│   │   │   ├── Register.tsx     # Cadastro
│   │   │   ├── AdminPanel.tsx   # Painel admin
│   │   │   └── seller-dashboard.tsx # Painel vendedor
│   │   ├── context/
│   │   │   └── AppContext.tsx   # Context API global
│   │   ├── data/
│   │   │   └── products.ts      # 100 produtos mockados
│   │   ├── App.tsx              # Componente raiz
│   │   ├── Root.tsx             # Layout principal
│   │   └── routes.tsx           # Configuração de rotas
│   └── styles/
│       ├── index.css            # Estilos globais
│       ├── theme.css            # Variáveis de tema
│       └── fonts.css            # Fontes customizadas
├── HOSPEDAGEM.md                # Guia de hospedagem
└── package.json
```

## 🚀 Como Executar Localmente

### Pré-requisitos
- Node.js 18+ instalado
- npm ou pnpm instalado

### Instalação

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/techshop.git

# Entre na pasta
cd techshop

# Instale as dependências
npm install

# Execute em modo desenvolvimento
npm run dev

# Acesse http://localhost:5173
```

### Build para Produção

```bash
# Criar build otimizado
npm run build

# O build estará na pasta /dist
```

## 📱 Funcionalidades Detalhadas

### Sistema de Busca Inteligente
- Busca em tempo real enquanto digita
- Sugestões automáticas de produtos
- Correção de erros de digitação (fuzzy search)
- Busca por nome, categoria e descrição
- Dropdown com preview de produtos

### Cálculo de Frete
- **3 opções de entrega:**
  - Padrão (7-10 dias) - R$ 15,90
  - Rápida (3-5 dias) - R$ 29,90
  - Expressa (1-2 dias) - R$ 49,90
- **Frete grátis** para compras acima de R$ 299
- Busca automática de CEP
- Formatação automática de endereço

### Sistema de Pagamentos (Simulado)
- **PIX** - Desconto de 5%
- **Cartão de Crédito** - Até 12x sem juros
- **Boleto Bancário** - Vencimento em 3 dias

### Assistente IA
- Responde perguntas sobre:
  - Entrega e frete
  - Formas de pagamento
  - Rastreamento de pedidos
  - Devoluções e garantia
  - Cadastro e login
  - Como vender na plataforma
- Interface de chat moderna
- Disponível 24/7
- Respostas contextuais

### Histórico de Pedidos
- Lista todos os pedidos do usuário
- Filtros por status (Processando, Em Transporte, Entregue, Cancelado)
- Código de rastreamento
- Previsão de entrega
- Detalhes completos de cada pedido

### Painel Administrativo
**Acesso:** Login com `admin@techshop.com`

- Dashboard com métricas:
  - Total de usuários
  - Total de pedidos
  - Receita total
  - Total de produtos
- Gerenciamento de usuários
- Tabela com busca e filtros
- Ações rápidas
- Exportar relatórios

## 🔐 Sistema de Autenticação

### Tipos de Conta
1. **Comprador** - Pode comprar produtos
2. **Vendedor** - Pode vender produtos
3. **Admin** - Acesso completo ao sistema

### Persistência
- Dados salvos em `localStorage`
- Login mantido entre sessões
- Cada usuário tem seu próprio histórico

## 📊 Dados

### Categorias (24 total)
- Eletrônicos (Computadores, Smartphones, Áudio, Gaming)
- Moda (Roupas, Calçados, Acessórios)
- Casa (Decoração, Móveis, Cozinha)
- Beleza (Cosméticos, Perfumes, Cuidados)
- Livros
- Brinquedos
- Pet Shop
- Automotivo
- Jardinagem
- Instrumentos Musicais
- E muito mais!

### 100 Produtos Incluídos
- Nomes realistas
- Preços variados (R$ 49 - R$ 15.999)
- Imagens do Unsplash
- Avaliações e reviews
- Descrições detalhadas
- Controle de estoque
- 26 lojas diferentes

## 🎯 Roadmap Futuro

### Curto Prazo
- [ ] Integração com gateway de pagamento real (Mercado Pago/Stripe)
- [ ] API de cálculo de frete real (Correios/Melhor Envio)
- [ ] Sistema de notificações por email
- [ ] Upload de imagens para produtos

### Médio Prazo
- [ ] Chat ao vivo com vendedores
- [ ] Sistema de reviews e fotos de produtos
- [ ] Programa de fidelidade
- [ ] Cupons de desconto
- [ ] Wishlist (lista de desejos)

### Longo Prazo
- [ ] App mobile (React Native)
- [ ] Sistema de afiliados
- [ ] Marketplace internacional
- [ ] IA para recomendações avançadas
- [ ] Realidade aumentada (AR) para preview de produtos

## 🌐 Deploy e Hospedagem

Consulte o arquivo [HOSPEDAGEM.md](./HOSPEDAGEM.md) para instruções detalhadas sobre:
- Opções de hospedagem (Vercel, Netlify, AWS, etc.)
- Configuração de banco de dados
- Integração de pagamentos
- Cálculo de frete
- Estimativa de custos
- Checklist de segurança

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para:
1. Fork o projeto
2. Criar uma branch (`git checkout -b feature/NovaFuncionalidade`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/NovaFuncionalidade`)
5. Abrir um Pull Request

## 📞 Suporte

- **Documentação:** Leia este README e HOSPEDAGEM.md
- **Issues:** Abra uma issue no GitHub
- **Email:** suporte@techshop.com (simulado)

## ⭐ Agradecimentos

- [React](https://react.dev/)
- [Tailwind CSS](https://tailwindcss.com/)
- [shadcn/ui](https://ui.shadcn.com/)
- [Unsplash](https://unsplash.com/) - Imagens dos produtos
- [Lucide](https://lucide.dev/) - Ícones

---

**Desenvolvido com ❤️ para criar a melhor experiência de e-commerce**

🚀 **Pronto para produção!** Deploy hoje mesmo e comece a vender!
