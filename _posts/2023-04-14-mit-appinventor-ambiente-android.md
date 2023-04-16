<p><span style="font-weight: 400;">O <strong>MIT App Inventor</strong> é um ambiente de programação visual intuitivo que permite a todos criar aplicativos totalmente funcionais para celulares Android, iPhones e tablets Android/iOS. Além disso, a ferramenta utiliza um estilo de programação em blocos que facilita a criação de aplicativos complexos e de alto impacto em ambientes de programação significativamente menores do que os ambientes tradicionais de programação.</span></p>
<p><span style="font-weight: 400;">Tendo em vista a praticidade dessa plataforma de programação, esse artigo tem como finalidade ensinar você a criar sua conta, descrever os componentes de interface disponíveis na plataforma de modo que você sairá apto a fazer sua primeira criação.</span></p>
<h2>Criando sua conta no Mit App Inventor</h2>
<p>Ao entrar no site <a href="https://appinventor.mit.edu/">Mit App Inventor</a> você se deparará com a seguinte tela:</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/1-1.png"/>

<p><span style="font-weight: 400;">Clique no botão <strong>“Create Apps!”</strong>. Após isto, você será redirecionado para uma tela de login em que deverá escolher a forma como deseja logar para iniciar a criação dos aplicativos. Em seguida, você estará nesta tela:</span></p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/2-1.png"/>

<p><span style="font-weight: 400;">Selecione a opção <strong>“Start New Project”</strong> e em seguida nomeie o aplicativo que será criado.</span></p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/3-1.png"/>

<p>Após ter realizado todos esses passos, estaremos nesta tela em que iremos desenvolver o layout e a programação de nosso aplicativo:</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/4.png"/>

<h2>Componentes de Interface</h2>
<p>Os componentes de interface são aqueles que permitem ao usuário do aplicativo interagir com o programa, eles se encontram do lado esquerdo da tela do seu computador. Para colocá-los dentro do seu aplicativo basta posicionar o mouse em cima do componente que você deseja usar, apertar o botão esquerdo do mouse e arrastá-lo para dentro do celular ilustrado no meio da tela.</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/5-1.png"/>

