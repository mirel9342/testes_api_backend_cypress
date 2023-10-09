Testes de API: O que são?

Os testes de API são um tipo de teste de software que se concentra em avaliar a funcionalidade do backend de um aplicativo ou sistema. Eles envolvem a verificação de como as APIs (Interfaces de Programação de Aplicativos) se comportam em resposta a solicitações específicas e como elas retornam os dados.

Por que os Testes de API são Importantes?

Os testes de API desempenham um papel crucial no desenvolvimento de software por várias razões:
Validação do Backend: Eles ajudam a garantir que o servidor backend esteja funcionando corretamente, processando solicitações e fornecendo respostas conforme o esperado.

Isolamento de Componentes: Os testes de API isolam a funcionalidade do backend, permitindo que você verifique se cada parte do sistema funciona individualmente, independentemente do frontend.

Eficiência: Eles são mais rápidos e eficientes do que testes de interface do usuário, uma vez que não envolvem renderização de páginas ou interações com a interface gráfica.

Detecção Precoce de Problemas: Ao identificar erros no backend antes que eles afetem o frontend ou os usuários finais, os testes de API ajudam a economizar tempo e recursos na correção de problemas.


Como os Testes de API Funcionam?

Os testes de API envolvem a execução de solicitações HTTP para as APIs do aplicativo e a avaliação das respostas recebidas. Aqui está uma visão geral do processo:

Preparação: Antes de iniciar os testes, você precisa configurar o ambiente, que pode incluir a autenticação, a criação de dados de teste e a preparação de cabeçalhos de solicitação.

Execução de Solicitações: Use uma biblioteca ou ferramenta de teste (como o Cypress, Postman, ou frameworks de teste em Python ou JavaScript) para enviar solicitações HTTP para as APIs que você deseja testar. Isso pode incluir solicitações GET, POST, PUT, DELETE, entre outras.

Asserções: Após receber as respostas das APIs, você define as asserções. As asserções são declarações que especificam o comportamento esperado das APIs. Por exemplo, você pode verificar se o código de status HTTP é 200 (OK), se determinados campos de dados estão presentes na resposta, ou se os valores retornados estão dentro das faixas aceitáveis.

Relatórios e Monitoramento: A maioria das ferramentas de teste de API gera relatórios detalhados que mostram os resultados dos testes. Isso inclui informações sobre quais testes passaram e quais falharam, bem como quaisquer erros ou exceções encontrados.

Iteração e Manutenção: Os testes de API devem ser iterados e atualizados conforme o aplicativo evolui. À medida que novos recursos são adicionados ou requisitos são modificados, os testes também devem ser ajustados para garantir que continuem a verificar a funcionalidade corretamente.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Neste cenário, o objetivo é verificar se o processo de login é bem-sucedido quando as credenciais (email e senha) estão corretas.
Descrição do Teste:
 * Envia uma solicitação POST para o endpoint http://localhost:3000/login.

 * Verifica se o código de status da resposta é igual a 200. Isso garante que a solicitação foi processada com sucesso.

 * Verifica se a mensagem de resposta é igual a "Login realizado com sucesso". Isso verifica se o login foi concluído com sucesso e a mensagem de sucesso esperada é retornada.

Teste Funcional de Validação de Senha Incorreta:

Neste cenário, o objetivo é verificar se o processo de login retorna um erro adequado quando a senha está incorreta.
* Envia uma solicitação POST para o endpoint http://localhost:3000/login.
* Verifica se o código de status da resposta é igual a 401. Isso indica que a solicitação não foi autorizada devido a uma senha incorreta.
* Verifica se a mensagem de resposta é igual a "Email e/ou senha inválidos". Isso confirma que o sistema respondeu corretamente a uma tentativa de login com senha incorreta.

-> Esses testes são importantes para garantir que o processo de login funcione corretamente, validando credenciais corretas e retornando erros apropriados em caso de falha. Certifique-se de que seu sistema está configurado para retornar os códigos de status HTTP e mensagens de erro apropriados, conforme especificado nos testes.

![image](https://github.com/mirel9342/testes_api_backend_cypress/assets/106937455/a3d23b01-86c2-4376-b0c2-400adb3f5b4d)








