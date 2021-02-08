# Inspector

A janela **Inspector** ( às vezes referida como "the inspector") exibe informações detalhadas sobre o GameObject selecionado, incluindo os comportamentos atrelados e suas propriedades e permite que você modifique as funcionalidades do GameObject na sua **Scene**.

Manter o **Inspector** organizado é importante, entre outras coisas, para evitar equívocos na introdução de dados para testar e ajustar os comportamentos criados facilitando tanto o trabalho de outros programadores no projeto e de outros membros como game designers.

Dentre as diversas ferramentas fornecidas nativamente pela Unity3D os **atributos** são de longe uma excelente opção para organizar o **Inspector**. 

**Figura 01  - Seleção de camera vista no Inspector**

![Inspector](https://i.imgur.com/2l5HR6T.png)

 **Fonte: O autor.**

## Atributos

São marcadores que podem ser posicionados acima de classes, propriedades ou funções em um script para indicar um comportamento especial. Por exemplo, **[HideInInspector]** que pode ser adicionado a uma propriedade para prevenir que a mesma seja exibida no **inspector**.

**Figura 02 - Script utilizando o atributo "HideInInspector" e Inspector do GameObject.**

![VisaoScript](https://i.imgur.com/xoEDiOo.png)

**Fonte: O autor.**

### Lista de atributos



#### Atributos de propriedade 



* **HideInInspector:** Faz com que a propriedade deixe de ser exibida no Inspector.

   

   ``[HideInInspector] public bool Ativo = true; ``

  

* **Range:** Limita a faixa de valores que podem ser usado por uma variavel do tipo float ou int.

  

   ``[Range(0,25)] public float RaioDeVisao; ``

  

* **Min:** Limita o valor mínimo que pode ser atribuído a uma variavel do tipo float ou int.

  

   ``[Min(1)] public float VidaMaximaDoPersonagem; ``

  

* **Multiline:** Faz com que o Inspector exiba mais de uma linha para variáveis do tipo string.

  

   ``[Multiline(2)] public string NomeDoPersonagem; ``

  

* **TextArea:** Faz com que o Inspector exiba uma caixa de texto rolável a ao se extrapolar o número  máximo de linhas informado.

  

   ``[TextArea(3,5)] public string BackgroundDoPersonamge; ``

  

* **ColorUsage:** Faz com que o Inspector habilite ou não a exibição do seletor de alpha e opções de HDR na na janela de seleção de cores.

  

   ``[ColorUsage(true,true)]public Color CorDoOculo;  ``

  

* **GradientUsage:** Faz com que o Inspector exiba opções de HDR na janela de seleção de gradiente.

  

   ``[GradientUsage(true)] public Gradient GradienteDeCor; ``

  

  **Figura 03 - Inspector mostrando todos os atributos listados acima.**

  ![VisaoScript](https://i.imgur.com/JguBpHs.png)

  **Fonte: O autor.**

  