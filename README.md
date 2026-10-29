# 🎓 HubTech — Hub de Oportunidades & Curadoria em Tecnologia

<p align="center">
  <img src="./assets/hubtech_icon_transparent.png" width="120" alt="HubTech Logo" />
</p>

<p align="center">
  <strong>Plataforma colaborativa de descoberta, curadoria e orientação de oportunidades educacionais em tecnologia para estudantes universitários.</strong>
</p>

<p align="center">
  <a href="https://hub-tech.vercel.app/" target="_blank">
    <img src="https://img.shields.io/badge/Live_Demo-hub--tech.vercel.app-10B981?style=for-the-badge&logo=vercel&logoColor=white" alt="Live Demo" />
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS_4-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white" />
</p>

---

## 🌐 Acesso à Plataforma

O projeto está no ar e pode ser acessado diretamente pelo link:

👉 **[https://hub-tech.vercel.app/](https://hub-tech.vercel.app/)**

---

## 🎬 Demonstração

![Navegação e funcionalidades do HubTech](./assets/demo.gif)

*Navegação fluida entre a página inicial, catálogo de cursos com filtros dinâmicos e central de benefícios estudantis.*

---

## 📸 Telas da Plataforma

<table>
<tr>
<td width="50%">

**Página Inicial (Hero & Destaques)**

![Tela inicial do HubTech](./assets/tela-home.png)

</td>
<td width="50%">

**Explorar Cursos & Certificações**

![Catálogo com filtros por área](./assets/tela-explorar.png)

</td>
</tr>
<tr>
<td width="50%">

**Central de Benefícios Universitários**

![Benefícios e ferramentas para estudantes](./assets/tela-beneficios.png)

</td>
<td width="50%">

**Detalhes da Oportunidade & Modal**

![Modal com contexto e link oficial](./assets/tela-modal-detalhes.png)

</td>
</tr>
</table>

---

## 🎯 O problema que o projeto resolve

Quem ingressa em cursos de tecnologia (especialmente nos primeiros semestres) frequentemente enfrenta dois grandes obstáculos:

1. **Dispersão de conteúdo:** Existem centenas de cursos, certificações gratuitas de peso internacional (Cisco, IBM, Microsoft, etc.) e pacotes de benefícios para estudantes (GitHub Student Developer Pack, JetBrains, AWS Educate, Azure), mas essas informações estão espalhadas em dezenas de sites diferentes.
2. **Falta de contexto prático:** O estudante novato muitas vezes não sabe por onde começar, quais pré-requisitos precisa ter ou quais certificações realmente têm valor para o mercado e para validação de horas complementares.

O **HubTech** centraliza, filtra e organiza essas oportunidades em um único ambiente moderno, gratuito e colaborativo.

---

## 💡 Filosofia do HubTech

- **Curadoria, não competição:** O HubTech não concorre com plataformas como Cisco Networking Academy, Microsoft Learn ou TryHackMe. Ele atua como uma camada inteligente de curadoria e direcionamento, encaminhando o aluno sempre para o link e provedor oficial.
- **Liberdade de escolha:** Apresenta caminhos, fundamentos e trilhas como possibilidades para o estudante construir sua própria jornada, sem impor regras rígidas.
- **Espírito colaborativo:** Os próprios alunos podem submeter novas plataformas, cursos e benefícios que descobriram, alimentando a base para toda a comunidade.

---

## ⚙️ Principais Funcionalidades

- **Catálogo de Cursos & Certificações:** Filtros por área de atuação (Frontend, Backend, DevOps, Cyber, Dados, etc.), nível de dificuldade, carga horária e emissão de certificado gratuito.
- **Central de Benefícios Estudantis:** Lista curada de ferramentas profissionais gratuitas ou com desconto para quem possui e-mail universitário.
- **Modal de Detalhes Contextualizado:** Informações sobre requisitos, idioma, carga horária estimada e orientações de aproveitamento.
- **Sistema de Sugestão da Comunidade:** Formulário integrado para envio de novas oportunidades para revisão e aprovação.
- **SEO & Performance:** Metatags completas, dados estruturados Schema.org (JSON-LD), sitemap dinâmico e renderização veloz.

---

## 🛠️ Stack Tecnológica & Arquitetura

### Frontend
- **React 19:** Aproveitamento das APIs mais recentes do ecossistema React.
- **TypeScript:** Tipagem estática em 100% dos componentes e contratos de dados.
- **Vite:** Build tool de alta performance para desenvolvimento e bundle otimizado.
- **Tailwind CSS 4:** Estilização utilitária moderna com design tokens.
- **Motion (`motion`):** Transições suaves de página, drawers e modais.
- **Shaders React (`@paper-design/shaders-react`):** Renderização visual líquida/fluida no background para uma identidade estética dark e imersiva.
- **Lucide Icons:** Conjunto consistente de ícones vetoriais.

### Backend & Banco de Dados
- **Node.js & Express:** Camada de API para gerenciamento de dados, rotas de consulta e submissões.
- **Supabase (PostgreSQL):** Banco de dados relacional gerenciado na nuvem.
  - Tabela `opportunities`: Cadastro de cursos, certificações, tags, cargas horárias e metadados.
  - Tabela `submissions`: Fila de oportunidades enviadas pela comunidade para triagem.
  - Tabela `admin_users`: Controle de acesso autenticado.
- **Segurança & Validação:** Validação estrita de schemas com **Zod**, autenticação via **JWT** e hashing de senhas com **bcryptjs**.

### Deploy & Hospedagem
- **Vercel:** Hospedagem com distribuição global por CDN e suporte a Serverless Functions.

---

## 🗺️ Próximos Passos (Roadmap)

- [ ] **Automações de Validação de Links:** Criação de scripts/agentes para checagem periódica da integridade e status das URLs das plataformas parceiras.
- [ ] **Integração Discord Bot:** Notificações automáticas de novas oportunidades adicionadas diretamente no servidor da comunidade.
- [ ] **Filtros Avançados:** Filtro por plataformas parceiras específicas e tipo de credencial.

---

## 👨‍💻 Autor

**Pedro Henrique Caputo**  
Estudante de Ciência da Computação — Cruzeiro do Sul  
- [LinkedIn](https://www.linkedin.com/in/pedro-caputo/)  
- [GitHub](https://github.com/pedro-caputo)

---

## 📄 Licença

Este repositório de apresentação e documentação está sob a licença [MIT](LICENSE).
