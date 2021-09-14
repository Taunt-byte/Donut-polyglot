# Donut

Status: Pronto

## Sobre

+ É uma rosquinha que se mexe no terminal
+ Foi feita em 2006 usando a linguagem C
+ O link para a materia feita pelo autor esta abaixo:
    
    <code>https://www.a1k0n.net/2011/07/20/donut-math.html</code>

## Como funciona ?

Em seu núcleo, é um framebuffer e um Z-buffer no qual se renderiza pixels. Uma vez que está apenas renderizando arte ASCII de resolução relativamente baixa, eu trapaceio maciçamente. Tudo o que ele faz é plotar pixels ao longo da superfície do toro em incrementos de ângulo fixo, e o faz com densidade suficiente para que o resultado final pareça sólido. Os “pixels” que plota são caracteres ASCII correspondentes ao valor de iluminação da superfície em cada ponto:., - ~:; =! * # $ @ Do mais escuro ao mais brilhante. Nenhum raytracing necessário.

Então, como fazemos isso? Bem, vamos começar com a matemática básica por trás da renderização em perspectiva 3D. O diagrama a seguir é uma vista lateral de uma pessoa sentada em frente a uma tela, visualizando um objeto 3D atrás dela.


## Começando
