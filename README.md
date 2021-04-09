# HUD

## Criando a HUD basica de um personagem

Neste exemplo vamos inserir uma HUD básica de **VIDA** do personagem.
- Primeiramente criamos um evento de **Dano** na blueprint do personagem:

![AddCustomEvent](imagens/AddCustomEvent.jpg)

![EventDano](imagens/EventDano.jpg)

Logo após, criamos uma variável tipo **float** com o nome **Vida**;
Em seguida seguimos com a lógica do Dano:

![LogicaDano2](imagens/LogicaDano2.jpg)

Com a lógica do **Evento Dano** pronta, seguimos para a criaçao da HUD;

Criamos uma Blueprint Widget para mostrar a vida do persongem na tela. Então para isso:

Criar uma Widget:
- Aperte o botão direito do mouse no content Browser:

![CriandoWidget](imagens/CriandoWidget.jpg)  

- Nomeamos como BP_WidgetHUDHeroi: ![BP_WidgetHUDHeroi](imagens/BP_WidgetHUDHeroi.jpg)

- Em seguida, abra o blueprint criado:

![telawidget](imagens/telawidget.jpg)

- Arraste o text até a tela tracejada, no exemplo acima foi inserido dois Texts, onde um foi nomeado com Vida e o outro em branco onde será realizado uma **bind** onde será mostrado a vida do personagem;

- No text destacado na imagem acima, é feito uma **bind**:

![BindWidget](imagens/BindWidget.jpg)

Ao criar a bind, será levado até a área de Graph da widget;

![graphWidget](imagens/graphWidget.jpg)

Em seguida, no Event Graph do Blueprint do persongem:

![CreateWidgetBPpersonagem](imagens/CreateWidgetBPpersonagem.jpg)

![Widgetdopersonagem](imagens/Widgetdopersonagem.jpg)

Após isto, voltar ao **BP_WidgetHUDHeroi**:

No Event Graph do Widget:

- Criar a referência ao personagem:

![ReferenciaPersonagem](imagens/ReferenciaPersonagem.jpg)

em seguida, inserir a referência:

![inserindoreferenciaperson2](imagens/inserindoreferenciaperson2.jpg)

![inserindoreferenciaperson3](imagens/inserindoreferenciaperson3.jpg)

![inserindoreferenciaperson4](imagens/inserindoreferenciaperson4.jpg)

Em seguida, salvar e compilar;

![Widgetnatela](imagens/Widgetnatela.jpg)
