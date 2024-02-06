---
up: "[[Spaces/Home/Notas Temporárias/Questões/Questões.md]]"
---

# Tópico 1
| Questão Nº  | Observação                                                                                                       |
|-----|------------------------------------------------------------------------------------------------------------------|
| 1   | Para redeploy de VMs sempre usar Redeploy blade                                                                 |
| 3   | Para Armazenar certificados, senha ou qualquer dado sensível use Azure Key Vault                                 |
| 4   | Use Policy Access para criar restrições para acesso a os dados sensíveis                                         |
| 5   | Para implantar o arquivo de manifesto YAML para o aplicativo em AKS use o comando `kubectl apply "f myapp.yaml` |
| 6   | Quando falamos de `platformFaultDomainCount` no ARM. O número de domínios de falha para conjuntos de disponibilidade gerenciados varia de acordo com a região – dois ou três por região. |
| 7   | O limite superior de `platformUpdateDomainCount` é 20                                                             |
| 8   | Plano de consumo reduzirá o custo total operação caso a hospedagem caso não precise ficar ligada o tempo todo.  |
| 9   | Para migrar migrar o MongoDB para a conta do Azure Cosmos DB precisamos mongorestore                              |
| 10  | Uma identidade gerenciada do Azure Active Directory permite que seu aplicativo acesse facilmente outros recursos protegidos pelo AAD, como o Azure Key Vault. |
| 11  | Sempre antes de criar o `az webapp` precisa criar `az appservice plan create`                                     |
| 12  | No Azure KeyVault o SoftDelete é uma quarentena para a lixeira                                                  |
| 13  | No Azure KeyVault o PurgeProtection é uma quarentena de remoção total sem volta de recuperação dos dados       |
| 14  | Para ser notificado à partir de métricas usamos azure monitor                                                    |
| 15  | Para criar notificação do azure monitor é necessário uma parâmetro de condicional e parâmetro temporal           |
| 16  | Usamos --window size para contar um período de tempo                                                             |














17. O SendGrid é serviço de envio de email. Existem dois tipo de modelo para Azure Functions sendo eles  SendGrid Action sendo síncrono e Biding SendGrid sendo assíncrono. Um exemplo da diferença entre os dois seria caso optasse pelo modelo sincrono seria o bloqueio da execução do aplicativo de funções até que o email fosse enviado, já o modelo assíncrono não haveria bloqueio 

18. Os domínios customizados precisão de certificado TLS que é passado via HTTP Request Header em Base64

19. Os domínios fornecidos pelo azure, conhecido `nomedosite.azurewebsites.com.net` tem seu TLS automático

20. Sempre antes de criar o `az webapp` precisa criar `az appservice plan create`

21. Para criar webapp a partir dokerfile devemos primeiro criar as variáveis de ambiente depois criamos webapp e depois configuramos dokerfile e só depois o host

22. Function App no Plano Premium (evita qualquer inicialização a frio e Plano de Consumo não suporta VNet

23. Uma identidade atribuída pelo sistema está vinculada ao seu aplicativo e será excluída se o seu aplicativo for excluído

24. Para lidar com azure functions que ultrapassam o tempo limite a melhor solução é Durable Function async pattern

25. Independentemente da configuração de tempo limite do aplicativo de funções, 230 segundos é o tempo máximo que uma função disparada por HTTP pode levar para responder a um pedido

26. O feed de alterações fornece logs de transações de todas as alterações que ocorrem nos blobs e nos metadados de blob em sua conta de armazenamento.

27. A primeira instrução no Dockerfile deve ser a instrução FROM para especificar a imagem a ser usada como imagem base. Em seguida, especifique o diretório de trabalho da imagem. Em seguida, copie todo o conteúdo do aplicativo usando o comando COPY. Em seguida, use o comando CMD para executar o comando PowerShell e a instrução ENTRYPOINT para executar o aplicativo dotnet.

28. Para este cenário em que as imagens devem ser processadas o mais rápido possível e a latência deve ser minimizada, recomenda-se usar o plano de Serviço de Aplicativo em vez do plano de Consumo no azure functions.

29. Sempre usar Grande de Eventos quando queremos captar um disparo de um evento contido no azure

30. Termos 'menos de um minuto' ou 'baixa latência' refletem um grande possibilidade de necesitar de grande de eventos







