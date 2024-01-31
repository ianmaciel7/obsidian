1. Para redeploy de VMs sempre usar Redeploy blade
2. Para Armazenar certificados, senha ou qualquer dado sensível use Azure Key Vault
	* Use Policy Access para criar restrições para acesso a os dados sensíveis
3. para implantar o arquivo de manifesto YAML para o aplicativo em AKS use o comando ` kubectl apply "f myapp.yaml.` para criar 
4. 
5. 
6. quando falamos de `platformFaultDomainCount` no ARM. O número de domínios de falha para conjuntos de disponibilidade gerenciados varia de acordo com a região – dois ou três por região.
7. O limite superior de `platformUpdateDomainCount` é 20
8. plano de consumo reduzirá o custo e
9. Sempre usar Grande de Eventos quando queremos captar um disparo de um evento contido no azure
	* termos <mark style="background: #FFF3A3A6;">'menos de um minuto'</mark> ou <mark style="background: #FFB8EBA6;">'baixa latência'</mark> refletem um grande possibilidade de nessitar de grande de eventos   