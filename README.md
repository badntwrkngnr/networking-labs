# Networking Labs – Repositório de Prática de Redes

Este repositório reúne laboratórios práticos de redes de computadores que utilizo para estudar, revisar e documentar tópicos fundamentais de networking: CLI e administração de dispositivos, switching, roteamento, serviços IP e segurança. A ideia é centralizar materiais de diferentes fontes confiáveis em um único lugar, com roteiros, topologias e soluções de referência para praticar de forma estruturada.

Os laboratórios atuais foram construídos a partir de conteúdos voltados à certificação Cisco CCNA e utilizam Cisco IOS, mas os conceitos trabalhados (VLANs, STP, OSPF, NAT, ACLs, IPv6, etc.) são universais e aplicáveis a qualquer ambiente de redes. O objetivo do repositório é crescer para além de um único fabricante, passando a cobrir novos temas, plataformas e cenários de automação.

Os laboratórios podem ser executados em **PNETLab/EVE-NG** (arquivos `.zip` com a topologia `.unl`) e, nos labs que já possuem topologia compatível, também no **[Containerlab](https://containerlab.dev)** (arquivos `.clab.yml`). Veja as instruções de cada ferramenta na seção [Como Usar](#como-usar).

## Para quem é este repositório

- Quem estuda para certificações de redes (como a CCNA) e quer praticar com labs prontos.
- Profissionais que querem revisar fundamentos de redes de forma prática.
- Quem está migrando de áreas adjacentes (infraestrutura, desenvolvimento, cloud) e precisa construir base sólida em networking.

## Servidor do Discord

Também criei um servidor no Discord, para quem quiser participar ou ajudar: [NetworkLabs](https://discord.gg/VTpuvYmp)

## Fontes dos Laboratórios

- **[CertSkills](https://www.certskills.com)**
- **[Jeremy's IT Lab](https://www.jeremysitlab.com)**
- **[Workshops do Gustavo Kalau](https://www.youtube.com/@GustavoKalau/playlists)**

Observação: Este repositório organiza e referencia materiais para estudo. Respeite as licenças/termos de uso originais dos autores e cursos.

## Visão Geral dos Temas

| Pasta | Tema | Principais assuntos |
| --- | --- | --- |
| `01-cli-basics/` | Fundamentos de CLI | Configuração básica de switches e roteadores, senhas, SSH/Telnet |
| `02-switching-layer2/` | Switching e Camada 2 | VLANs, trunking, STP/RSTP, VTP, EtherChannel, switching L3 |
| `03-static-routing/` | Roteamento Estático | Rotas estáticas IPv4/IPv6 e troubleshooting |
| `04-dynamic-routing/` | Roteamento Dinâmico | OSPF, RIP |
| `05-ip-services/` | Serviços IP | Endereçamento IPv4/IPv6, DHCP, NAT/PAT, NTP, Syslog, CDP/LLDP, links seriais |
| `06-basic-security/` | Segurança Básica | ACLs, Port Security, DHCP Snooping, DAI |

## Estrutura do Repositório

Os laboratórios estão organizados por temas para facilitar o estudo. Cada diretório de laboratório contém:

- `instructions.md`: roteiro do laboratório e objetivos.
- `lab-solution.md`: referência de solução.
- `assets/`: imagens de topologia, capturas de tela e arquivos `.zip` com as topologias (quando aplicável).

### 📁 Organização por Temas

#### `01-cli-basics/` - Fundamentos de CLI

Configurações básicas de switches e roteadores, segurança de acesso CLI, SSH/Telnet, e exploração de comandos.

- `01_basic-switch-configuration/`
- `02_basic-switch-setup/`
- `03_basic-router-setup/`
- `04_config-lab_cli-passwords-1/`
- `05_config-lab_cli-passwords-2/`
- `06_config-lab_enabling-ssh-and-disabling-telnet/`
- `07_config-lab_switch-ip-1/`
- `08_config-lab_login-security-1/`
- `09_config-lab_cli-miscellany-1/`
- `10_config-lab_switch-duplex-and-speed/`
- `11_config-lab_switch-admin-config/`
- `12_config-lab_switch-ip-config/`
- `13_config-lab_cli-exploration-1/`
- `14_config-lab_cli-exploration-2/`
- `15_config-lab_telnet-config/`
- `16_config-lab_ssh-config/`

#### `02-switching-layer2/` - Switching e Protocolos de Camada 2

VLANs, trunking, STP/RSTP, VTP, EtherChannel (L2 e L3), e troubleshooting de switching.

- `01_ethernet-lan-switching/`
- `02_configuring-switch-interfaces/`
- `03_vlan-and-vtp-configuration/`
- `04_lan-switching-troubleshooting/`
- `05_config-lab_vlan-basics-3/`
- `06_config-lab_data-and-voice-vlan-1/`
- `07_config-lab_data-and-voice-vlan-2/`
- `08_config-lab_trunking-puzzle-1/`
- `09_config-lab_basic-vlans/`
- `10_config-lab_trunking-for-only-some-vlans/`
- `11_config-lab_rstp-config-1/`
- `12_config-lab_rstp-config-2/`
- `13_config-lab_l2-etherchannel-1/`
- `14_config-lab_l2-etherchannel-2/`
- `15_config-lab_big-vlan-and-stp-lab-1/`
- `16_config-lab_roas-basics-1/`
- `17_config-lab_layer3-switching-1/`
- `18_config-lab_layer3-switching-2/`
- `19_config-lab_layer3-switching-with-svis/`
- `20_config-lab_layer3-switching-with-routed-ports/`
- `21_config-lab_l3-etherchannel-1/`

#### `03-static-routing/` - Roteamento Estático

Configuração de rotas estáticas IPv4 e IPv6, e troubleshooting de roteamento.

- `01_static-routes/`
- `02_ip-routing-troubleshooting/`
- `03_config-lab_ipv4-static-routes-1/`
- `04_config-lab_ipv4-static-routes-2/`
- `05_config-lab_ipv4-static-routes-3/`
- `06_config-lab_ipv6-static-routes-1/`
- `07_config-lab_ipv6-static-routes-2/`
- `08_config-lab_ipv4-static-routes-practice-exam-question-1/`

#### `04-dynamic-routing/` - Roteamento Dinâmico

Configuração e otimização de protocolos de roteamento dinâmico como OSPF e RIP.

- `01_rip-v2/`
- `02_config-lab_ospf-interface-config-1/`
- `03_config-lab_ospf-interface-config-2/`
- `04_config-lab_ospf-network-config-1/`
- `05_config-lab_ospf-network-config-2/`
- `06_config-lab_ospf-multi-area-ospf-1/`
- `07_config-lab_ospf-multi-area-ospf-2/`
- `08_config-lab_ospf-dr-priority/`
- `09_config-lab_ospf-network-type/`
- `10_config-lab_ospf-router-ids/`
- `11_config-lab_ospf-metrics/`

#### `05-ip-services/` - Serviços IP

Endereçamento IPv4/IPv6, DHCP, NAT/PAT, links seriais (HDLC, PPP, Frame Relay), NTP, Syslog, e protocolos de descoberta (CDP/LLDP).

- `01_configuring-serial-links/`
- `02_hdlc/`
- `03_ppp/`
- `04_frame-relay/`
- `05_config-lab_ipv4-addressess-1/`
- `06_config-lab_ipv4-addressess-2/`
- `07_config-lab_ipv4-addressess-3/`
- `08_config-lab_ipv4-addressess-4/`
- `09_config-lab_ipv4-addressess-5/`
- `10_config-lab_dhcp-relay/`
- `11_config-lab_router-as-dhcp-client/`
- `12_config-lab_ipv6-eui64-addressing-1/`
- `13_config-lab_ipv6-global-unicast-addressing-1/`
- `14_config-lab_ipv6-special-addresses-1/`
- `15_config-lab_ipv6-special-addresses-2/`
- `16_config-lab_cdp-lldp-1/`
- `17_config-lab_ntp-client-and-server/`
- `18_config-lab_syslog-1/`
- `19_config-lab_syslog-2/`
- `20_config-lab_syslog-3/`
- `21_config-lab_dynamic-nat-1/`
- `22_config-lab_static-nat-1/`
- `23_config-lab_interface-pat-1/`
- `24_config-lab_pat-with-a-pool-1/`

#### `06-basic-security/` - Segurança Básica

ACLs (padrão e estendidas), Port Security, DHCP Snooping, DAI e outras técnicas de segurança de camada 2.

- `01_port-security/`
- `02_config-lab_standard-numbered-acl-1/`
- `03_config-lab_standard-named-acl-1/`
- `04_config-lab_extended-numbered-acl-1/`
- `05_config-lab_extended-named-acl-1/`
- `06_config-lab_basic-port-security-1/`
- `07_config-lab_basic-port-security-2/`
- `08_config-lab_basic-port-security-3/`
- `09_config-lab_basic-port-security-4/`
- `10_config-lab_dhcp-snooping-1/`
- `11_config-lab_dhcp-snooping-2/`
- `12_config-lab_dai-1/`

## Pré-requisitos

- PNETLab ou EVE-NG **ou** Containerlab (veja os requisitos específicos em [Executando um Lab no Containerlab](#executando-um-lab-no-containerlab)).
- Conhecimentos básicos de redes (modelo OSI/TCP-IP, endereçamento IP).
- Noções de CLI. Os laboratórios atuais utilizam Cisco IOS; novos laboratórios poderão utilizar outras plataformas, que serão indicadas no `instructions.md` de cada lab.

## Como Usar

1. Clone o repositório.
2. Navegue até o tema desejado (ex.: `01-cli-basics/`, `02-switching-layer2/`, etc.).
3. Escolha um diretório de lab (ex.: `01-cli-basics/02_basic-switch-setup/`).
4. Leia o `instructions.md` para entender objetivos e passos.
5. Abra a topologia correspondente na ferramenta (arquivos em `assets/lab/`): o `.zip` contendo `.unl` para PNETLab/EVE-NG, ou o arquivo `.clab.yml` para o Containerlab (quando disponível).
6. Execute as configurações conforme o roteiro.
7. Compare seu resultado com o `lab-solution.md` e ajuste o que for necessário.

Exemplo de clonagem:

```
git clone https://github.com/badntwrkngnr/networking-labs.git
cd networking-labs
```

### Importando um Lab no PNETLab/EVE-NG

Para importar um lab, você deve baixar o arquivo `.zip` dentro da pasta do lab desejado. Após realizar o download, você deve acessar o seu PNETLab (o processo é muito semelhante no EVE-NG):

#### 1. Na tela inicial, clique em 'Import' conforme o exemplo abaixo:

![Importando o Lab](./assets/img/00-import-lab.png)

#### 2. Selecione o arquivo e clique em 'Upload':

![Escolhendo o arquivo](./assets/img/01-choose-file.png)

#### 3. Clique em 'Upload' na coluna 'Actions':

![Fazendo o Upload](./assets/img/02-upload.png)

#### 4. Ao final do processo, você verá uma mensagem de sucesso:

![Upload realizado com sucesso](./assets/img/03-success.png)

#### 5. Na lista de labs, aparecerá o lab que você fez o upload:
![Lab listado](./assets/img/04-listed-lab.png)

#### 6. Clique no lab e depois em 'Open':

![Abrindo o Lab](./assets/img/05-abrindo-o-lab.png)

#### 7. Antes de iniciar os equipamentos, você deve fazer os procedimentos abaixo, para que os equipamentos iniciem com as configurações que deixei prontas previamente. Naquele ícone do lado esquerdo, apenas passe o mouse que irá abrir um menu de opções:

![Menu de Opções](./assets/img/06-iniciando-o-lab-1.png)

#### 8. Ao abrir o menu, clique em 'Setup Nodes':

![Setup Nodes](./assets/img/07-iniciando-o-lab-2.png)

#### 9. Clique em 'Wipe All Nodes' para limpar todas as configurações dos equipamentos:

![Wipe All Nodes](./assets/img/08-iniciando-o-lab-3.png)

#### 10. Confirme que deseja limpar as configurações clicando em 'Yes':

![Wipe All Nodes? Yes!](./assets/img/09-iniciando-o-lab-4.png)

#### 11. Observe nas notificações ao lado direito que os nodes foram limpos:

![Wiped](./assets/img/10-iniciando-o-lab-5.png)

#### 12. Abra novamente o menu de opções, depois em 'Setup Nodes' e na sequência clique em 'Set Nodes Startup-cfg To Exported':

![Set Nodes Startup-cfg To Exported](./assets/img/11-iniciando-o-lab-6.png)

#### 13. Observe nas notificações que após o boot, os equipamentos irão iniciar com as configurações que foram aplicadas previamente:

![Notificação Exported](./assets/img/12-iniciando-o-lab-7.png)

#### 14. Agora finalmente iremos iniciar os equipamentos. Para isso, você pode fazer individualmente ou ligar todos de uma vez. Para ligar todos de uma vez, será necessário abrir o menu de opções novamente, clicar em 'Setup Nodes' e depois clicar em 'Start All Nodes':

![Start All Nodes](./assets/img/13-iniciando-o-lab-8.png)

#### 15. Observe que ao aparecer o ícone de 'Play', poderemos acessar os equipamentos:

![Equipments Started](./assets/img/14-iniciando-o-lab-9.png)

#### 16. Clique em um dos equipamentos para confirmar que ele já tem configuração aplicada, pois já deve estar com hostname:

![Lab listado](./assets/img/15-iniciando-o-lab-10.png)

#### Para realizar a confirmação das configurações, pode variar de lab para lab, mas com os comandos abaixo já deve ser suficiente:

```cisco
enable
show running-config
```

### Executando um Lab no Containerlab

Além do PNETLab/EVE-NG, os labs podem ser executados com o [Containerlab](https://containerlab.dev), que sobe os equipamentos como containers Docker a partir de um arquivo `.clab.yml`. Vamos demonstrar como utilizar usando o lab `01-cli-basics/01_basic-switch-configuration` que já possui esse arquivo em `assets/lab/basic-switch-configuration.clab.yml`, e os passos abaixo usam esse lab como exemplo. Para os demais labs o processo é o mesmo, bastando usar o `.clab.yml` da pasta correspondente.

#### Requisitos

- Linux x86_64 (ou WSL2 no Windows) com **Docker** e **Containerlab** instalados. Veja o [guia de instalação](https://containerlab.dev/install/).
- Permissão de `sudo` (o Containerlab precisa de privilégios para criar as interfaces de rede).
- Imagens Docker dos equipamentos Cisco IOL, já disponíveis localmente:
  - `vrnetlab/cisco_iol:17.18.02` (roteador)
  - `vrnetlab/cisco_iol:l2-17.18.02` (switch L2)
- A imagem dos "PCs" (`wbitt/network-multitool:alpine-extra`) é baixada automaticamente do Docker Hub.

> **Importante:** as imagens Cisco IOL **não** estão neste repositório e não podem ser redistribuídas. O binário IOL vem do pacote de imagens de referência do Cisco CML e é transformado em imagem Docker com o projeto [vrnetlab](https://github.com/hellt/vrnetlab). O passo a passo está na [documentação do Containerlab](https://containerlab.dev/manual/kinds/cisco_iol/).

#### 1. Confirme que o Docker e o Containerlab estão instalados:

```bash
docker --version
containerlab version
```

#### 2. Confirme que as imagens do Cisco IOL existem no seu Docker:

```bash
docker images | grep -E "cisco_iol|multitool"
```

Você deve ver as tags `17.18.02` e `l2-17.18.02`. Se as suas imagens tiverem outra tag (por exemplo `L2-17.12.01`), edite o campo `image:` dos nós no arquivo `.clab.yml`. As tags do Docker diferenciam maiúsculas de minúsculas.

#### 3. Entre na pasta onde está o arquivo `.clab.yml` do lab:

```bash
cd 01-cli-basics/01_basic-switch-configuration/assets/lab
```

#### 4. Suba o lab:

```bash
sudo containerlab deploy -t basic-switch-configuration.clab.yml
```

O Containerlab cria os containers e as conexões entre eles. O IOL leva alguns minutos para terminar o boot, então aguarde antes de acessar os equipamentos. Ao final, será exibida uma tabela com os nós do lab.

#### 5. Confira se todos os nós estão rodando:

```bash
sudo containerlab inspect -t basic-switch-configuration.clab.yml
```

Todos os nós (`r1`, `sw1`, `pc1`, `pc2` e `pc3`) devem aparecer com o estado `running`. A tabela mostra também o endereço IP de gerência de cada nó.

#### 6. Entenda o mapeamento das interfaces:

No Containerlab, a interface `Ethernet0/0` do IOL é reservada para a **gerência** (conectada à rede de gerência do Docker). As interfaces de dados começam em `eth1`, que corresponde a `Ethernet0/1` (`e0/1`). Por isso, os números das interfaces são diferentes da topologia do PNETLab mostrada em `assets/img/topology.png`:

| Conexão | Containerlab | Nome no IOS (Containerlab) | PNETLab (`topology.png`) |
| --- | --- | --- | --- |
| R1 ↔ SW1 | `r1:eth1` ↔ `sw1:eth1` | R1 `e0/1` ↔ SW1 `e0/1` | R1 `e0/0` ↔ SW1 `e0/0` |
| SW1 ↔ PC1 | `sw1:eth2` ↔ `pc1:eth1` | SW1 `e0/2` | SW1 `e0/1` |
| SW1 ↔ PC2 | `sw1:eth3` ↔ `pc2:eth1` | SW1 `e0/3` | SW1 `e0/2` |
| SW1 ↔ PC3 | `sw1:eth4` ↔ `pc3:eth1` | SW1 `e0/4` | SW1 `e0/3` |

Os PCs já sobem com endereço IP configurado na `eth1`: `pc1` = `192.168.0.13/24`, `pc2` = `192.168.0.14/24` e `pc3` = `192.168.0.15/24`.

#### 7. Acesse o roteador e o switch via SSH:

```bash
ssh admin@r1
ssh admin@sw1
```

O usuário e a senha padrão são `admin` / `admin`. Os nomes `r1` e `sw1` são os nomes dos containers (o arquivo usa `prefix: ""`). Se o nome não for resolvido, use o endereço IP mostrado no `containerlab inspect`.

> Para acessar o IOS, use sempre o SSH. O comando `docker exec -it r1 bash` abre um shell Linux do container, não a CLI do IOS.

#### 8. Acesse os PCs e teste a conectividade entre eles:

```bash
docker exec -it pc1 sh
ip addr show eth1
ping -c 3 192.168.0.14
```

Os PCs devem se comunicar através do switch. Se o ping falhar logo após o `deploy`, aguarde o switch terminar de iniciar e tente novamente.

#### 9. Realize o lab:

Abra o `instructions.md` do lab e execute as configurações no `r1` e no `sw1` por SSH. Se o seu usuário já entrar direto no modo EXEC privilegiado, use o comando `disable` para voltar ao modo EXEC usuário antes de testar as senhas dos passos 3 e 8 do lab.

#### 10. Salve a configuração e compare com a solução:

```cisco
copy running-config startup-config
```

Depois compare o seu resultado com o `lab-solution.md`.

#### 11. Encerre ou reinicie o lab:

Para desligar o lab **mantendo** as configurações que você salvou:

```bash
sudo containerlab destroy -t basic-switch-configuration.clab.yml
```

Para apagar tudo e recomeçar do zero (equivalente ao 'Wipe All Nodes' do PNETLab):

```bash
sudo containerlab destroy -t basic-switch-configuration.clab.yml --cleanup
sudo containerlab deploy -t basic-switch-configuration.clab.yml
```

> O Containerlab cria uma pasta `clab-basic-switch-configuration/` ao lado do `.clab.yml` durante o `deploy`. Ela guarda os dados do lab e não deve ser enviada ao Git (adicione `clab-*/` ao `.gitignore`).

#### Problemas comuns

| Sintoma | O que verificar |
| --- | --- |
| `pull access denied` ou imagem não encontrada | A imagem Cisco IOL não existe localmente ou a tag é diferente da usada no `.clab.yml` (passo 2). |
| `permission denied` ao executar o `containerlab` | Execute com `sudo`. |
| Sem acesso SSH ao switch (`sw1`) | Aguarde o boot completo e confira se o nó do switch tem `type: L2` no `.clab.yml`, que é o valor usado na documentação do Containerlab para a imagem IOL-L2. |
| O ping entre os PCs não funciona | Aguarde o boot do switch e confira o IP da `eth1` de cada PC com `ip addr show eth1`. |

## Boas Práticas de Estudo

- **Refaça**: repita o lab sem olhar a solução até dominar o procedimento.
- **Varie**: altere endereçamento, topologia e parâmetros para testar sua compreensão.
- **Documente**: registre comandos, resultados de verificação e aprendizados.

## Roadmap (ideias futuras)

- Incluir checklists de verificação (show commands) por tópico.
- Adicionar mais laboratórios de troubleshooting avançado.
- Expandir o conteúdo para além do Cisco IOS, com labs em outras plataformas e fabricantes.
- Adicionar novos temas, como BGP, redes em datacenter, VPNs, QoS e wireless.
- Incluir laboratórios de automação de redes (Python, Ansible, APIs) aplicados aos cenários já existentes.
- Adicionar topologias Containerlab (`.clab.yml`) aos demais laboratórios.

## Contribuição

Sugestões e correções são bem-vindas. Abra uma Issue ou envie um Pull Request com:

- Descrição clara do problema/melhoria.
- Prints/topologias se aplicável.
- Referências (quando derivado de conteúdo de terceiros).

## Licença

Consulte o arquivo `LICENSE` para detalhes. Materiais de terceiros citados/organizados aqui permanecem sob suas respectivas licenças.