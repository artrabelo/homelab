# Visão geral

Documentação do meu ambiente virtualizado para estudo prático de infraestrutura de rede, aplicando conceitos de rede, administração de firewall e provisionamento de VMs.

## Estrutura do projeto

- Host: Arch Linux
- Firewall: OPNsense
- Rede:
  - `vtnet0`: rede WAN (192.168.4.0/24)
  - `vtnet1`: rede LAN para VMs internas (192.168.5.0/24)
- Estrutura lógica:
  - `192.168.5.254` - OPNsense
  - `192.168.5.10` - Active Directory (Windows Server)

## Para fazer

- Uma aplicação baseada em Ansible e FastAPI para receber mensagens de estados das VMs e aplicar configurações
- Aplicar políticas de grupo em clientes Windows através do Active Directory