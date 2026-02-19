# Relatório Técnico – T1047 Windows Management Instrumentation (WMI)

## Visão Geral

A técnica T1047 descreve o uso do WMI para execução remota de comandos e movimentação lateral.

## Como o Ataque Funciona

WMI permite administração remota legítima. No entanto, atacantes utilizam essa funcionalidade para:

- Executar processos remotamente
- Criar persistência
- Coletar informações do sistema

Por ser uma ferramenta nativa do Windows, muitas vezes passa despercebida.

## Impacto

- Movimentação lateral silenciosa
- Execução remota sem ferramentas externas
- Dificuldade de detecção sem monitoramento adequado

## Cenário Prático em um SOC

O SOC deve monitorar:

- Processos iniciados por wmiprvse.exe
- Conexões remotas via WMI
- Execução de comandos administrativos fora do padrão

## Conclusão

O uso malicioso do WMI é comum em ataques internos e requer visibilidade aprofundada de logs e comportamento de processos.