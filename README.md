<h1> 🧭 Resumo: Criação e Configuração de uma Máquina Virtual no Microsoft Azure </h1>

✅ <b>1. Acesso à Plataforma</b>
- Acesse o portal: https://portal.azure.com
- Faça login com sua conta Microsoft (organizacional ou pessoal).

🧱 <b>2. Início da Criação da VM</b>
- No menu lateral, clique em "Máquinas Virtuais" (ou pesquise na barra superior).
- Clique em “+ Criar” > “Máquina virtual”.

📝 <b>3. Configurações Básicas</b>
- Preencha os dados principais:
- Assinatura e Grupo de Recursos: Selecione ou crie um novo grupo de recursos (um "container" para os serviços).
- Nome da VM: Ex: minhaVM1.
- Região: Escolha a região geográfica (ex: Brasil Sul).
- Imagem (Sistema Operacional): Escolha o SO desejado (Windows Server, Ubuntu, etc.).
- Tamanho: Defina a capacidade da VM (CPU, RAM). Azure oferece tamanhos padrão (ex: B1s, D2s_v3).
- Autenticação:
  - Windows: senha ou chave SSH.
  - Linux: geralmente chave SSH.
- Portas de entrada: Ative as portas necessárias (ex: 22 para SSH, 3389 para RDP).

💾 <b>4. Disco (Armazenamento)</b>
- Escolha o tipo de disco do SO: HDD (mais barato) ou SSD (mais rápido).
- Pode adicionar discos de dados posteriormente, se necessário.

🌐 <b>5. Rede</b>
- Crie ou selecione uma rede virtual (VNet).
- Configure a sub-rede.
- Habilite ou desabilite o IP público (necessário para acesso remoto).
- Configure o grupo de segurança de rede (NSG): define regras de tráfego de entrada e saída.

🔒 <b>6. Opções Avançadas (opcional)</b>
- Extensões: scripts ou ferramentas adicionais para instalação automática.
- Monitoramento: habilitar logs, diagnóstico, backup etc.

📦 <b>7. Revisar + Criar</b>
- Revise todas as configurações.
- Clique em “Criar” para iniciar o provisionamento.

🚀 <b>8. Após a Criação</b>
- Acesse a VM pela interface do portal.
- Conecte-se:
- Windows: via RDP.
- Linux: via SSH.
- Instale aplicativos, configure serviços, ajuste firewall interno, etc.

🔁 <b>9. Gerenciamento</b>
- Iniciar/parar/reiniciar a VM.
- Monitorar uso de CPU, memória, disco e rede.
- Redimensionar a VM se necessário.
- Configurar backup, snapshots ou automatizações (runbooks).

💡 <b>Dicas</b>
- Usar tags para organizar e rastrear custos.
- Usar grupos de segurança e firewall do SO juntos para segurança em camadas.
- Avaliar o uso de Azure Bastion para conexões seguras via navegador (sem IP público exposto).
