# Como criar apps da Web na WebView

Leia mais no guia: 
[https://developer.android.com/guide/webapps/webview?hl=pt-br](https://developer.android.com/guide/webapps/webview?hl=pt-br)

<p>Antes de colocar a mão na massa e começar a programar, precisamos verificar se seu site é responsivo e se adapta a diferentes tamanhos de tela.</p>
<p>Precisamos verificar também se seu site é <strong>Mobile-friendly</strong>, ou seja, qual o potencial dele para funcionar em um celular baseado em fatores como responsividade e velocidade de carregamento.</p>
<p>Para fazer esse teste, vamos utilizar uma ferramenta do Google chamada <a href="https://search.google.com/test/mobile-friendly" target="_blank" rel="noopener">Mobile-friendly Test</a> para verificar de forma automática se seu site funciona bem em um celular.</p>
<p>Basta colocar a url do seu site no campo que aparece na ferramenta e clicar em <strong>Run Test</strong>. Depois de fazer a análise a ferramenta vai mostrar se seu site está preparado para funcionar em um celular.</p>
<p><img loading="lazy" decoding="async" class="aligncenter size-full wp-image-4547" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-veririfcar-mobile-friendly.png" alt="" width="1187" height="633" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-veririfcar-mobile-friendly.png 1187w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-veririfcar-mobile-friendly-300x160.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-veririfcar-mobile-friendly-768x410.png 768w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-veririfcar-mobile-friendly-1024x546.png 1024w" sizes="(max-width: 1187px) 100vw, 1187px" /></p>
<p>Na imagem acima eu fiz um teste com a url <a href="https://jar.io" target="_blank" rel="noopener">https://jar.io</a> e ele mostrou a mensagem <strong>&#8220;Page is mobile friendly&#8221;.</strong> Estamos prontos para converter o site para um aplicativo.</p>
<p>Caso não apareça essa mensagem para você, será necessário fazer alguns ajustes em seu site antes de converte-lo.</p>
<h2><span id="Entendendo_sobre_a_WebView">Entendendo sobre a <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a></span></h2>
<p><img loading="lazy" decoding="async" class="aligncenter size-full wp-image-4562" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-entendendo.png" alt="" width="800" height="350" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-entendendo.png 800w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-entendendo-300x131.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-entendendo-768x336.png 768w" sizes="(max-width: 800px) 100vw, 800px" /></p>
<p>As <strong>WebViews</strong> permitem que você exiba o conteúdo de um site como parte do <a href="https://jar.iodesenvolvimento-android/android-layouts-viewgroups-intro/" target="_blank" rel="noopener">layout</a> de sua Acitivty, com recursos a mais do que os navegadores padrão.</p>
<p>Uma <strong><a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a></strong> é útil quando você precisa aumentar o controle sobre a interface do usuário e as opções avançadas de configuração que permitem incorporar páginas Web em um ambiente especialmente projetado para seu aplicativo.</p>
<p>A estrutura da <strong><a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a></strong> permite que você especifique as configurações que fazem com que suas páginas Web apareçam no tamanho e escala adequados em todas as configurações de tela.</p>
<p>Você pode até mesmo definir uma interface entre seu aplicativo Android e suas páginas Web que permite que o JavaScript nas páginas Web faça chamadas para APIs em seu aplicativo, fornecendo APIs do Android para seu aplicativo baseado na Web.</p>
<h2><span id="Comecando_o_Projeto">Começando o Projeto</span></h2>
<p><img decoding="async" loading="lazy" class="aligncenter size-full wp-image-4563" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-comecando-projeto.png" alt="" width="800" height="350" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-comecando-projeto.png 800w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-comecando-projeto-300x131.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-comecando-projeto-768x336.png 768w" sizes="(max-width: 800px) 100vw, 800px" /></p>
<p>Para começarmos a conversão do seu site em um aplicativo Android, crie um novo projeto no Android Studio escolhendo a opção de <strong>Empty Activity</strong> na penúltima tela de configuração.</p>
<p><img decoding="async" loading="lazy" class="aligncenter size-full wp-image-4551" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-projeto-android-studio.png" alt="" width="1301" height="744" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-projeto-android-studio.png 1301w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-projeto-android-studio-300x172.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-projeto-android-studio-768x439.png 768w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-projeto-android-studio-1024x586.png 1024w" sizes="(max-width: 1301px) 100vw, 1301px" /></p>
<p>Desta forma vamos ter um projeto com uma Activity e seu layout XML criada.</p>
<p>É a partir daqui que vamos começar a fazer as modificações para transformar nosso site em um aplicativos Android.</p>
<h2><span id="Adicionando_a_WebView">Adicionando a <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a></span></h2>
<p><img decoding="async" loading="lazy" class="aligncenter size-full wp-image-4564" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-adicionando.png" alt="" width="800" height="350" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-adicionando.png 800w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-adicionando-300x131.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-adicionando-768x336.png 768w" sizes="(max-width: 800px) 100vw, 800px" /></p>
<p>Vamos começar adicionando o componente XML da <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> no layout da nossa Activity.</p>
<p>Abra o arquivo <strong>activity_main.xml</strong> e substitua o conteúdo dela pelo código abaixo. Basicamente vamos utilizar um <a href="https://jar.iodesenvolvimento-android/android-layouts-viewgroups-intro/" target="_blank" rel="noopener">LinearLayout</a> com uma <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> dentro.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="xml">&lt;?xml version="1.0" encoding="utf-8"?&gt;
&lt;LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    tools:context=".MainActivity"&gt;

    &lt;<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a>
        android:id="@+id/<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">webview</a>"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        /&gt;

&lt;/LinearLayout&gt;</pre>
<p>O componente XML da <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> é bem simples e não tem muitas configurações para fazer. O restante dos controles vamos fazer em nossa classe <strong>MainActivity</strong>.</p>
<p>Abra a classe <strong>MainActivity</strong> e adicione o carregamento da URL na <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> no método <strong>onCreate</strong> como o exemplo abaixo.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="java">private <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> myWebView;

@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);

    myWebView = (<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a>) findViewById(R.id.<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">webview</a>);
    myWebView.loadUrl("https://jar.io");
}</pre>
<p>Precisamos adicionar também uma &#8220;permissão de uso&#8221; para o usuário acessar a Internet. Adicione a permissão de Internet dentro do seu <strong><a href="https://jar.iodesenvolvimento-android/androidmanifest/" target="_blank" rel="noopener">AndroidManifest</a></strong>.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="xml">&lt;?xml version="1.0" encoding="utf-8"?&gt;
&lt;manifest xmlns:android="http://schemas.android.com/apk/res/android"
    package="br.com.androidpro.androidprowebview"&gt;
    
    &lt;uses-permission android:name="android.permission.INTERNET"/&gt;

    &lt;application
        android:allowBackup="true"
        android:icon="@mipmap/ic_launcher"
        android:label="@string/app_name"
        android:roundIcon="@mipmap/ic_launcher_round"
        android:supportsRtl="true"
        android:theme="@style/AppTheme"&gt;
        &lt;activity android:name=".MainActivity"&gt;
            &lt;intent-filter&gt;
                &lt;action android:name="android.intent.action.MAIN" /&gt;

                &lt;category android:name="android.intent.category.LAUNCHER" /&gt;
            &lt;/intent-filter&gt;
        &lt;/activity&gt;
    &lt;/application&gt;

