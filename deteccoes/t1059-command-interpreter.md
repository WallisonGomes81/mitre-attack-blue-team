# T1059 - Command and Scripting Interpreter

## Objetivo
Detectar execução suspeita de comandos via PowerShell, CMD ou scripts automatizados.

## Descrição da Técnica
A técnica T1059 permite que atacantes executem comandos arbitrários utilizando interpretadores de comando.

## Fonte de Log
- Windows Security Event ID 4688
- PowerShell Event ID 4104 (Script Block Logging)
- Sysmon Event ID 1

## Indicadores de Comprometimento
- Execução de PowerShell com parâmetros suspeitos (-enc, -nop, -w hidden)
- Download de arquivos via PowerShell
- Execução de scripts remotos

## Severidade
Alta

## Ação Recomendada
- Bloquear execução remota
- Analisar comandos executados
- Verificar persistência no sistema

## Referência
MITRE ATT&CK - T1059