# Validações de Dados em Banco para QA

Este repositório contém um script SQL com **consultas úteis para validação de dados diretamente no banco**, com foco em atividades comuns da área de QA (Quality Assurance).

As queries podem ser utilizadas como parte de uma verificação manual pós-teste ou para garantir a integridade de massas de dados em ambientes de desenvolvimento, homologação ou produção (quando permitido).

---

## 🧪 O que esse script faz?

O arquivo `validacoes_qa.sql` realiza as seguintes validações:

- Verifica se há usuários sem e-mail cadastrado
- Identifica datas de nascimento inseridas no futuro
- Checa por CPFs duplicados
- Busca usuários com nome ausente ou vazio
- Lista todos os valores distintos no campo `status`

---

## 📌 Quando usar?

- Após o cadastro de um novo usuário para validar se os dados foram persistidos corretamente
- Durante a criação de massa de testes
- Em testes de regressão envolvendo integridade de dados
- Em auditorias manuais no banco

---
## 📂 Estrutura

- `validacoes_qa.sql`: script principal com consultas SQL para validações manuais
- `README.md`: este arquivo com instruções e explicações
- `bdd_validacoes.txt`: validação de dados no banco para usuários