&lt;/manifest&gt;</pre>
<p>Execute o projeto no emulador ou em um celular físico para ver como está ficando.</p>
<p><img decoding="async" loading="lazy" class="aligncenter wp-image-4553 size-medium" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-1-teste-emulador-169x300.png" alt="" width="169" height="300" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-1-teste-emulador-169x300.png 169w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-1-teste-emulador-768x1365.png 768w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-1-teste-emulador-576x1024.png 576w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-1-teste-emulador.png 1080w" sizes="(max-width: 169px) 100vw, 169px" /></p>
<p>Se seu site aparecer no emulador quer dizer que já estamos com meio caminho andado. Porém algumas funcionalidades do seu site ainda podem não estar funcionando.</p>
<h2><span id="Habilitando_o_JavaScript">Habilitando o JavaScript</span></h2>
<p><img decoding="async" loading="lazy" class="aligncenter size-full wp-image-4565" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-habilitando-javascript.png" alt="" width="800" height="350" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-habilitando-javascript.png 800w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-habilitando-javascript-300x131.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-habilitando-javascript-768x336.png 768w" sizes="(max-width: 800px) 100vw, 800px" /></p>
<p>Se você está seguindo este tutorial e utilizou a mesma url que eu no projeto, vai perceber que ao tentar clicar no menu a esquerda do site, ele não faz nada. Isso acontece porque por padrão o JavaScript é desabilitado na <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a>.</p>
<p>Então, precisamos habilitar o JavaScript para que as funcionalidades do nosso site se comportem como se tivesse em um navegador no computador.</p>
<p>Para fazer isso, basta recuperar as configurações do <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> e habilitar o JavaScript.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="java">@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);

    myWebView = (<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a>) findViewById(R.id.<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">webview</a>);
    myWebView.loadUrl("https://jar.io");

    WebSettings webSettings = myWebView.getSettings();
    //Habilitando o JavaScript
    webSettings.setJavaScriptEnabled(true);
}</pre>
<p>Execute novamente o projeto e tente clicar no menu.</p>
<p><img decoding="async" loading="lazy" class="aligncenter size-full" src="https://media.giphy.com/media/7SEME1xOz8WHU5zr48/giphy.gif" width="270" height="480" /></p>
<p>Você vai perceber que agora o menu funciona.</p>
<h2><span id="Controlando_a_Navegacao">Controlando a Navegação</span></h2>
<p><img decoding="async" loading="lazy" class="aligncenter size-full wp-image-4566" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-navegacao.png" alt="" width="800" height="350" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-navegacao.png 800w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-navegacao-300x131.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-navegacao-768x336.png 768w" sizes="(max-width: 800px) 100vw, 800px" /></p>
<p>O comportamento padrão quando um usuário clica em um link dentro da página na <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a>, é abrir o aplicativo de navegador padrão do sistema. Isso pode prejudicar a experiência do usuário.</p>
<p>Para manter a navegação de página dentro do <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> e também dentro do aplicativo, precisamos criar uma subclasse de <a href="https://developer.android.com/reference/android/webkit/WebViewClient" target="_blank" rel="noopener"><strong>WebViewClient</strong></a> e substituir o método <strong>shouldOverrideUrlLoading</strong>.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="java">import android.app.Activity;
import android.content.Intent;
import android.net.Uri;
import android.webkit.<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a>;
import android.webkit.WebViewClient;


