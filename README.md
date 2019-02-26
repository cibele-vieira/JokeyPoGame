# JokeyPoGame
O jogo do papel pedra e tesoura
from random import randint
from time import sleep
print ('\033[35;mJOKEY PO')
print('─┐　─┐')
print('│▒│ /▒/')
print('│▒│/▒/')
print('│▒ /▒/─┬─┐')
print('│▒│▒|▒│▒│ ')
print('│▒┌──┘▒▒▒│')
print('└┐▒▒▒▒▒▒┌┘')
print('└┐▒▒▒▒┌')
print('----------------------')
print ('\033[32;m[0] PEDRA')
print ('[1] PAPEL')
print ('[2] TESOURA')
print('----------------------')
jogador = int(input('Qual e sua jogada? '))
print('----------------------')
print('-=-'*10)
sleep(0.5)
print ('\033[0;33;mJo')
sleep(0.5)
print('Key')
sleep(0.5)
print('PO')
sleep(0.5)
print('-=-'*10)
itens = ('PEDRA','PAPEL','TESOURA')
sleep(0.5)
computador = randint(0,2)
print ('\033[34;m----------------------')
print('\033[34;m|PC - {}          -|'.format(itens[computador]))
print('|  X                 -|')
print('\033[34;m|VC - {}          -|'.format(itens[jogador]))
print ('\033[34;m----------------------')
if computador ==0: # Pedra

 if jogador ==0:
     print ('\033[7;35;mEMPATE')
 elif jogador ==1:
     print('\033[0;35;mPAPEL embrulha PEDRA')
     print(' VOCE GANHOU ')
 elif jogador ==2:
     print('PEDRA quebra TESOURA')
     print('\033[0;31;mVocê PERDEUUUU')
 else:
     print ('\033[34;mJogada inválida!')



elif computador == 1:#papel

    if jogador == 0:
        print('=-=-=-=-=-==-PAPEL embrulha PEDRA')
        print('\033[0;31;mVocê PERDEUUUU')
    elif jogador == 1:
        print('\033[7;30;mEMPATE')
    elif jogador == 2:
        print('-=-=-=-=-=-=-=TESOURA corta PAPEL')
        print('VOCE GANHOU')

elif computador == 2:#tesoura

    if jogador == 0:
        print('\033[0;35;m -=-=-=-=-=-=PEDRA quebra TESOURA')
        print('VOCE GANHOU')
    elif jogador == 1:
        print('-=-=-=-==-=-=-=-=TESOURA corta PAPEL')
        print('\033[0;31;mVocê PERDEUUUU')
    elif jogador == 2:
        print('\033[7;35;mEMPATE')
