# LAB-VLANs-SubInterfaces
Laboratório prático de VLANs e subinterfaces com roteador e switch. Inclui configuração de rede, topologia, testes de conectividade, documentação completa e evidências em imagens.
Lab de VLANs e Subinterfaces – Configuração de Rede Simulada



1. Objetivo
Criar rede simulada com VLANs separadas.
Configurar subinterfaces no roteador para comunicação entre VLANs.
Testar conectividade entre PCs e roteador.
Documentar todo o processo para referência futura.


2. Equipamentos e Recursos
Roteador Cisco (GigabitEthernet0/0)
Switch Cisco
2 PCs virtuais
Cabos Ethernet virtuais
Software de simulação: Packet Tracer ou VirtualBox


3. Topologia da Rede
PC1 (VLAN10) conectado ao Switch
PC2 (VLAN20) conectado ao Switch
Switch conectado ao Roteador (porta G0/0)
VLANs separadas e conectadas ao roteador via trunk


4. Configuração do Roteador
Ativar interface física G0/0
Criar subinterfaces:
G0/0.10 → VLAN10 → IP 192.168.10.1 /24
G0/0.20 → VLAN20 → IP 192.168.20.1 /24
Ativar as subinterfaces


5. Configuração do Switch
Criar VLAN10 e VLAN20
Configurar porta conectada ao roteador como trunk
Atribuir portas dos PCs às VLANs correspondentes:
PC1 → VLAN10
PC2 → VLAN20


6. Configuração dos PCs
PC1: IP 192.168.10.40 /24 → Gateway 192.168.10.1
PC2: IP 192.168.20.10 /24 → Gateway 192.168.20.1


7. Testes de Conectividade
PC1 para PC2: ping bem-sucedido
PC1 para Gateway 192.168.10.1: ping bem-sucedido
PC2 para PC1: ping bem-sucedido
PC2 para Gateway 192.168.20.1: ping bem-sucedido


8. Aprendizados
Diferença entre VLAN e subinterface.
Função do roteador como gateway e roteador entre VLANs.
Importância de configurar trunk para comunicação entre VLANs.
Configuração correta de IPs e gateways.
Teste e troubleshooting de conectividade.


9. Próximos Passos
Adicionar VLAN30 e expandir topologia.
Criar novas subinterfaces no roteador para VLAN adicional.
Testar comunicação entre todas as VLANs.
Continuar documentando novos testes.


10. Prints e Evidências
Roteador: prints/router-config.png
Switch: prints/switch-vlan.png
PC1: prints/pc1-ip.png
PC2: prints/pc2-ip.png
Teste de ping: prints/ping-test.png
