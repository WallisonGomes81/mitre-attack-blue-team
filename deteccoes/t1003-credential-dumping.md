# T1003 - Credential Dumping

## Objetivo
Detectar tentativa de extração de credenciais através de acesso ao processo LSASS.

## Descrição da Técnica
A técnica T1003 permite que atacantes obtenham credenciais armazenadas na memória do sistema, frequentemente utilizando ferramentas como Mimikatz.

## Fonte de Log
- Windows Security Event ID 4688 (Process Creation)
- Sysmon Event ID 10 (Process Access)

## Indicadores de Comprometimento
- Processo acessando LSASS.exe
- Execução de ferramentas suspeitas como mimikatz.exe
- Dump de memória do processo LSASS

## Severidade
Alta

## Ação Recomendada
- Isolar a máquina da rede
- Encerrar processos suspeitos
- Forçar redefinição de credenciais
- Realizar análise forense

## Referência
MITRE ATT&CK - T1003