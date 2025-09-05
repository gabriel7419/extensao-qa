## Cenário 03: Gestão de funcionários via módulo PIM.

### Caso de Teste 01: Adicionar novo funcionário com dados válidos.

| ID       | Descrição                                                          |
| :------- | :----------------------------------------------------------------- |
| C03-CT01 | O sistema deve permitir o cadastro de um funcionário com dados válidos. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo PIM.       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** clica em \"Add Employee\"                                  |
| **E** preenche \"John\" no campo First Name e \"Doe\" no Last Name |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** o funcionário deve ser cadastrado e exibido na lista do PIM |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O funcionário deve aparecer corretamente listado no módulo PIM. |

**CENÁRIO TESTADO E EVIDENCIADO: **
https://jam.dev/c/c8e9ce83-3d9a-418d-9f38-f58f52cb4616

---

### Caso de Teste 02: Tentar adicionar funcionário sem preencher campos obrigatórios.

| ID       | Descrição                                                                  |
| :------- | :------------------------------------------------------------------------- |
| C03-CT02 | O sistema deve exibir erros ao tentar salvar um funcionário sem preencher os campos obrigatórios. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa a tela de \"Add Employee\"          |
| **E** deixa os campos obrigatórios em branco                     |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** mensagens de erro devem ser exibidas nos campos obrigatórios |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagens de validação.     |

**CENÁRIO TESTADO E EVIDENCIADO: **
https://jam.dev/c/a4307efe-e560-4652-9334-2a351403c137

---

### Caso de Teste 03: Pesquisar funcionário já cadastrado.

| ID       | Descrição                                                  |
| :------- | :--------------------------------------------------------- |
| C03-CT03 | O sistema deve retornar corretamente o funcionário pesquisado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O funcionário deve já estar cadastrado no sistema.            |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"PIM\"                     |
| **E** digita \"John Doe\" no campo de busca                      |
| **QUANDO** clicar no botão \"Search\"                            |
| **ENTÃO** o sistema deve exibir \"John Doe\" na lista de resultados |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O funcionário correspondente deve ser listado corretamente.     |

**CENÁRIO TESTADO E EVIDENCIADO**
[C03-CT03](https://jam.dev/c/f46ec73f-8622-4751-812b-2beee5401404)
