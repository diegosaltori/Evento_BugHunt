# 🧪 Casos de Teste — PhotoGram  
**Versão:** 1.0  
**Sistema:** PhotoGram  
**Propósito:** Roteiro base para apoiar os testes exploratórios do evento Bug Hunt  
**Autor:** Diego Saltori  
**Evento:** Bug Hunt — PhotoGram  

---

## 🧾 Tela de Registro

### 🧩 Caso de Teste 01 — Registro de novo usuário
**Versão:** 1.0  
**Objetivo:** Validar o processo de criação de uma nova conta de usuário.  

#### Passos
1. Acessar a tela de registro.  
   - **Resultado Esperado:** A tela deve exibir os campos necessários para criar uma conta.  
2. Preencher apenas o campo “Nome de Usuário” e clicar em “Registrar”.  
   - **Resultado Esperado:** O sistema deve exibir alguma forma de retorno (mensagem ou redirecionamento).  
3. Repetir o teste preenchendo apenas o campo “Senha”.  
   - **Resultado Esperado:** O sistema deve se comportar de forma consistente com o caso anterior.  
4. Preencher ambos os campos e clicar em “Registrar”.  
   - **Resultado Esperado:** O sistema deve criar o usuário e redirecionar para a tela de login.  

> 💡 *Dica:* Observe se há campos opcionais, confirmações ou validações implícitas que possam faltar.  

---

## 🔐 Tela de Login

### 🧩 Caso de Teste 02 — Login com credenciais válidas
**Versão:** 1.0  
**Objetivo:** Verificar se o login funciona corretamente e se o fluxo de acesso está coerente.  

#### Passos
1. Acessar a tela de login.  
   - **Resultado Esperado:** Campos “Usuário” e “Senha” devem estar visíveis.  
2. Inserir um nome de usuário e senha válidos e clicar em “Entrar”.  
   - **Resultado Esperado:** O sistema deve permitir o acesso e redirecionar para o dashboard.  
3. Fazer logout e tentar novamente com uma senha incorreta.  
   - **Resultado Esperado:** O sistema deve exibir uma mensagem genérica de erro de autenticação.  

> 💡 *Dica:* Observe como o sistema trata mensagens de erro e feedbacks visuais.  

---

## 🏠 Tela de Dashboard

### 🧩 Caso de Teste 03 — Exibição de postagens
**Versão:** 1.0  
**Objetivo:** Validar a visualização e o comportamento dos elementos na tela principal.  

#### Passos
1. Acessar o dashboard após o login.  
   - **Resultado Esperado:** As postagens devem ser carregadas e exibidas em lista.  
2. Verificar se há botões de ação (Editar, Excluir) em cada postagem.  
   - **Resultado Esperado:** Os botões devem estar disponíveis conforme o design definido.  
3. Clicar no botão “Excluir” em uma postagem.  
   - **Resultado Esperado:** O sistema deve remover a postagem da tela (sem travamentos).  
4. Utilizar o campo de filtro e digitar parte do título de uma postagem existente.  
   - **Resultado Esperado:** Apenas postagens correspondentes devem permanecer visíveis.  

> 💡 *Dica:* Observe se há informações extras sendo exibidas ou se algo incomum aparece no console.  

---

## 📸 Tela de Postagem (Visualização)

### 🧩 Caso de Teste 04 — Visualização de postagem e comentários
**Versão:** 1.0  
**Objetivo:** Verificar o comportamento da tela ao exibir detalhes de uma postagem.  

#### Passos
1. No dashboard, clicar em uma postagem para abrir seus detalhes.  
   - **Resultado Esperado:** A tela deve mostrar título, descrição, autor e data.  
2. Verificar se a saudação do usuário aparece corretamente.  
   - **Resultado Esperado:** O sistema deve exibir uma mensagem de boas-vindas.  
3. Navegar pelo carrossel de fotos.  
   - **Resultado Esperado:** As imagens devem mudar ao interagir com os controles.  
4. Tentar adicionar um comentário e confirmar.  
   - **Resultado Esperado:** O novo comentário deve aparecer na lista.  

> 💡 *Dica:* Observe a forma como o conteúdo é exibido — há algo “estranho” na forma como textos são renderizados?  

---

## ➕ Tela de Nova Postagem (Add)

### 🧩 Caso de Teste 05 — Criação de nova postagem
**Versão:** 1.0  
**Objetivo:** Garantir que o usuário consiga criar uma postagem com título, descrição e fotos.  

#### Passos
1. Acessar a tela de nova postagem.  
   - **Resultado Esperado:** Os campos de título, descrição e fotos devem estar visíveis.  
2. Preencher apenas o título e clicar em “Publicar”.  
   - **Resultado Esperado:** O sistema deve registrar a postagem ou indicar erro de forma clara.  
3. Preencher todos os campos e clicar em “Publicar”.  
   - **Resultado Esperado:** A postagem deve ser criada e o sistema deve redirecionar para a tela inicial.  
4. Observar o tempo de redirecionamento após o envio.  
   - **Resultado Esperado:** O retorno deve ocorrer dentro de um tempo considerado razoável.  

> 💡 *Dica:* Preste atenção no comportamento do sistema durante o redirecionamento — nem sempre o tempo é o mesmo.  

---

### 🧩 Caso de Teste 06 — Melhoria de texto por IA
**Versão:** 1.0  
**Objetivo:** Testar a funcionalidade de melhoria automática de texto na descrição.  

#### Passos
1. Acessar a tela de nova postagem e inserir uma descrição simples.  
   - **Resultado Esperado:** O campo de descrição deve aceitar texto livre.  
2. Clicar no botão “Gerar Melhoria de Texto”.  
   - **Resultado Esperado:** O sistema deve processar a requisição e exibir uma nova versão do texto.  
3. Verificar se o texto aprimorado substitui o original ou se aparece em campo separado.  
   - **Resultado Esperado:** O comportamento deve ser coerente com a proposta da funcionalidade.  
4. Publicar a postagem com o texto melhorado.  
   - **Resultado Esperado:** O texto final deve refletir a versão aprimorada exibida na tela.  

> 💡 *Dica:* Observe se há algum indicativo visual (loading, mensagem, log) durante a execução da IA.  

---

## ✏️ Tela de Edição de Postagem (Edit)

### 🧩 Caso de Teste 07 — Edição de postagem existente
**Versão:** 1.0  
**Objetivo:** Validar a capacidade do usuário de alterar postagens já criadas.  

#### Passos
1. No dashboard, selecionar uma postagem criada anteriormente e clicar em “Editar”.  
   - **Resultado Esperado:** A tela de edição deve abrir com os dados da postagem.  
2. Alterar o título e salvar.  
   - **Resultado Esperado:** O sistema deve confirmar a atualização e exibir o novo título.  
3. Adicionar novas fotos e salvar novamente.  
   - **Resultado Esperado:** O sistema deve aceitar as imagens adicionadas.  
4. Tentar remover uma foto existente.  
   - **Resultado Esperado:** O comportamento do sistema deve indicar se a exclusão é possível.  

> 💡 *Dica:* Compare o layout da tela de edição com o da criação — algo parece fora do padrão?

---

> 🐞 *Desafie-se a ir além dos passos descritos. Questione, investigue e descubra o que o sistema realmente faz.*
