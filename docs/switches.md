# Mapeamento de Switches

Detalhamento de portas, dispositivos conectados, tipo de cabo, modo de conexão e VLAN para cada switch do projeto.

## SwitchEng (Engenharia)

| Portas | Porta Dispositivo | Tipo de Cabo | Dispositivos Conectados | Modo Conexão | VLAN |
|---|---|---|---|---|---|
| Fa0/1 a Fa0/10 | Fa0 | Direto | PcEng01 ao 10 | Acesso | (A) 100 |
| Fa0/13 | Fa0 | Direto | ServDadosEng | Acesso | (B) 200 |
| Fa0/14 | Fa0 | Direto | ImpressEng | Acesso | (B) 200 |
| Gig0/1 | Fa0/1 | Crossover | SwitchCentral | Trunk | Todas |

## SwitchComp (Compras)

| Portas | Porta Dispositivo | Tipo de Cabo | Dispositivos Conectados | Modo Conexão | VLAN |
|---|---|---|---|---|---|
| Fa0/1 a Fa0/10 | Fa0 | Direto | PcComp01 ao 10 | Acesso | (A) 300 |
| Fa0/13 | Fa0 | Direto | ServPed_DHCPComp | Acesso | (B) 400 |
| Fa0/14 | Fa0 | Direto | ImpressComp | Acesso | (B) 400 |
| Gig0/1 | Fa0/2 | Crossover | SwitchCentral | Trunk | Todas |

## SwitchTI (T.I. Interno)

| Portas | Porta Dispositivo | Tipo de Cabo | Dispositivos Conectados | Modo Conexão | VLAN |
|---|---|---|---|---|---|
| Fa0/1 a Fa0/10 | Fa0 | Direto | PcTI01 ao 10 | Acesso | (A) 500 |
| Fa0/13 | Fa0 | Direto | ServDVRTI | Acesso | (B) 600 |
| Fa0/14 | Fa0 | Direto | ImpressTI | Acesso | (B) 600 |
| Gig0/1 | Fa0/3 | Crossover | SwitchCentral | Trunk | Todas |

## SwitchInfra (Infraestrutura)

| Portas | Porta Dispositivo | Tipo de Cabo | Dispositivos Conectados | Modo Conexão | VLAN |
|---|---|---|---|---|---|
| Fa0/1 a Fa0/10 | Fa0 | Direto | PcInfra01 ao 10 | Acesso | (A) 700 |
| Fa0/13 | Fa0 | Direto | ServBKP_DHCPInfra | Acesso | (B) 800 |
| Fa0/14 | Fa0 | Direto | ImpressInfra | Acesso | (B) 800 |
| Gig0/1 | Fa0/4 | Crossover | SwitchCentral | Trunk | Todas |

## SwitchCentral (Central)

| Portas | Porta Dispositivo | Tipo de Cabo | Dispositivos Conectados | Modo Conexão | VLAN |
|---|---|---|---|---|---|
| Fa0/1 | Gig0/1 | Crossover | SwitchEng | Trunk | Todas |
| Fa0/2 | Gig0/1 | Crossover | SwitchComp | Trunk | Todas |
| Fa0/3 | Gig0/1 | Crossover | SwitchTI | Trunk | Todas |
| Fa0/4 | Gig0/1 | Crossover | SwitchInfra | Trunk | Todas |
| Fa0/5 | Fa0 | Direto | ServDNSCentral | Acesso | 900 |
| Fa0/6 | Fa0 | Direto | ServWebCentral | Acesso | 900 |
| Fa0/7 | Gig0/0 | Direto | RoteadorCentral | Trunk | Todas |
