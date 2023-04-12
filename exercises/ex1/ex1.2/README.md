# Adicione um aplicativo SAPUI5 ao seu site

Neste exercício, você usará o **Content Manager** para adicionar um aplicativo SAPUI5 ao seu site. Você também criará um grupo e atribuirá o aplicativo a ele.

## Pré-requisitos
 - Você já criou o `JobCore`.  

<br>

### Step 1:  abra o Content Manager

 Clique no ícone do Content Manager  no painel lateral para abrir o **Content Manager**.

>O  **Content Manager** tem duas guias: **My Content** , onde você pode configurar manualmente os itens de conteúdo e visualizar quaisquer outros itens de conteúdo disponíveis, e o **Content Explorer** , onde pode explorar o conteúdo exposto de canais disponíveis, selecionar o conteúdo e adicioná-lo ao seu próprio conteúdo.

  ![Open Content Manager](images/4a-content-manager.png)


<br>

### Etapa 2: criar e configurar um novo aplicativo

1.  Clique em **+ New** e selecione  **App** na lista.

    ![Add an app](images/5a-new-app.png)


    O editor de aplicativos é aberto com a guia **PROPERTIES** tab in focus.

2. Digite os seguintes valores:

    * **Title**: `New Orders`

    * **Open App**: no lugar

    * **URL**:  `https://sapui5.hana.ondemand.com/test-resources/sap/m/demokit/cart/webapp/index.html`

    ![Enter app properties](images/5b-app-properties.png)

    >Ao trabalhar em seu próprio ambiente, é melhor integrar os aplicativos SAPUI5 usando o repositório de aplicativos HTML5. Essa configuração permite que você gerencie melhor seu conteúdo no ciclo de vida Dev-QA-Prod. Você verá como fazer isso no exercício 2.

3. Clique na guia **NAVIGATION** para especificar a intenção do seu aplicativo.

    ![Go to Navigation](images/5c-go-to-navigation.png)

    > A combinação única de um objeto semântico e uma ação é chamada de intenção. Ele é usado para definir a navegação para um aplicativo.

4. Digite os seguintes valores:

    * **Semantic Object**: `Order`

    * **Action**: `Display`

    ![Add navigation properties](images/5d-navigation-props.png)

5. Clique na guia **VISUALIZATION**.

    Nesta guia, você especifica como o Tile do aplicativo será exibido no site.

6. Digite os seguintes valores:

      * **Subtitle**: `Shopping Cart `

      * **Information**:  `Order Now!`

      * **Icon**: Clique no ícone de navegação, digite `my-sales-order`, clique no ícone exibido e clique em **OK**.

      À direita, você pode ver uma visualização do bloco com todas as propriedades inseridas. Clique em **Save**.

    ![Add visualization properties](images/6a-visualization.png)

<br>

### Etapa 3: visualizar o aplicativo que você criou

Clique no ícone **Back** para navegar de volta ao *Content Manager*. Você também pode clicar no ícone do Content Manager no painel esquerdo.

  ![Go back to Content Manager](images/7a-back-to-content-manager.png)

Você pode ver seu aplicativo nesta lista

![View app in content manager list](images/8a-view-app.png)

Para que os usuários finais acessem o aplicativo em tempo de execução, você deve atribuir o aplicativo a uma role.Você também precisa atribuir o aplicativo a um grupo para que fique visível no site.

<br>

### atribuir o aplicativo à role Everyone 


>O conteúdo atribuído à role `Everyone`  fica visível para todos os usuários. Além disso, a role `Everyone`  é atribuída por padrão a cada site.

1. Clique na role **Everyone** .

    ![Select everyone role](images/9a-everyone-role.png)

2. Clique em **Editar**.

    ![Click Edit](images/10a-edit.png)

3. Clique na caixa de pesquisa no painel **Assignments** à direita. Todos os aplicativos disponíveis são mostrados na lista abaixo.   

4. Na lista **Results** , clique no ícone **+** ao lado do `New Orders` para atribuir essa role ao seu aplicativo.

    ![Assign role to app](images/11a-assign-role.png)    

5. Clique em **Salvar**.

    ![Save](images/12a-save.png)
    
6. Clique no ícone **Back** para navegar de volta ao *Content Manager*. 

<br>

### Etapa 5: crie um grupo e atribua o aplicativo a ele

<br>

>Um grupo é um conjunto de um ou mais aplicativos exibidos juntos em um site da barra de ativação. A atribuição de aplicativos a grupos os torna visíveis para o usuário.
 Assigning apps to groups, makes them visible to the user.
   ![Group](images/13a-group.png)
   
<br>

1. Clique em  **+ New** e selecione **Group** para criar um grupo.

    ![Add a new group](images/14a-new-group.png)

2. Digite  `Purchasing` como **Title** e no painel **Assignments** clique dentro da caixa de pesquisa à direita da tela, para mostrar todos os aplicativos disponíveis. Você deveria ver `New Orders`.

3. Na lista **Results** , clique em **+** para atribuir o  `New Orders` ao seu grupo.

    ![Configure group properties](images/17a-configure-group.png)

4. Clique em **Save**.

    ![Save group](images/18a-save.png)

<br>

### Etapa 6: revise o site

1. Clique no ícone Site Directory no painel esquerdo para abrir o **Site Directory**.

    ![Open Site Directory](images/19a-to-site-directory.png)

2. No tile `JobCore` , clique no ícone  **Go to site**.

    ![Go to site](images/20a-open-site.png)

3. Isso é o que você vai ver:

    ![View site](images/21a-JobCore-site.png)

    Seu  App `New Orders` é exibido no grupo `Purchasing` .
    

4. Clique no Tile `New Orders` para iniciar o aplicativo.

   ![View app](images/22a-new-orders-app.png)

No aplicativo, clique em qualquer categoria à esquerda para ver as ofertas de produtos.

<br>

## Resumo

Você adicionou com sucesso um aplicativo ao seu site. Agora você verá agora uma demonstração de como consumir conteúdo federado de um sistema SAP S/4HANA Volte ao [Guia principal](../../../README.md) para saber mais sobre a federação de conteúdo.