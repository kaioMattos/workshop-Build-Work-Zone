# Exercício 2.2 - Criar um aplicativo SAP Fiori usando o SAP Business Application Studio

Neste exercício, você desenvolverá um aplicativo SAPUI5 freestyle simples, seguindo as diretrizes de design do SAP Fiori.

<br>

### Etapa 1: criar um aplicativo SAPUI5 a partir de um modelo

Usando o assistente de criação de aplicativo, você pode, a qualquer momento, clicar no botão Voltar para voltar à etapa anterior ou clicar em uma etapa específica do assistente para voltar a essa etapa.

1. Na aba *Get Started* clique **Start from template**.

   ![Start from Template](images/n01-craete-app-frrom-template.png)

2. Selecione **SAP Fiori Application**, e clique em **Start**.

   ![SAP Fiori](images/n02-choose-template-type.png)

3. Na tela *Template Selection*, selecione *Application Type* **SAPUI5 freestyle**

   ![SAPUI5 Freestyle](images/n03-choose-app-type.png)

4. Selecione **SAPUI5 Appliction** escolhaaa basic UI Application e clique em **Next**. 

   ![SAPUI5 App Type](images/n04-choose-empty-UI5-App.png)
   
5. Para *Data Source and Service Selection*, selecione **None** nosso aplicativo não irá consumir nenhum sistema backend. Agora clique em **Next**.

   ![Select Data Source](images/n05-select-datasource-none.png)

6. No proximo passo, você pode escolher um nome padrão para a view ou manter View1, clique em **Next**.

   ![View name](images/n06-keep-view-name.png)

7. Selecione os seguintes **Project Attributes**, e clique em **Next**.

    | Step | Parameter | Value |
    |:-----|:----------|:------|
    | A | Module name | **`helloworld`** |
    | B | Application title | **Hello World** |
    | C | Application namespace | **técnico** |
    | D | Description | **SAPUI5 freestyle application** |
    | E | Project folder path | **`/home/user/projects`** (padrão)|
    | F | Minimum SAPUI5 version | **1.102.1** (padrão) |
    | G | Add deployment configuration | **Yes**|
    | H | Add FLP configuration | **Yes** |
    | I | Configure advanced options | **No** (padrão) |

   ![Project Attributes](images/n07-enter-project-attributes.png)
    
8. Para **Deployment Configuration**, selecione **Cloud Foundry** na lista e o *Destination Name* como **None**. clique em **Next**. selecione o botão de opção **Yes** no input `Add Application to managed application router?`

   ![Deployment Settings](images/n08-deployment-config.png)

9. Por fim, na tela **Fiori Launchpad Configuration**  selecione o seguinte e clique em **Finish**. 

    | Step | Parameter | Value |
    |:-----|:----------|:------|
    | A | Semantic Object | **helloworld** |
    | B | Action | **display** |
    | B | Title | **My Hello World** |
    | B | Subtitle (optional) | **App Customizado UI5** |

    ![Launchpad configuration](images/n09-flp-config.png)


10. Aguarde até que a instalação das dependências do projeto seja concluída. Uma notificação de que "O projeto foi gerado" aparece na parte inferior direita da tela. Você obteria um pop-up como mostrado abaixo. Selecione  **open folder** para ver a estrutura da pasta do Projeto gerada no espaço de trabalho.
    
    ![application generated](images/n10-open-folder-in-workspace.png)
    
 Caso demore muito ou o pop-up não apareça, você também pode abrir a pasta no painel esquerdo **Open Folder**  e selecionar o caminho da pasta como `/home/user/projects/` escolha **helloworld**.

![application generated](images/n10a-alternative-open-folder.png)

<br>

### Etapa 4: execute o aplicativo localmente no Dev Space

Para testar seu aplicativo, agora você pode executá-lo localmente no SAP Business Application Studio.

1.	No painel esquerdo do *Explorer* clique com o botão direito do mouse na pasta **webapp** e selecione **Preview Application** no menu de contexto.

    ![Preview App](images/n12-preview-app.png)

2.	Selecione a primeira entrada **`Start fiori run...`** para executar o aplicativo localmente.

    ![Start helloworld](images/n13-select-run-command.png)

3. Agora você deve ver o aplicativo *Hello World*

 >Se o seu navegador não permitir a abertura de uma nova guia, você poderá ver uma mensagem no canto superior esquerdo com um link para permitir a abertura de uma nova guia.
   
   ![select flp lauchpad](images/n18-preview-app.png)
   
<br>

## Resumo

Agora você criou um aplicativo simples. No próximo exercício, você criará o aplicativo e o implementará no Cloud Foundry.

Continue para - [Exercício 2.3 - Crie e implemente seu aplicativo ](../ex2.3/README.md)
