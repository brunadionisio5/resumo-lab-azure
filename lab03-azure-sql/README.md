# Laboratório Azure: Configuração de Instância de Banco de Dados (SQL)

Este repositório contém resumos, anotações e dicas sobre como criar e configurar uma instância gerenciada de banco de dados SQL no Microsoft Azure, conforme proposto no desafio da DIO.

---

## 📋 Resumo dos Passos

1. **Acessar o Portal Azure**
   - Site: [https://portal.azure.com](https://portal.azure.com)

2. **Criar um recurso**
   - Clique em “+ Criar um recurso”
   - Selecione “Banco de Dados” > “Instância Gerenciada de SQL”

3. **Configurar a Instância**
   - Nome do recurso: escolha um nome único
   - Região: selecione a mais próxima
   - Credenciais de administrador: configure usuário e senha
   - Capacidade: escolha o plano (atenção ao custo!)

4. **Configurar rede**
   - Certifique-se de configurar a rede virtual corretamente
   - Permitir acesso à porta 1433 (se necessário)

5. **Revisar e criar**
   - Verifique todas as configurações
   - Clique em “Criar” e aguarde a implantação

---

## 🛠️ Dicas Importantes

- Use nomes consistentes para seus recursos no Azure.
- Configure grupos de recursos para manter tudo organizado.
- Habilite backups automáticos para garantir segurança.
- Teste a conexão ao banco usando ferramentas como Azure Data Studio ou SQL Server Management Studio (SSMS).
- Atenção à configuração de firewall para permitir conexões externas (se necessário).

---

## 🔗 Links Úteis

- [Documentação Oficial - Criar Instância Gerenciada de SQL](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart)
- [Guia Rápido GitHub](https://docs.github.com/pt/get-started/quickstart/hello-world)
- [Guia Markdown no GitHub](https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github)