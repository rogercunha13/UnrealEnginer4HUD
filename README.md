# HUD

## Criando a HUD basica de um personagem

Neste exemplo vamos inserir uma HUD básica de **VIDA** do personagem.
- Primeiramente criamos um evento de **Dano** na blueprint do personagem:

![Imagem_AddCustomEvent](ImagensHUD/Imagem_AddCustomEvent.jpg)

![Imagem_EventDano](ImagensHUD/Imagem_EventDano.jpg)

Logo após, criamos uma variável tipo **float** com o nome **Vida**;
Em seguida seguimos com a lógica do Dano:

![Imagem_LogicaDano2](ImagensHUD/Imagem_LogicaDano2.jpg)

Com a lógica do **Evento Dano** pronta, seguimos para a criaçao da HUD;

Criamos uma Blueprint Widget para mostrar a vida do persongem na tela. Então para isso:

Criar uma Widget:
- Aperte o botão direito do mouse no content Browser:

![Imagem_CriandoWidget](ImagensHUD/Imagem_CriandoWidget.jpg)

- Nomeamos como BP_WidgetHUDHeroi: ![BP_WidgetHUDHeroi](imagens/BP_WidgetHUDHeroi.jpg)

- Em seguida, abra o blueprint criado:

![Imagem_telawidget](ImagensHUD/Imagem_telawidget.jpg)

- Arraste o text até a tela tracejada, no exemplo acima foi inserido dois Texts, onde um foi nomeado com Vida e o outro em branco onde será realizado uma **bind** onde será mostrado a vida do personagem;

- No text destacado na imagem acima, é feito uma **bind**:

![Imagem_BindWidget](ImagensHUD/Imagem_BindWidget.jpg)

Ao criar a bind, será levado até a área de Graph da widget;


![Imagem_graphWidget](ImagensHUD/Imagem_graphWidget.jpg)

Em seguida, no Event Graph do Blueprint do persongem:

![Imagem_CreateWidgetBPpersonagem](ImagensHUD/Imagem_CreateWidgetBPpersonagem.jpg)

![Imagem_Widgetdopersonagem](ImagensHUD/Imagem_Widgetdopersonagem.jpg)

Após isto, voltar ao **BP_WidgetHUDHeroi**:

No Event Graph do Widget:

- Criar a referência ao personagem:

![Imagem_ReferenciaPersonagem](ImagensHUD/Imagem_ReferenciaPersonagem.jpg)

em seguida, inserir a referência:

![Imagem_inserindoreferenciaperson2](ImagensHUD/Imagem_inserindoreferenciaperson2.jpg)

![Imagem_inserindoreferenciaperson3](ImagensHUD/Imagem_inserindoreferenciaperson3.jpg)

![Imagem_inserindoreferenciaperson4](ImagensHUD/Imagem_inserindoreferenciaperson4.jpg)

Em seguida, salvar e compilar;

![Imagem_Widgetnatela](ImagensHUD/Imagem_Widgetnatela.jpg)
HUD no viewport.