public class WebViewClientImpl extends WebViewClient {

    private Activity activity = null;

    public WebViewClientImpl(Activity activity) {
        this.activity = activity;
    }

    @Override
    public boolean shouldOverrideUrlLoading(<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">webView</a>, String url) {
        if(url.contains("androidpro.com.br")) return false;

        Intent intent = new Intent(Intent.ACTION_VIEW, Uri.parse(url));
        activity.startActivity(intent);
        return true;
    }

}</pre>
<p>Depois é só utilizar a classe no método <strong>onCreate</strong> da sua <strong>MainActivity</strong>.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="java">@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);

    myWebView = (<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a>) findViewById(R.id.<a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">webview</a>);

    WebViewClientImpl webViewClient = new WebViewClientImpl(this);
    myWebView.setWebViewClient(webViewClient);

    myWebView.loadUrl("https://jar.io");

    //Habilitando o JavaScript
    WebSettings webSettings = myWebView.getSettings();
    webSettings.setJavaScriptEnabled(true);
}</pre>
<p>Também precisamos implementar o botão <strong>Voltar</strong>, para que possamos navegar para as página anteriores visitadas.</p>
<p>Fazemos isso adicionando o método <strong>onKeyDown</strong> em nossa <strong>MainActivity</strong>.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="java">@Override
public boolean onKeyDown(int keyCode, KeyEvent event) {
    if ((keyCode == KeyEvent.KEYCODE_BACK) &amp;&amp; myWebView.canGoBack()) {
        myWebView.goBack();
        return true;
    }

    return super.onKeyDown(keyCode, event);
}</pre>
<p>O método <strong>onKeyDown</strong> foi substituído por uma implementação que primeiro verifica se o <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> pode voltar. Se o usuário tiver navegado para fora da primeira página carregada dentro do <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a>, o <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> poderá voltar.</p>
<p>O <a title="" class="aalmanual" target="_blank" href="https://developer.android.com/guide/webapps/webview?hl=pt-br">WebView</a> mantém um histórico de navegação como um navegador normal. Se não houver histórico, isso resultará no comportamento padrão do botão <strong>Voltar</strong>, ou seja, sair do aplicativo.</p>
<h2><span id="Personalizando_o_Aplicativo">Personalizando o Aplicativo</span></h2>
<p><img decoding="async" loading="lazy" class="aligncenter size-full wp-image-4567" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-personalizando.png" alt="" width="800" height="350" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-personalizando.png 800w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-personalizando-300x131.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-personalizando-768x336.png 768w" sizes="(max-width: 800px) 100vw, 800px" /></p>
<p>Vamos personalizar nosso aplicativo para incorporar ainda mais o site dentro dele e parecer uma coisa só.</p>
<p>A primeira coisa, é remover a &#8220;Action Bar&#8221; e deixar o site aparecendo quase em tela cheia. Para isso, vamos alterar o tema do nosso <strong><a href="https://jar.iodesign-layout/criando-styles-e-themes-no-android/" target="_blank" rel="noopener">Styles</a></strong>.</p>
<p>Abra o arquivo <strong>styles.xml</strong> e troque o atributo <strong>parent</strong> da tag <strong>&lt;style&gt;</strong> para <strong>Theme.AppCompat.NoActionBar</strong>.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="xml">&lt;resources&gt;

    &lt;!-- Base application theme. --&gt;
    &lt;style name="AppTheme" parent="Theme.AppCompat.NoActionBar"&gt;
        &lt;!-- Customize your theme here. --&gt;
        &lt;item name="colorPrimary"&gt;@color/colorPrimary&lt;/item&gt;
        &lt;item name="colorPrimaryDark"&gt;@color/colorPrimaryDark&lt;/item&gt;
        &lt;item name="colorAccent"&gt;@color/colorAccent&lt;/item&gt;
    &lt;/style&gt;

