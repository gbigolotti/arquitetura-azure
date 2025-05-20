# arquitetura-azure

Pré-requisitos:

Conta Azure ativa

Grupo de recursos existente ou novo

Rede virtual configurada (VNet) com sub-rede dedicada

Criação da Instância Gerenciada:

Acesse o Portal do Azure.

Busque por "SQL Managed Instances" e clique em "Criar".

Preencha os campos obrigatórios:

Assinatura: Selecione sua assinatura Azure.

Grupo de recursos: Use um existente ou crie um novo.

Nome da Instância Gerenciada: Ex: sql-mi-demo.

Região: Escolha uma região suportada.

Redes virtuais: Configure ou selecione uma VNet existente.

Defina Credenciais de administrador (login e senha do SQL).

Revise e clique em "Criar" (o processo pode levar até 6 horas).

Validação:

Após a implantação, acesse a instância no Portal.

Use o SQL Server Management Studio (SSMS) para conectar-se usando o endereço DNS da instância.

Estrutura do Repositório GitHub
/sql-managed-instance-demo  
│   README.md  
│   LICENSE  
│   .gitignore  
│   connectivity-guide.md  (opcional)  
└───/images  
     portal-config.png  
     vnet-setup.png  
     ssms-connection.png  
Conteúdo do README.md
(Template personalizável)

markdown
# 🗃️ Instância Gerenciada de SQL do Azure - Demonstração  

Documentação do processo de criação e configuração de uma Instância Gerenciada de SQL no Azure.  

## 🎯 Objetivo  
- Implementar uma Instância Gerenciada de SQL seguindo a [documentação oficial](https://learn.microsoft.com/pt-br/azure/azure-sql/managed-instance/instance-create-quickstart).  
- Validar a conectividade via SSMS.  

## 📋 Passos Realizados  
1. **Configuração de Rede**:  
   - Criação de rede virtual (VNet) com sub-rede dedicada.  
2. **Implantação da Instância**:  
   - Definição de nome, região e credenciais no Portal do Azure.  
3. **Validação**:  
   - Conexão ao banco de dados via SSMS.  

## ⚙️ Pré-requisitos  
- Conta Azure ativa  
- SQL Server Management Studio (SSMS) instalado  
- Permissões de administrador na assinatura  

## 📸 Screenshots  
<p align="center">
  <img src="/images/portal-config.png" width="300" alt="Configuração no Portal">
  <img src="/images/ssms-connection.png" width="300" alt="Conexão SSMS">
</p>

## 📁 Como Usar Este Repositório  
```bash
git clone https://github.com/seu-usuario/sql-managed-instance-demo.git
🔗 Recursos Úteis
Documentação Oficial da Instância Gerenciada

Guia de Conectividade

📜 Licença
Este projeto está sob a licença MIT. Veja LICENSE para detalhes.


---

### **Passo a Passo para Criar o Repositório**  
1. **Crie o repositório no GitHub**:  
   - Nome: `sql-managed-instance-demo` (público).  
   - Adicione o arquivo `README.md` usando o template acima.  

2. **Adicione arquivos extras**:  
   - `.gitignore`: Use [este template](https://github.com/github/gitignore/blob/main/VisualStudio.gitignore).  
   - `LICENSE`: Escolha uma licença (ex: MIT).  

3. **Organize as screenshots**:  
   - Renomeie as imagens para `portal-config.png`, `ssms-connection.png`, etc.  
   - Faça upload para a pasta `/images`.  

4. **Gere o ZIP**:  
   - No GitHub, clique em `Code > Download ZIP`.  

---

### **Descrição para Entrega do Projeto**  
*(Copie este texto ao enviar o projeto)*  
Repositório criado para documentar a implantação de uma Instância Gerenciada de SQL no Azure, seguindo o guia oficial da Microsoft. Inclui:

README.md com detalhes técnicos e screenshots

Configuração de rede virtual (VNet)

Validação via SQL Server Management Studio
