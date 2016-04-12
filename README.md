# template-libray-CI3.x
Library para usar template no CI3.x

# Instalação e uso

- Colocar o arquivo layout.php dentro da pasta application/library de seu projeto;
- Habilitar no arquivo config/autoload.php a library 'layout';
- Criar diretório layouts dentro de application/views;
- Criar arquivo layout.php dentro do diretório application/views/layouts Esse arquivo será sua estrutura da aplicação, com o HTML completo, com os heads, menu, topo, rodapé, etc.
- Colocar o codigo <?php echo $content_for_layout?> onde deseja que a view seja carregada;
- No controller, substituir a chamada $this->load->view por $this->layout->view. Os parâmetros são os mesmos;
- Caso desejar usar outro layout, basta chamar o método $this->layout->setLayout('layouts/outro_layout');

### Não me lembro o autor dessa classe. Por favor, entrar em contato para que possa citar o nome do autor. Apenas adaptei para PHP 5.x+.
