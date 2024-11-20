# -Auto-Injection-de-ID-nas-APIs

O documento descreve como configurar e registrar automaticamente handlers de **commands** e **queries** no sistema utilizando o **MediatR** em um projeto .NET. Ele faz o seguinte:

1. **Inicialização de Commands e Queries**: 
   - Define classes (`InicializeCommand` e `InicializeQuery`) para identificar e registrar automaticamente todos os **handlers** (implementações de `IRequestHandler<,>`) localizados no assembly do projeto.

2. **Configuração de Serviços com MediatR**:
   - Usa o método `AddMediatR` para configurar o MediatR e registrar handlers diretamente a partir do assembly.

3. **Simplificação da Injeção de Dependência**:
   - As classes encapsulam a lógica de registro de serviços, garantindo que handlers de commands e queries sejam automaticamente reconhecidos e adicionados ao contêiner de injeção de dependência.

4. **Facilidade de Integração**:
   - Torna o processo de integração com o MediatR mais organizado, centralizando a configuração em classes específicas e reutilizáveis.

Em resumo, o documento padroniza e simplifica a configuração do MediatR no projeto para lidar com commands e queries, economizando tempo e reduzindo o risco de erros manuais no registro de handlers.


