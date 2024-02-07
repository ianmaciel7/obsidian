---
up: "[[Spaces/Home/Notas Temporárias/Notas Temporárias.md]]"
---
* O Azure Key Vault é um serviço de nuvem projetado para o armazenamento seguro e acesso confiável a segredos[^1]. Este serviço é altamente versátil, podendo ser utilizado em diversos contextos, como em aplicativos web, funções (functions) e outros serviços, tanto dentro do ecossistema Azure quanto externamente a ele.
* Soft-delete behavior / Comportamento de exclusão reversível 
	* também é referido como "soft-delete"
	* permite que os objetos excluídos não sejam imediatamente removidos permanentemente, mas, em vez disso, sejam movidos para um estado de retenção por um período específico antes de serem permanentemente excluídos.
	* tem como finalidade definir tempo de recuperação cofre ou um objeto 
* Purge protection / Proteção contra limpeza
	* é um recurso de segurança que impede a exclusão permanente de objetos ou dados em um serviço ou sistema
	* é um comportamento opcional do Key Vault que não está habilitado por padrão. A só poderá ser habilitada quando a exclusão reversível estiver habilitada.
* Permission model vault / Modelo de permissão do cofre 
	* tem Access Policies Vault / Política de acesso
		* Uma política de acesso ao Key Vault determina se uma determinado entidade de segurança, ou seja, um usuário, aplicativo ou grupo de usuários, pode executar diferentes operações em chaves, segredos e certificados.
	
		


[^1]: segredos são qualquer coisa a qual você queira controlar rigidamente o acesso como Chaves de API como: senhas, certificados, chaves criptográficas, credenciais administrativas e etc..