&lt;/resources&gt;
</pre>
<p>Precisamos também alterar as cores do aplicativo, e isso você faz alterando dentro do <strong>colors.xml</strong>. Seguindo as cores do meu site, eu configurei desta forma.</p>
<pre class="EnlighterJSRAW" data-enlighter-language="xml">&lt;?xml version="1.0" encoding="utf-8"?&gt;
&lt;resources&gt;
    &lt;color name="colorPrimary"&gt;#a4c629&lt;/color&gt;
    &lt;color name="colorPrimaryDark"&gt;#719500&lt;/color&gt;
    &lt;color name="colorAccent"&gt;#404040&lt;/color&gt;
&lt;/resources&gt;
</pre>
<p>Por último, vamos criar um ícone personalizado para nosso aplicativo.</p>
<p>Basicamente eu peguei o logo do AndroidPro e gerei o ícone utilizando está ferramenta <a href="http://assetstudio.androidpro.com.br/icons-launcher.html" target="_blank" rel="noopener">Gerador de Ícones de Launcher</a>.</p>
<p><img decoding="async" loading="lazy" class="aligncenter wp-image-4558 size-medium" src="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-icone-launcher-300x300.png" alt="" width="300" height="300" srcset="https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-icone-launcher-300x300.png 300w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-icone-launcher-150x150.png 150w, https://www.androidpro.com.br/wp-content/uploads/2018/09/webview-icone-launcher.png 512w" sizes="(max-width: 300px) 100vw, 300px" /></p>
<p>Basta fazer o download do arquivo ZIP gerado pela ferramenta e subistituir todas as pastas <strong>Mipmap</strong> de dentro do seu aplicativo.</p>
<p><img decoding="async" loading="lazy" class="aligncenter size-full" src="https://media.giphy.com/media/1ZtpCVJZFbCPEZVI9Q/giphy.gif" width="270" height="480" /></p>
<p>Pronto!</p>
