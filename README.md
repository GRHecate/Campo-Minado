# Campo-Minado
Projeto Algoritmos 

Pseudocódigo jogo

def game():
    define o tamanho do tabuleiro
    controla a quantidade de minas
    exibe o tabuleiro
        exibe o tabuleiro a cada jogada
        exibe somente os quadradinhos já descobertos (visão do jogador)
    tabuleiro atualizado
   chama as outras funções 
        	initialize()
    	print()
    	step()
    	status()

def initialize():
     devolve uma matriz já com as minas espalhadas na matriz e nas outras	
posições onde não tiver minas deve preencher com quantas minas há nos quadradinhos
adjacentes. Espalhar as minas de forma aleatória na matriz.
    
def print():
    imprime o campo na visão jogador
    
def step():
    Essa função recebe o campo minado, uma posição e uma ação do jogador a ser feita no campo minado (revelar ou marcar a posição). 

    if o solicitado a ação revelar a posição e o jogador tenha sucesso:
        retornar -1 (o	jogo	pode	continuar)
    if tenha uma mina na posição solicitada para revelar:
        retornar 0 (jogador perdeu)
    if  solicitado marcar a posição:
        retornar 1 (jogo continua e quantidade de minas é decrementada)

    retornar matriz atualizada
    
#def status():
    if jogador encontrou todas as minas (abriu todos os quadradinhos sem minas):
        return True

game()    
