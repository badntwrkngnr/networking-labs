01-underlay-multi-wan: dois ou mais links de saída (ISPs simulados), rotas default, NAT. É a base antes de ligar o SD-WAN.
02-sdwan-zones-members: criação da interface SD-WAN, membros, zonas e política de firewall apontando para a zona.
03-performance-sla: health checks (latência, jitter, perda de pacote) para medir a qualidade de cada link.
04-sdwan-rules: estratégias de seleção (manual, best quality, lowest cost, maximize bandwidth) e steering por aplicação ou destino.
05-overlay-ipsec-advpn: túneis IPsec entre sites como membros SD-WAN, depois ADVPN (hub-and-spoke com atalhos spoke-to-spoke).
06-sdwan-bgp-overlay: BGP sobre o overlay, no padrão de design da Fortinet (hub como route reflector, spokes como clientes).
07-troubleshooting: comandos de diagnóstico (diagnose sys sdwan ...), cenários de falha de link e de SLA.