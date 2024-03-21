# aprendendo este [exemplo](https://phaser.io/tutorials/making-your-first-phaser-3-game/part9)
# eu entendi que tem que colocar dois tipos diferentes de coisas em locais diferentes 
# dentro do create - as coisas que não vão mudar
# dentro do update - as coisas que vão mudar 

###### é mais importante eu primeiro ver todo o exemplo desto jogo em phaser e so depois ir mexendo no meu jogo ? se esse for o caso e preciso voltar denovo para o exemplo deste jogo e ver o pedaço que preciso para o meu jogo

###### é mais importante assim que eu entender como funciona a funcionalidade eu ja ir implementando e somente fazer um tutorial passo a passo ter um jeito mais rapido e acessar quando eu esquecer 

<br/>

# 19 mar - 2h30 parei no exemplo 7

# 20 mar - 30' parei no exemplo 8

# 21 mar - 16' terminei o resto do exemplo 8
### dúvida : // se overlap é uma coisa que vai mudar porque não é feito no updating ?
###### este exemplo eu posso usar para  colocar a ideia da arturia(vai adicionar mais tempo ) ou do professor de aumentar os pontos de score quando o jogador coletar , 
###### ai seria assim passou 1 labirinto por minuto tem 10 pontos
###### ai seria assim passou 2 labirinto por minuto tem 20 pontos
###### ai seria assim passou 3 labirinto por minuto tem 30 pontos

###### pegou um quadradinho tem 2 pontos



###### aqui eu tive uma ideia o jogo o chção é larva - aí a pessoa precisaa ficar pulando dirteto de um jeito que não encoste no chão - pedaço em cima da plataforma e ela tem e ir passando entre as plataformas sem encostar no chão , aí eu coloco a colisão do pesonagem somente com o pedaço de cima da palaforma para ele explodir , e quando ele encosta no pedaço debaixo da plataforma ele não explodi

# 21 mar - 12' terminei o exemplo 9
###### #a mesma função que detecta quando jogador colide com estrela( tira fisica da estrela tocada e a remove ) é a mesma função que aumenta o score     
###### #dentro do update() eu chamo a função que faz isso e esta função n esta dentro do update() 
###### # as variaveis devem ser globais logo , devo criar elas dentro do arquivo script e n dentro de alguma função , mas dentro das funões é que altero o valor delas 


# 21 mar - 20' começei o exemplo 10
# adicionei uma atividade 21 no jogo from the ashes parecido com a lógica do baddies feito no exemplo parte 10

##  por exemplo esta funçaão para a pessoa jogadora pensar que é possivel passar mas n semdo possivel pois o bloco pareide apenas fica piscando cor do bloco pareide e branco e assim continua ficando pareide (player.setTint(0xff0000);)
# `The bombs will of course bounce off the platforms, and if the player hits them we'll call the hitBomb function. All that will do is stop the game and turn the player red:

function hitBomb (player, bomb)
{
    this.physics.pause();

    player.setTint(0xff0000);

    player.anims.play('turn');

    gameOver = true;
}`

# parei aqui neste frase `So far, so good, but we need to release a bomb. `