<p><strong>Button</strong></p>
<p>Botão tem a capacidade de detectar cliques na tela. Muitos aspectos de sua aparência podem ser alterados, bem como se ele é clicável. Suas propriedades podem ser alteradas no Designer ou no Editor de Blocos.</p>
<p><strong>CheckBox</strong></p>
<p>O componente pode detectar toques do usuário e podem alterar seu estado booleano (é um tipo de dado primitivo que possui dois valores, que podem ser considerados como 0 ou 1, falso ou verdadeiro.) em resposta.<br />
Um componente levanta um evento quando o usuário o toca. Existem muitas propriedades que afetam sua aparência que podem ser definidas no Designer ou Editor de Blocos.</p>
<p><strong>DatePicker</strong></p>
<p>Um botão que, quando clicado, lança uma caixa de diálogo pop-up para permitir que o usuário selecione uma data no Calendário Gregoriano. A data e a hora são manipuladas usando métodos no componente Relógio.</p>
<p><strong>Image</strong></p>
<p>Componente para exibir imagens e animações básicas. A imagem a ser exibida e outros aspectos da aparência da Imagem podem ser especificadas no Designer ou no Editor de Blocos.</p>
<p><strong>Label</strong></p>
<p>São componentes usados para mostrar texto. A Label exibe o texto especificado pela propriedade. Todas as propriedades podem ser definidas no Designer ou Editor de Blocos, que controlam a aparência e colocação do texto.</p>
<p><strong>ListPicker</strong></p>
<p>Um botão que, quando clicado, exibe uma lista de textos para o usuário escolher entre. Os textos podem ser especificados através do Designer ou Editor de Blocos definindo a propriedade ElementsFromString para sua concatenação separada por strings (por exemplo) ou definindo a propriedade Elements para uma lista no editor Blocos.<br />
Definindo a propriedade ShowFilterBar para, tornará a lista pesquisável. Outras propriedades afetam a aparência do botão (TextAlignment, BackgroundColor, etc.) e se ele pode ser clicado (Ativado).</p>
<p><strong>ListView</strong></p>
<p>Este é um componente que exibe uma lista de elementos de texto e/ou imagens na tela para o usuário selecionar. Listas simples de strings podem ser definidas usando a propriedade ElementsFromString (do mesmo modo que ListPicker). Listas mais complexas de elementos contendo várias strings e/ou imagens podem ser criadas usando as propriedades ListData e ListViewLayout. Aviso: Este componente não funcionará corretamente em telas que são roláveis se sua altura estiver definida para preencher a tela completamente.</p>
<p><strong>Notifier</strong></p>
<p>O componente Notifier exibe mensagens de alerta e cria entradas de log do Android através de uma variedade de métodos.</p>
<p><strong>PasswordTextBox</strong></p>
<p>Permite que os usuários digitem senhas em um componente de caixa de texto de senha, que oculta o texto digitado nele. Este componente é bem similar ao TextBox comum, contudo, não exibe os caracteres que o usuário digitou.<br />
Em geral, este componente é utilizado junto com um Button para que uma ação seja executada ao finalizar a digitação do texto.</p>
<p><strong>Slider</strong></p>
<p>O slider é uma barra deslizante em que o usuário pode alterar os valores de seleção do polegar de controle. À medida que o polegar deslizante é arrastado, ele acionará o evento PositionChanged, relatando a posição do polegar. A posição relatada do polegar pode ser usada para atualizar dinamicamente outro atributo componente, como o FontSize de uma Label ou o Raio de um.SliderTextBoxBall<br />
O componente possui valores padrão que podem facilmente serem alterados com base nas suas necessidades. Os valores são os seguintes:<br />
MinValue = 10<br />
MaxValue = 50<br />
Posição do Polegar = 30</p>
<p><strong>Spinner</strong></p>
<p>Exibe uma caixa de diálogo com uma lista de elementos. Pode-se definir a propriedade ElementsFromString em uma lista separada de címula de valores (por exemplo) ou definindo a propriedade Elements em uma lista no Editor de Blocos.</p>
<p><strong>Switch</strong></p>
<p>O componente pode detectar toques do usuário e podem alterar seu estado booleano em resposta. Sua estrutura de programação é similar a CheckBox, tendo de diferença apenas sua aparência. Os switches possuem dois estados: on (verdadeiro) e off (falso).</p>
<p><strong>TextBox</strong></p>
<p>Caixa de texto que permite que os usuários digitem o que desejarem. A propriedade MultiLine determina se o texto pode ter mais de uma linha. Para uma caixa de texto de uma única linha, o teclado fechará automaticamente quando o usuário pressionar a tecla Done. Para fechar o teclado para caixas de texto multiline, o aplicativo deve usar o método HideKeyboard. A propriedade NumbersOnly restringe o teclado a aceitar apenas entrada numérica. O componente possui outras propriedades que afetam o aparecimento da caixa de texto (TextAlignment, BackgroundColor, etc.) e se ela pode ser usada (Habilitada). As caixas de texto geralmente são usadas com o componente Botão, com o usuário clicando nele quando a entrada de texto estiver concluída.</p>
<p><strong>TimePicker</strong></p>
<p>Um botão que, quando clicado, abre uma caixa de diálogo para permitir que o usuário selecionar uma hora (Obs: A data e a hora são manipuladas usando métodos no componente Relógio).</p>
<p><strong>WebViewer</strong></p>
<p>Componente para visualização de páginas da Web. O HomeUrl pode ser especificado no Designer ou no Editor de Blocos. A exibição pode ser definida para seguir links quando eles são grampeados, e os usuários podem preencher formulários da Web.<br />
É válido destacar que este não é um navegador completo. Por exemplo, pressionar a “tecla de voltar” do aparelho celular sairá do aplicativo, em vez de voltar ao histórico do navegador.<br />
Você pode usar a propriedade WebViewString para fazer a comunicação entre seu aplicativo e código Javascript em execução na página.</p>
<h2>Criando seu primeiro aplicativo no Mit App Inventor</h2>
<p>Neste momento, você já conhece todos os componentes de interface disponíveis na plataforma <strong>Mit App Inventor</strong>. Sendo assim, separamos um modelo de aplicativo para demonstrar como colocar seus novos conhecimentos em prática.</p>
<p>Primeiramente coloque 3 botões no celular ilustrado no centro da tela do seu computador:</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/6-1.png"/>

<p>Neste momento, iremos alterar as propriedades de cada botão. Selecione o primeiro botão, você notará que aparece a seguinte tabela no lado direito da tela:</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/7-2.png"/>

<p>Iremos alterar estes valores com base no que desejamos.</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/8-1.png"/>

<p>Repare que realizamos mudanças nas propriedades do botão conforme o design que nós queríamos, faça o mesmo com os três botões do seu aplicativo. Crie o design que mais lhe agrada. Mas utilize o seguinte texto nos botões 1, 2 e 3 respectivamente: “Mudar Texto”, “Vibrar” e “Abrir outra tela”, pois essas são as três funções que lhe ensinaremos a fazer neste artigo.</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/9-1.png"/>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/9-1.png" alt="" width="600" height="338"/>



<p>Após fazer as alterações nas propriedades dos botões, iremos alterar os nomes de cada um deles, para facilitar no entendimento da programação. Vá na aba “Components” e selecione o “Button1”, clique em “Rename” e digite “Mudar Texto” na caixa “New name”.</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/10-1.png"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/10-1.png" alt="" width="266" height="121"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/11-1.png"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/11-1.png" alt="" width="617" height="294"/>

