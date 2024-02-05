---
tags:
  - azure
---

1. Para redeploy de VMs sempre usar Redeploy blade
2. Para Armazenar certificados, senha ou qualquer dado sensível use Azure Key Vault
	* Use Policy Access para criar restrições para acesso a os dados sensíveis
3. para implantar o arquivo de manifesto YAML para o aplicativo em AKS use o comando ` kubectl apply "f myapp.yaml.` para criar 
4. 
5. 
6. quando falamos de `platformFaultDomainCount` no ARM. O número de domínios de falha para conjuntos de disponibilidade gerenciados varia de acordo com a região – dois ou três por região.
7. O limite superior de `platformUpdateDomainCount` é 20
8. Plano de consumo reduzirá o custo total operação caso a hospedagem caso não precise ficar ligada o tempo todo.                                                                                                                                                                                                                                                                             O SendGrid é serviço de envio de email. Existem dois tipo de modelo para Azure Functions sendo eles  SendGrid Action sendo síncrono e Biding SendGrid sendo assíncrono. Um exemplo da diferença entre os dois seria caso optasse pelo modelo sincrono seria o bloqueio da execução do aplicativo de funções até que o email fosse enviado, já o modelo assíncrono não haveria bloqueio 
9. Os domínios customizados precisão de certificado TLS que é passado via HTTP Request Header em Base64
	* Além disso precisa de uma configuração na propria aplicação
	* Exceção disso são próprios domínios do azure conhecido `nomedosite.azurewebsites.com.net`
10. Sempre antes de criar o `az webapp` precisa criar `az appservice plan create`
11. para criar webapp  a partir dokerfile devemos primeiro criar as variaveis de ambiente depois criamos webapp e depois configuramos dokerfile e só depois o host
12. Function no Plano Premium (evita qualquer inicialização a frio  e Plano de Consumo  n suporta VNet,Uma identidade atribuída pelo sistema está vinculada ao seu aplicativo e será excluída se o seu aplicativo for excluído
13. 
14. 
15. 
16. para lidar azure functions que ultrapassam o tempo limite a melhor solução é Durable Function async pattern
17. 
18. Independentemente da configuração de tempo limite do aplicativo de funções, 230 segundos é o tempo máximo que uma função disparada por HTTP pode levar para responder a um pedido
19. a
20. o feed de alterações fornece logs de transações de todas as alterações que ocorrem nos blobs e nos metadados de blob em sua conta de armazenamento.
21. A primeira instrução no Dockefile deve ser a instrução FROM para especificar a imagem a ser usada como imagem base. Em seguida, especifique o diretório de trabalho da imagem. Em seguida, copie todo o conteúdo do aplicativo usando o comando COPY. Em seguida, use o comando CMD para executar o comando PowerShell e a instrução ENTRYPOINT para executar o aplicativo dotnet.
22. Para este cenário em que as imagens devem ser processadas o mais rápido possível e a latência deve ser minimizada, recomenda-se para azure functions usar o plano de Serviço de Aplicativo em vez do plano de Consumo.
23. Sempre usar Grande de Eventos quando queremos captar um disparo de um evento contido no azure
	* termos <mark style="background: #FFF3A3A6;">'menos de um minuto'</mark> ou <mark style="background: #FFB8EBA6;">'baixa latência'</mark> refletem um grande possibilidade de necesitar de grande de eventos   