APP_NAME - Sippy


### **RFs (Requisitos Funcionais)**

[1].  **Cadastro de Solicitações de Avaliação**
   - O residente deve poder enviar uma solicitação para avaliação de instalação de painel solar, preenchendo um formulário com:
     - Nome
     - E-mail
     - Telefone
     - Endereço com validação de endereço de Los Angeles (completamento automático)
     - Horário preferido para a avaliação

[2]. **Gerenciamento de Solicitações pelo Admin**  
   - O funcionário do município deve ter acesso a uma lista de todas as solicitações, podendo visualizar detalhes como status, horário e informações de contato.

[3]. **Visualização de Solicitações no Mapa**  
   - O funcionário do município deve poder ver as solicitações de avaliação em um mapa, com cada endereço marcado em ordem de visita.

[4]. **Agendamento Otimizado**  
   - Um algoritmo deve ordenar as visitas por proximidade e horário preferido, minimizando o tempo de deslocamento entre elas.

[5]. **Exportação de Agenda de Visitas**  
   - O funcionário deve poder exportar a agenda de visitas planejadas (em PDF ou Excel) com detalhes do residente, horário e endereço.

[6]. **Notificações por E-mail**  
   - Um sistema de notificação deve enviar e-mails aos residentes, informando o horário exato da visita um dia antes.

[7]. **Login de Admin**  
   - A aplicação deve permitir que apenas funcionários predefinidos da prefeitura façam login com autenticação via Google ou GitHub OAuth.

---

### **RNs (Regras de Negócio)**

[1]. **Validação de Endereço**  
   - Somente endereços válidos de Los Angeles devem ser aceitos no sistema, garantindo que as visitas estejam dentro da área da cidade.

[2]. **Autorização de Funcionários**  
   - Somente funcionários preaprovados (definidos por e-mails verificados) podem acessar a área administrativa.

[3]. **Preferência de Horário Indicativa**  
   - O horário preferido pelo residente é apenas uma indicação e não uma garantia, podendo ser ajustado pelo sistema de acordo com a rota otimizada.

[4]. **Cancelamento de Solicitações**  
   - Os residentes podem cancelar uma solicitação a qualquer momento antes da visita.

[5]. **Controle de Status**  
   - A solicitação deve ter status de "pendente", "confirmado", ou "visitado", atualizado conforme o progresso.

---

### **RNFs (Requisitos Não-Funcionais)**

[1]. **Escalabilidade**  
   - O back-end deve ser escalável para suportar um grande número de solicitações e usuários simultâneos, utilizando práticas modulares e otimizadas.

[2]. **Segurança**  
   - O sistema deve proteger os dados do usuário, garantindo armazenamento seguro e aplicando boas práticas de autenticação OAuth para admins.

[3]. **Desempenho**  
   - A aplicação deve responder rapidamente às ações dos usuários, com uma latência aceitável tanto para o front-end quanto para o back-end.

[4]. **Disponibilidade**  
   - A aplicação deve estar disponível 99% do tempo durante o horário comercial, minimizando o tempo de inatividade.

[5]. **Responsividade**  
   - A interface do usuário deve ser responsiva, permitindo uma experiência consistente em dispositivos desktop, tablets e celulares.

[6]. **Manutenção e Testes**  
   - O sistema deve ser documentado e possuir testes automatizados para garantir a qualidade do código e facilitar futuras manutenções e evoluções.

[7]. **Privacidade e Conformidade**  
   - A aplicação deve cumprir regulamentações de privacidade de dados, armazenando informações pessoais de forma segura e permitindo exclusão sob demanda.
