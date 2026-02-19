# Relatório Técnico – T1003 Credential Dumping

## Visão Geral

A técnica T1003 – Credential Dumping descreve métodos utilizados por atacantes para extrair credenciais armazenadas em sistemas comprometidos. Essas credenciais podem incluir senhas em texto claro, hashes NTLM e tickets Kerberos.

## Como o Ataque Funciona

O ataque geralmente ocorre após a fase de pós-exploração, quando o invasor já possui acesso inicial ao sistema.

O processo LSASS (Local Security Authority Subsystem Service) armazena credenciais em memória. Ferramentas como Mimikatz exploram esse processo para extrair essas informações.

## Impacto

- Comprometimento de contas administrativas
- Movimentação lateral
- Escalonamento de privilégios
- Comprometimento total do domínio

## Cenário Prático em um SOC

Em um ambiente corporativo, o SOC deve monitorar:

- Acesso suspeito ao processo LSASS
- Execução de ferramentas conhecidas de dump
- Criação de arquivos de dump de memória

A rápida identificação pode evitar a propagação do ataque na rede.

## Conclusão

Credential Dumping é uma técnica crítica amplamente utilizada em ataques reais e exige monitoramento constante e políticas rígidas de proteção de credenciais.