<p>Agora, daremos início a programação em blocos do nosso aplicativo. No canto superior direito, selecione a opção “Blocks” e a seguinte tela aparecerá:</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/12-1.png"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/12-1.png" alt="" width="600" height="283"/>
</picture>
</noscript></p>
<p>Para voltar para a tela anterior, basta clicar na opção “Designer” no canto superior direito da tela.</p>
<p>No lado esquerdo clique no nome do nosso botão “Mudar Texto”.</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/13-1.png"/>


<p>Agora, aparecerão vários blocos que você pode selecionar para configurar a ação desse botão.</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/14-1.png"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/14-1.png" alt="" width="512" height="576"/>


<p>Arraste o primeiro bloco que está escrito: “When Mudar_Texto click do” para o meio da tela. Clique novamente nas opções do botão “Mudar Texto” e desça os blocos que apareceram até achar o seguinte bloco:</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/15-1.png"/>



<img src="https://www.makerhero.com/wp-content/uploads/2022/12/16-1.png"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/16-1.png" alt="" width="268" height="72"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/17-1.png"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/17-1.png" alt="" width="158" height="227"/>


<p>Pegue o primeiro bloco e arraste-o até os que havíamos montado, você perceberá que programar nesta plataforma é como montar um quebra-cabeça.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/18.png"/>




<img src="https://www.makerhero.com/wp-content/uploads/2022/12/19.png"/>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/19.png" alt="" width="294" height="88"/>


<p>Digite no quadrado rosa o que você deseja que apareça no texto do botão.</p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/20.png" alt="" width="554" height="67"/>

          
<p>Agora, iremos configurar o segundo Botão utilizando a mesma lógica do primeiro:</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/21.png" alt="" width="380" height="386"/>

          
          
<p>Voltaremos agora na aba <strong>“Designer”</strong> para adicionar um componente de som em nosso App. Do lado esquerdo, digite a palavra “Sound” no campo de pesquisa da paleta de componentes:</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/22.png" alt="" width="171" height="148"/>

          >
<p>Selecione o terceiro componente que apareceu, arraste-o e solte na tela do celular, ele é um componente invisível. Agora, vamos voltar para a tela <strong>“Blocks”</strong>. Do mesmo modo que pegamos um bloco para configurar os botões, pegaremos no componente Sound.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/23.png" alt="" width="489" height="505"/>

          
<p>Arraste o bloco <strong>“Call Sound1 Vibrate Millisecs”</strong> e conecte-o com o bloco do botão de Vibrar que havíamos colocado no meio da tela.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/24.png" alt="" width="190" height="93"/>

          
<p>Por fim, adicionaremos a quantidade de tempo que o celular ficará vibrando. Vá na categoria <strong>“Math”</strong> no canto esquerdo e selecione o quadrado azul que possui apenas um <strong>“0”</strong> escrito. Arraste e conecte no bloco acima.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/25.png" alt="" width="223" height="107"/>

          
<p>Como o componente Sound funciona em milissegundos, 1 segundo é equivalente a 1000 milissegundos. Sendo assim, vamos configurá-lo para vibrar por 3 segundos.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/26.png" alt="" width="238" height="104"/>

          
<p>Agora, faremos o terceiro botão. Deste modo, repetiremos o primeiro passo dos outros dois botões.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/27.png" alt="" width="444" height="377"/>

<p>Vá até a categoria <strong>“Control”</strong> e encontre o bloco <strong>“Open another screen&#8230; ScreenName:”</strong>, conecte-o com o bloco do botão<strong> “Abrir outra tela”</strong>.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/28.png" alt="" width="299" height="61"/>

<p>Para abrir outra tela, precisamos criar uma tela segundária. Para isto, clique em <strong>“Add screen”</strong> no canto superior da tela. Adicione o nome da segunda tela e clique em<strong> “ok”</strong>.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/29.png" alt="" width="600" height="306"/>

          
<p>Para voltar na tela principal, vá no canto superior da tela e clique no nome da segunda Tela e selecione <strong>“Screen1”</strong>.</p>


<img src="https://www.makerhero.com/wp-content/uploads/2022/12/30.png" alt="" width="490" height="113"/>

<p>Volte no Blocks da tela 1 e vá até o último bloco que nós criamos. Altere a opção de tela que está escolhida e selecione <strong>“SegundaTela”</strong></p>

<img src="https://www.makerhero.com/wp-content/uploads/2022/12/31.png" alt="" width="374" height="95"/>


<p>Pronto, neste momento, terminamos nosso aplicativo. Para baixa-lo em seu celular vá no canto superior e clique em <strong>“Build” 🡪 “Android App (.apk)”</strong><br />

  
<img src="https://www.makerhero.com/wp-content/uploads/2022/12/32.png" alt="" width="494" height="83"/>

<p>Espere-o compilar e escaneie o QRcode com seu smartphone, Talvez seja necessário que você altere as permissões do seu celular para que ele consiga instalar o programa. Clique nos botões e veja a mágica acontecer. Parabéns, você criou seu primeiro aplicativo! Aproveite e use sua criatividade como desejar.
<hr />
